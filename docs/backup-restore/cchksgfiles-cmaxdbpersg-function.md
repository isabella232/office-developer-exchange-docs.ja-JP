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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455262"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>CChkSGFiles.CMaxDbPerSG 関数

**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
1 つの Exchange サーバー ストレージ グループに許容されるデータベースの最大数を返します。
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>パラメーター

なし。
  
## <a name="return-value"></a>Return value

指定した Exchange サーバーでストレージ グループごとに許容されるデータベースの最大数。 ストレージグループは Exchange 2013 の一部ではないため、この関数は1を返します。
  
## <a name="remarks"></a>注釈

**CCheckSGFiles** オブジェクトを使用すると唯一のストレージ グループに含まれるデータベース (およびトランザクション ログ ファイル) を検証できます。そのため、**CMaxDbPerSG** 関数から返される値もデータベースの最大数を表すことになります。これは、**CCheckSGFiles** クラスのインスタンスを使用することで確認できます。  
  
既定では、Exchange Server 2003 および Exchange Server 2007 では、ストレージグループごとに最大5つのデータベースが許可されていることに注意してください。
  
## <a name="requirements"></a>Requirements

Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

