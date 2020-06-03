---
title: CChkSGFiles.ERR 列挙型
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: '最終更新日: 2015 年 3 月 9 日'
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455255"
---
# <a name="cchksgfileserr-enumeration"></a>CChkSGFiles.ERR 列挙型 
  
**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
呼び出された関数の結果を示します。 この列挙型は、**CCheckSGFiles** クラスの多数の関数によって返されます。 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a>値

|**メンバー名**|**値**|**説明**|
|:-----|:-----|:-----|
|errSuccess  <br/> |.0  <br/> |関数はエラーなしで正常に終了しました。  <br/> |
|errTaskDropped  <br/> |-106  <br/> |**ErrTerm** 関数によって返され、一部のデータベース ページとトランザクション ログ ファイルがチェックされなかったことや、検証中にエラーが発生したことを示します。  <br/> |
|errRequiredLogFilesMissing ありません  <br/> |-543  <br/> |データベースをクリーン シャットダウン状態にするために必要な 1 つ以上のログ ファイルがログ ファイル パスに見つからなかったか、指定された 3 文字のベース名がありませんでした。  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |関数に渡された 1 つ以上のパラメーターが正しくありません。  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |メモリ不足のため、要求された操作を完了できませんでした。  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |データベース ページに格納されているチェックサムが、予期されるチェックサムと一致しません。  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |オブジェクトの使用中に、**ErrTerm** 関数が呼び出されました。 **ErrTerm** が、**ErrCheckDbPages** や **ErrCheckLogFiles** が返される前に呼び出されると、この状況が生じることがあります。  <br/> |
   
## <a name="requirements"></a>Requirements

Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

