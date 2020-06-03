---
title: CChkSGFiles.ErrCheckLogs 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 71e21bb3a748a532f9e3167e0b36898acde71b02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526719"
---
# <a name="cchksgfileserrchecklogs-function"></a>CChkSGFiles.ErrCheckLogs 関数

**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
**ErrInit** 関数で指定されたすべてのデータベース ファイルのログ ファイルを検証します。 検証済みログ ファイルは、**ErrInit** に渡されたパス内に存在し、3 文字のベース ログ ファイル名を持っているものです。
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>パラメーター

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
出力パラメーターです。 **True**の場合、このパラメーターは、トランザクションログファイルにエラーが見つかったことを示しますが、データを失わずにデータベースをクリーンシャットダウン状態にするために必要ではないログファイルにこれらのエラーが含まれていました。 このパラメーターに返される**実際**の値は、 **Errchecklogs**が**errsuccess**を返す場合にのみ有効です。 
    
### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。 
  
ログファイルでエラーが検出された場合でも、この関数は**Errsuccess**を返すことに注意してください。 そのため、 **Errchecklogs**が**errsuccess**を返すと、アプリケーションは**pfOnlyUnnecessaryLogsCorrupt** return パラメーターも確認する必要があります。 **ErrCheckLogs** が **errSuccess** を返したときに、**pfOnlyUnnecessaryLogsCorrupts** が **true** の場合は、データベースを最新状態にする必要のないログ ファイルにのみ、1 つ以上のエラーが見つかったことを意味します。
  
## <a name="remarks"></a>注釈

**ErrCheckDbHeaders** 関数は、**ErrCheckLogs** 関数よりも先に呼び出す必要があります。 
  
Exchange データベースのトランザクションログファイルがチェックされている場合、データを失わずにストレージグループ内のデータベースをクリーンシャットダウン状態にするために、一部のログファイルが必要になることがありますが、その他のログファイルは必要ない場合があります。 **Errchecklogs**関数は、データベースを最新の状態にするために必要な最古および最新のログファイルの両方を決定します。 
  
**ErrCheckLogs** 関数は、**ErrInit** 関数に渡したものと同じに、指定したパス内にある指定した 3 文字のベース ファイル名を持つすべてのログ ファイルを検証します。 
  
ログ ファイルにエラーが見つからない場合、**ErrCheckLogs** は **errSuccess** を返します。 
  
必要とされるログ ファイルのいずれかに破損が見つかると、**ErrCheckLogs** はエラーを返します。 
  
必要とされる最古のログ ファイルよりも古いログ ファイルにのみエラーが見つかった場合、この関数は **errSuccess** を返して、戻り値パラメーター **pfOnlyUnnecessaryLogCorrupt** を **true** に設定します。 アプリケーションでは、そうした古いログ ファイルの一部にエラーが存在することを認識する必要があり、該当する場合にはユーザーに警告するようにします。 いずれにしても、こうしたエラーがデータベースの全体的な整合性に影響することや、ログ フォワードの実行が成功するかどうかに影響することはありません。
  
**ErrCheckLogs** が必要であると判断した最古のログよりも後に作成されたログ ファイルにエラーが見つかった場合、この関数はエラーを返します。 データベースを最新状態にするために必要になるログ ファイルよりも後に生成されたものにログ ファイル エラーが見つかった場合にも、エラーが返されます。 識別されたログ ファイルを使用してデータベースをクリーン シャットダウン状態にすることは可能ですが、それよりも後の破損したログ ファイルで指定されたトランザクションは適用されないため、データベースの復元時にデータを損失することになります。 
  
**CChkSGFiles** オブジェクトでは、**ErrInit** 関数で登録したすべてのログ ファイルが実際に確認されたかどうかを判別します。 正常に確認されなかったログがあると、**ErrTerm** 関数はエラーを返します。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのマルチスレッドの部分で **ErrCheckLogs** 関数を呼び出すことができますが、**CCheckSGFiles** オブジェクトごとに 1 回しか呼び出せません。 
  
## <a name="requirements"></a>Requirements

Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

