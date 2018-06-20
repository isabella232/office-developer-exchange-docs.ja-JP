---
title: CChkSGFiles.New 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758856"
---
# <a name="cchksgfilesnew-function"></a>CChkSGFiles.New 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
**CChkSGFiles**クラスの新しいインスタンスを作成します。 チェックするには、ストレージ グループおよびデータベースを指定する前に、この関数を呼び出す必要があります。 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Parameters

なし。
  
## <a name="return-value"></a>Return value

新しく作成されたオブジェクトへの参照 (ポインター)。
  
## <a name="remarks"></a>備考

**新規**の関数は、 **CCheckSGFiles**オブジェクトを作成し、そのオブジェクトへの参照 (ポインター) を呼び出し元に返します。 **CCheckSGFiles**クラスのすべての他の関数を呼び出す前にこの関数を呼び出す必要があります。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、シングル スレッド アプリケーションの部分で、**新規**の関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

