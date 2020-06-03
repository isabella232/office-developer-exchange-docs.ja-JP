---
title: CChkSGFiles.PgnoFromFileOffset 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452896"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="77aa8-103">CChkSGFiles.PgnoFromFileOffset 関数</span><span class="sxs-lookup"><span data-stu-id="77aa8-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="77aa8-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="77aa8-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="77aa8-105">物理データベース ファイルで指定したバイト インデックスに対応するデータベースの論理ページ番号を返します。</span><span class="sxs-lookup"><span data-stu-id="77aa8-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="77aa8-106">ファイル オフセットが無効な場合、またはデータベースに対する **ErrCheckDbHeaders** 関数の呼び出しが行われていない場合、この関数は 0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="77aa8-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="77aa8-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="77aa8-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="77aa8-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="77aa8-108">ibFileOffset</span></span>
  
<span data-ttu-id="77aa8-109">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="77aa8-109">Input parameter.</span></span> <span data-ttu-id="77aa8-110">データベース ファイル内のオフセット (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="77aa8-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="77aa8-111">戻り値</span><span class="sxs-lookup"><span data-stu-id="77aa8-111">Return value</span></span>

<span data-ttu-id="77aa8-112">指定したオフセットを含んでいるデータベース ファイルの論理ページ番号。</span><span class="sxs-lookup"><span data-stu-id="77aa8-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="77aa8-113">注釈</span><span class="sxs-lookup"><span data-stu-id="77aa8-113">Remarks</span></span>

<span data-ttu-id="77aa8-114">**ibFileOffset** パラメーターが無効な場合、**PgnoFromFileOffset** 関数は 0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="77aa8-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="77aa8-115">また、**CCheckSGFiles** インスタンスの **ErrCheckDbHeaders** 関数を呼び出していない場合も、**PgnoFromFileOffset** 関数は 0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="77aa8-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="77aa8-116">**ErrCheckDbHeaders** を呼び出すことで、データベース ヘッダーに割り当てられたデータベースのページ サイズとページ数を初期化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77aa8-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="77aa8-117">**Errcheckdbpages**を呼び出すための準備として、 **Pgnofromfileoffset**を使用して**ページ \_ 情報**構造の要素に入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="77aa8-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="77aa8-118">**ErrCheckDbPages** への **rgPageInfo** パラメーターは、配列内の各要素が **PAGE_INFO** 構造体であることと、**ulPgno** メンバーの値が正しく初期化されていることを必要とします。</span><span class="sxs-lookup"><span data-stu-id="77aa8-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="77aa8-119">マルチスレッド アプリケーションで CHKSGFILES を使用している場合、**PgnoFromFileOffset** 関数は、そのアプリケーションのシングルスレッドの部分で呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="77aa8-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="77aa8-120">通常、この関数は確認するデータベースごとに複数回呼び出すことになります。</span><span class="sxs-lookup"><span data-stu-id="77aa8-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="77aa8-121">Requirements</span><span class="sxs-lookup"><span data-stu-id="77aa8-121">Requirements</span></span>

<span data-ttu-id="77aa8-122">Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="77aa8-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="77aa8-123">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="77aa8-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

