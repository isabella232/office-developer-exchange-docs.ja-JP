---
title: CChkSGFiles.New 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: e50b41e761b8e46d778011b6bac3db4dbb624809
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516273"
---
# <a name="cchksgfilesnew-function"></a>CChkSGFiles.New 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
**CChkSGFiles** クラスの新しいインスタンスを作成します。この関数を呼び出してから、確認するストレージ グループとデータベースを指定する必要があります。 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>パラメーター

なし。
  
## <a name="return-value"></a>Return value

新しく作成されたオブジェクトへの参照 (ポインター)。
  
## <a name="remarks"></a>注釈

**New** 関数は、**CCheckSGFiles** オブジェクトを作成して、そのオブジェクトへの参照 (ポインター) を呼び出し元に返します。この関数を最初に呼び出してから、**CCheckSGFiles** クラスのその他の関数を呼び出す必要があります。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **New** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。  
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

