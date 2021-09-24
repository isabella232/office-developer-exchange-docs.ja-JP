---
title: CChkSGFiles.CMaxDbPerSG 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 1a82e71afde4766734d0875f68d7932a9fd9f26a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510526"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>CChkSGFiles.CMaxDbPerSG 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
1 つの Exchange サーバー ストレージ グループに許容されるデータベースの最大数を返します。
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>パラメーター

なし。
  
## <a name="return-value"></a>Return value

指定した Exchange サーバーでストレージ グループごとに許容されるデータベースの最大数。 ストレージ グループは 2013 年Exchangeの一部ではないので、この関数は 1 を返します。
  
## <a name="remarks"></a>注釈

**CCheckSGFiles** オブジェクトを使用すると唯一のストレージ グループに含まれるデータベース (およびトランザクション ログ ファイル) を検証できます。そのため、**CMaxDbPerSG** 関数から返される値もデータベースの最大数を表すことになります。これは、**CCheckSGFiles** クラスのインスタンスを使用することで確認できます。  
  
既定では、2003 Exchange Server 2007 Exchange Serverは、ストレージ グループごとに最大 5 つのデータベースを許可します。
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

