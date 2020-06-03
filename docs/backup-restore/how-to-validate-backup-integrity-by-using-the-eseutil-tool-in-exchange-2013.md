---
title: Exchange 2013 で Eseutil ツールを使用してバックアップの整合性を検証する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。
ms.openlocfilehash: e8f1a46e2d94729ae5586861317312e277216d63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452798"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Exchange 2013 で Eseutil ツールを使用してバックアップの整合性を検証する

Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。 
  
**製品:** Exchange Server 2013 
  
ボリューム シャドウ コピー サービス (VSS) により、Exchange はデータベースへの書き込みを停止することなくバックアップを作成できるようになるため、サーバーはすべてのページを操作することも、必要な整合性検査を実行することもありません。 このため、VSS を使用するバックアップおよび復元アプリケーションは、スナップショットの整合性を検証する必要があります。 Exchange Server 2013 は、スナップショットの整合性を確認するための次の2つの方法をサポートしています。 
  
- CHKSGFILES API
    
- Eseutil コマンドライン ツール
    
CHKSGFILES API を使用することをお勧めします。これは、バックアップアプリケーションが、CHKSGFILES 整合性チェック中に検出されたエラーを検出、診断、および報告するのが簡単なためです。 CHKSGFILES API の使用方法については、「 [Exchange 2013 で CHKSGFILES api を使用してバックアップの整合性を検証](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)する」を参照してください。
  
## <a name="running-the-eseutil-tool"></a>Eseutil ツールの実行

スナップショットの整合性を検査するには、次の表で特定されるデータベース ファイルとログ ファイルに対して Eseutil コマンドを実行します。  
  
**表 1.バックアップの種類ごとの Eseutil.exe コマンド**

|**ファイルの種類/バックアップの種類**|**完全バックアップ**|**コピー バックアップ**|**増分バックアップ**|**差分バックアップ**|
|:-----|:-----|:-----|:-----|:-----|
|.edb  <br/> |"eseutil /k /i"  <br/> |"eseutil /k /i"  <br/> |該当なし  <br/> |該当なし  <br/> |
|.log  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (2)  <br/> |"eseutil /k" (2)  <br/> |
   
> [!NOTE]
> .stm ファイルと .chk ファイルには、Eseutil コマンドを実行する必要はありません。 
  
スナップショット データベースを復旧するには、チェックポイント ログの世代番号以上のログ ファイル世代番号が付いたすべてのログ ファイルが必要になります。 存在する場合は、現在のログ ファイル (Enn.log) もデータベースの復旧に必要になります。 必要なログファイルのいずれかが整合性チェックに失敗した場合、リクエスターは、 [BackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa382651%28v=vs.85%29.aspx)メソッドを呼び出す前に、バックアップコンポーネントの状態が FALSE に設定されていることを確認する必要があります。 チェックポイント ログ ファイルを識別するには、スナップショット チェックポイント ファイルに対して Eseutil.exe を実行して、"Checkpoint:" の出力を解析します。 次の例は、チェックポイント ファイルに対して Eseutil.exe を実行する方法を示しています。 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

この例の 2 行目は戻り値です。0x20 は、チェックポイント ログ ファイルのログ世代番号 (16 進数) です。この例では、スナップショット データベースの復旧には E01000020.log 以降のログ ファイルに破損がないことが必要です。これは、データベース自体が物理的な整合性検査に合格していても同じことです。
  
データベースの復旧には、増分バックアップまたは差分バックアップのセットに含まれるすべてのログ ファイルが必要になります。ログ シーケンスの整合性は、ログ ファイルのプレフィックスに対して Eseutil.exe を実行することで検査できます。次の例は、特定のパスにある E01xxxxx.log という形式のすべてのログ ファイルに対して整合性検査を実行する方法を示しています。
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Eseutil.exe の出力の確認

要求側は、負でない値で返される終了 ERRORLEVEL エラーをすべて検証する必要があります。 ERRORLEVEL 値の詳細については、「[一般的な Eseutil エラーのリファレンス](https://technet.microsoft.com/library/aa996759%28v=exchg.80%29.aspx)」を参照してください。 コマンド ラインで ERRORLEVEL を確認するには、Eseutil.exe の実行終了後に「echo %errorlevel%」と入力します。 負の ERRORLEVEL は、1 つ以上のファイルが破損していることを示します。
  
リクエスターが**BackupComplete**メソッドを呼び出す前に、バックアップコンポーネントの状態が整合性チェックの結果を反映していることを確認する必要があります。 破損が見つかった場合は、状態は FALSE になります。破損が検出されなかった場合、状態は TRUE になります。 
  
## <a name="see-also"></a>関連項目

- [Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Exchange 2013 のバックアップと復元アプリケーションの作成](build-backup-and-restore-applications-for-exchange-2013.md)
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

