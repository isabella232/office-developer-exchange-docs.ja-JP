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
description: '�ŏI�X�V��: 2015�N3��9��'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759807"
---
# <a name="cchksgfileserr-enumeration"></a>CChkSGFiles.ERR 列挙型 
  
**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
呼び出された関数の結果を示します。 **CCheckSGFiles**クラスの多くの関数では、この列挙体が返されます。 
  
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
|errSuccess  <br/> |0  <br/> |関数はエラーなしで正常に終了しました。  <br/> |
|errTaskDropped  <br/> |-106  <br/> |すべてのデータベース ページとトランザクション ログ ファイルがオンになっているかの検証中にエラーが発生したことを示すために**ErrTerm**関数によって返されます。  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |データベースをクリーン シャットダウン状態にするために必要な 1 つ以上のログ ファイルがログ ファイル パスに見つからなかったか、指定された 3 文字のベース名がありませんでした。  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |関数に渡された 1 つ以上のパラメーターが正しくありません。  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |メモリ不足のため、要求された操作を完了できませんでした。  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |データベース ページに格納されているチェックサムが、予期されるチェックサムと一致しません。  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |オブジェクトがまだ使用されているときに、 **ErrTerm**関数が呼び出されました。 これは、 **ErrCheckDbPages**する前に**ErrTerm**が呼び出されるまたは**ErrCheckLogFiles**が返された場合に発生します。  <br/> |
   
## <a name="requirements"></a>必要条件

Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

