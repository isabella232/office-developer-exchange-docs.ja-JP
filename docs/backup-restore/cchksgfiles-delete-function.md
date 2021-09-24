---
title: CChkSGFiles.Delete 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: cf1c23dd75442d73dfea49e0831d0859da321a40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510541"
---
# <a name="cchksgfilesdelete-function"></a>CChkSGFiles.Delete 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
**CChkSGFiles** クラスの既存のインスタンスを破棄します。この関数は、アプリケーションが特定のオブジェクトの操作を完了した後で呼び出す必要があります。 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>パラメーター

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
入力パラメーター。既存の **CCheckSGFiles** オブジェクトへのポインターです。オブジェクトに関連付けられていたメモリは解放されます。 
    
## <a name="return-value"></a>Return value

なし。
  
## <a name="remarks"></a>注釈

**Delete** 関数は、**CCheckSGFiles** オブジェクトに関連付けられていたメモリを解放します。 Delete を呼び **出** した後  *、pcchecksgfiles*  パラメーターで渡されたポインターは無効であり、そのオブジェクトに対して他の操作を実行できません。 
  
アプリケーションで **ErrCheckDbPages** 関数を使用する場合、そのアプリケーションではメモリ バッファーを手動で開放する必要があります。**Delete** 関数はメモリ バッファーを解放しません。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **Delete** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。  
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

