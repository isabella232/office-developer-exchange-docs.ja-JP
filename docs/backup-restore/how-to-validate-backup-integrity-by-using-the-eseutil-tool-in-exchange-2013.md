---
title: Exchange 2013 の Eseutil ツールを使用してバックアップの整合性を検証します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。
ms.openlocfilehash: 03c4c23d433418911240bbe7c337308a989f3739
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758857"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Exchange 2013 の Eseutil ツールを使用してバックアップの整合性を検証します。

Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。 
  
**に適用されます:** Exchange Server 2013 
  
ボリューム シャドウ コピー サービス (VSS) は、Exchange のデータベースへの書き込み中に、バックアップを作成できます、ため、サーバーはすべてのページを修正されず、必要な整合性チェックを実行します。 このため、VSS を使用するバックアップと復元のアプリケーションは、スナップショットの整合性を確認してください。 Exchange Server 2013 には、スナップショットの整合性をチェックするための次の 2 つの方法がサポートされています。 
  
- CHKSGFILES API
    
- Eseutil コマンドライン ツール
    
検出、診断、バックアップ ・ アプリケーションをより簡単にし、CHKSGFILES の一貫性の時に検出されたエラーの報告を確認するためには、CHKSGFILES API を使用することをお勧めします。 CHKSGFILES API を使用する方法の詳細については、 [Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)を参照してください。
  
## <a name="running-the-eseutil-tool"></a>Eseutil ツールの実行

スナップショットの整合性を検査するには、次の表で特定されるデータベース ファイルとログ ファイルに対して Eseutil コマンドを実行します。  
  
**表 1 です。バックアップの種類ごとに、Eseutil.exe コマンド**

|**ファイルの種類とバックアップの種類**|**フル ・ バックアップ**|**コピー バックアップ**|**インクリメンタル ・ バックアップ**|**差分バックアップ**|
|:-----|:-----|:-----|:-----|:-----|
|.edb  <br/> |"eseutil /k /i"  <br/> |"eseutil /k /i"  <br/> |適用できません  <br/> |適用できません  <br/> |
|.log  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (1)  <br/> |"eseutil /k" (2)  <br/> |"eseutil /k" (2)  <br/> |
   
> [!NOTE]
> .stm ファイルと .chk ファイルには、Eseutil コマンドを実行する必要はありません。 
  
番号、ログ ファイルの生成を持つすべてのログ ファイルは、生成のチェックポイントのログ ファイルの数、スナップショット データベースをリカバリするために必要以上には。 、存在する場合は現在のログ ファイル (Enn.log) がデータベースのリカバリに必要なも。 必要なログ ファイルには、整合性チェックが失敗した場合、依頼者は、 [BackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382651%28v=vs.85%29.aspx)メソッドを呼び出す前に、バックアップ コンポーネントの状態を FALSE に設定されていることを確認してください。 チェックポイント ・ ログ ・ ファイルを識別するには、スナップショットのチェックポイント ファイルに対して Eseutil.exe を実行し、解析の出力」のチェックポイント:.」 次の例では、チェックポイント ・ ファイルに対して Eseutil.exe を実行する方法を示します。 
  
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

依頼者は、すべて終了 ERRORLEVEL エラー値が返されますが負でないことを確認してください。 ERRORLEVEL の値については、[一般的な Eseutil エラーのリファレンス](http://technet.microsoft.com/en-us/library/aa996759%28v=exchg.80%29.aspx)を参照してください。 コマンドラインで ERRORLEVEL を表示するには、入力「エコー % エラーレベル %」Eseutil.exe の実行が完了した後です。 負のエラー レベルは、1 つまたは複数のファイルが破損していることを示します。
  
リクエスターは、 **BackupComplete**メソッドを呼び出して、前に、バックアップ コンポーネントの状態に整合性チェックの結果が反映されていることを確認してくださいする必要があります。 破損が見つかった場合はステータスになります。破損が検出されず、状態が TRUE になります。 
  
## <a name="see-also"></a>関連項目

- [Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [バックアップを作成し、Exchange 2013 のアプリケーションを復元します。](build-backup-and-restore-applications-for-exchange-2013.md)
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

