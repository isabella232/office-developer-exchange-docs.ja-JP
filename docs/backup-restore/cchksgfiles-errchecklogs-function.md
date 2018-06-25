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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758864"
---
# <a name="cchksgfileserrchecklogs-function"></a>CChkSGFiles.ErrCheckLogs 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
**ErrInit**関数で指定されたすべてのデータベース ファイルのログ ファイルを検証します。 検証済みのログは、パス内に存在し、 **ErrInit**に渡される 3 文字ベースのログ ファイル名があります。
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parameters

### <a name="pfonlyunnecessarylogscorrupt"></a>pfOnlyUnnecessaryLogsCorrupt 
  
出力パラメーターです。 **True の場合**、このパラメーターを示しますが、トランザクション ・ ログ ・ ファイル、これらのエラーのエラーが検出されたことがとされたに不要なログ ファイル内に見つかったすべてデータベース クリーン シャット ダウン状態にデータを失わずにします。 このパラメーターに返される**場合は true**の値は、 **ErrCheckLogs**には、 **errSuccess**が返されるときにのみに有効です。 
    
### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>�߂�l

[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。 
  
ログ ファイルにエラーが検出された場合でも、この関数に**errSuccess**を返すことができますを覚えておく必要があります。 したがって、 **ErrCheckLogs**に**errSuccess**が返されるとき、アプリケーションもを確認する**pfOnlyUnnecessaryLogsCorrupt**の戻り値パラメーター。 **ErrCheckLogs**に**errSuccess**が返されるときに**pfOnlyUnnecessaryLogsCorrupts**が**true**の場合は、データベースを最新にする必要がないログ ファイルでは、1 つまたは複数のエラーが検出されたことを示します。
  
## <a name="remarks"></a>備考

**ErrCheckLogs**関数が呼び出される前に、 **ErrCheckDbHeaders**関数を呼び出す必要があります。 
  
Exchange データベースのトランザクション ログ ファイルをチェックすると、ログ ファイルのいくつか必要がありますデータが失われることがなく、クリーン シャット ダウン状態にストレージ グループ内のデータベースをオンラインにその他のログ ファイルは必要はありませんが。 **ErrCheckLogs**関数は、最も古いと最新のデータベースを表示するために必要な最新のログ ファイルの両方を決定します。 
  
**ErrCheckLogs**関数は、 **ErrInit**関数に渡されるときにも、指定した 3 文字ベース ファイル名を持つ、指定したパス内のすべてのログ ファイルを確認します。 
  
ログ ファイルでエラーが見つからない場合、 **ErrCheckLogs**は**errSuccess**を返します。 
  
必要なログ ファイルのいずれかが壊れている可能性がある、 **ErrCheckLogs**はエラーを返します。 
  
必要な最初のものよりも古いログ ファイルでのみエラーが見つかった場合、この関数は**errSuccess**を返し、 **pfOnlyUnnecessaryLogCorrupt**の戻り値パラメーターを**true**に設定。 これら古いログ ・ ファイルの一部にエラーがある場合は、その可能性がある警告が表示されます、アプリケーションが認識する必要があります。 いずれの場合も、これらのエラーしないデータベースの全体的な整合性に影響を与えるか、ログ フォワードを実行が成功するかどうかに影響を与えます。
  
最も早く訪れる後に作成された任意のログ ファイルにエラーが見つかった場合は、 **ErrCheckLogs**を決定するログが必要な関数はエラーを返します。 後に生成されたログ ファイルは、ログ ファイルのエラーが見つかった場合でも最新状態にするために必要なのエラーが返されます。 特定のログ ファイルを使用してクリーン シャット ダウンの状態にデータベースを移動することですが、後で破損したログ ファイルで指定されているトランザクションは適用されません、データベースが復元されたときにデータが失われる結果。 
  
**CChkSGFiles**オブジェクトは、実際にチェック アウトされたすべてのログ ファイルを**ErrInit**関数に登録されているかどうかを決定します。 表示しない場合は、すべてのログがない正常にチェック、 **ErrTerm**関数はエラーを返します。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **ErrCheckLogs**関数を呼び出すことができますが、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

