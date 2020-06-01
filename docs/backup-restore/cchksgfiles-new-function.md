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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455234"
---
# <a name="cchksgfilesnew-function"></a>CChkSGFiles.New 関数

**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
**CChkSGFiles** クラスの新しいインスタンスを作成します。 この関数を呼び出してから、確認するストレージ グループとデータベースを指定する必要があります。 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>パラメーター

なし。
  
## <a name="return-value"></a>Return value

新しく作成されたオブジェクトへの参照 (ポインター)。
  
## <a name="remarks"></a>注釈

**New** 関数は、**CCheckSGFiles** オブジェクトを作成して、そのオブジェクトへの参照 (ポインター) を呼び出し元に返します。 この関数を最初に呼び出してから、**CCheckSGFiles** クラスのその他の関数を呼び出す必要があります。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **New** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。  
  
## <a name="requirements"></a>Requirements

Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

