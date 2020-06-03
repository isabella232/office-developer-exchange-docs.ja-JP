---
title: CChkSGFiles.NO_FLAGS 列挙型
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NO_FLAGS
api_type:
- dllExport
ms.assetid: 6b18b645-fec4-429a-9900-62ad0f19bf96
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: a55bcf2c845b6896105d446a14a70cc45fbc3de2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455360"
---
# <a name="cchksgfilesno_flags-enumeration"></a><span data-ttu-id="35096-103">CChkSGFiles.NO_FLAGS 列挙型</span><span class="sxs-lookup"><span data-stu-id="35096-103">CChkSGFiles.NO_FLAGS enumeration</span></span>

<span data-ttu-id="35096-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="35096-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="35096-105">ほとんどの **CCheckSGFiles** クラスの関数によって受け入れられる **ulFlags** パラメーターのプレース ホルダーの値として機能します。</span><span class="sxs-lookup"><span data-stu-id="35096-105">Serves as a placeholder value for the **ulFlags** parameters that are accepted by most **CCheckSGFiles** class functions.</span></span> 
  
```cs
Enum { NO_FLAGS = 0 }

```

## <a name="requirements"></a><span data-ttu-id="35096-106">Requirements</span><span class="sxs-lookup"><span data-stu-id="35096-106">Requirements</span></span>

<span data-ttu-id="35096-107">Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="35096-107">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="35096-108">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="35096-108">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

