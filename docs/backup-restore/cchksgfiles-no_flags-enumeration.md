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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: dbe4cedf2011a1607a6db55dc064bd42dc229123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759810"
---
# <a name="cchksgfilesnoflags-enumeration"></a><span data-ttu-id="67248-103">CChkSGFiles.NO_FLAGS 列挙型</span><span class="sxs-lookup"><span data-stu-id="67248-103">CChkSGFiles.NO_FLAGS enumeration</span></span>

<span data-ttu-id="67248-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="67248-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="67248-105">**CCheckSGFiles**クラスのほとんどの関数で受け入れられる**ulFlags**パラメーターのプレース ホルダーの値として使用されます。</span><span class="sxs-lookup"><span data-stu-id="67248-105">Serves as a placeholder value for the **ulFlags** parameters that are accepted by most **CCheckSGFiles** class functions.</span></span> 
  
```cs
Enum { NO_FLAGS = 0 }

```

## <a name="requirements"></a><span data-ttu-id="67248-106">必要条件</span><span class="sxs-lookup"><span data-stu-id="67248-106">Requirements</span></span>

<span data-ttu-id="67248-107">Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="67248-107">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="67248-108">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="67248-108">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

