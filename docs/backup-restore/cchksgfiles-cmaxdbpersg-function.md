---
title: CChkSGFiles.CMaxDbPerSG 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759824"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>CChkSGFiles.CMaxDbPerSG 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
1 つの Exchange サーバー ストレージ グループに許容されるデータベースの最大数を返します。
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Parameters

なし。
  
## <a name="return-value"></a>Return value

指定された Exchange サーバーでは、ストレージ グループあたりのデータベースの最大数です。 ストレージ ・ グループは Exchange 2013 の一部ではないため、この関数は 1 を返します。
  
## <a name="remarks"></a>備考

**CMaxDbPerSG**関数によって返される値もチェックを使用してデータベースの最大数を表すように、1 つのストレージ ・ グループに (データベースとトランザクション ログ ファイル) を検証する**CCheckSGFiles**オブジェクトを使用することができます、**CCheckSGFiles**クラスのインスタンスです。 
  
既定では、Exchange Server 2003 と Exchange Server 2007 を許可する最大のストレージ グループあたり 5 データベースに注意してください。
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

