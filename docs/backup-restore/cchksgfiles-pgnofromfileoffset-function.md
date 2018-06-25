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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758869"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="6afde-103">CChkSGFiles.PgnoFromFileOffset 関数</span><span class="sxs-lookup"><span data-stu-id="6afde-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="6afde-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6afde-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="6afde-105">物理データベース ・ ファイルで指定したバイトのインデックスを作成するには、対応するデータベースの論理ページ番号を返します。</span><span class="sxs-lookup"><span data-stu-id="6afde-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="6afde-106">ファイル オフセットが正しくない場合、またはデータベースの**ErrCheckDbHeaders**関数が呼び出されていない場合は、この関数は 0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="6afde-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="6afde-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="6afde-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="6afde-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="6afde-108">ibFileOffset</span></span>
  
<span data-ttu-id="6afde-p102">入力パラメーター。データベース ファイル内のオフセット (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="6afde-p102">Input parameter. The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="6afde-111">�߂�l</span><span class="sxs-lookup"><span data-stu-id="6afde-111">Return value</span></span>

<span data-ttu-id="6afde-112">指定したオフセットを含んでいるデータベース ファイルの論理ページ番号。</span><span class="sxs-lookup"><span data-stu-id="6afde-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6afde-113">備考</span><span class="sxs-lookup"><span data-stu-id="6afde-113">Remarks</span></span>

<span data-ttu-id="6afde-114">**IbFileOffset**パラメーターが有効でない場合、 **PgnoFromFileOffset**関数は、0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="6afde-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="6afde-115">**PgnoFromFileOffset**は、 **CCheckSGFiles**インスタンス上で、 **ErrCheckDbHeaders**関数を呼び出していない場合にも 0 (ゼロ) を返します。</span><span class="sxs-lookup"><span data-stu-id="6afde-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="6afde-116">データベース ヘッダーに割り当てられたページの数、データベースのページ サイズを初期化するために**ErrCheckDbHeaders**を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="6afde-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="6afde-117">入力するのには**PgnoFromFileOffset**を使用する必要があります、**ページ\_情報** **ErrCheckDbPages**を呼び出すための準備としての要素を構造化します。</span><span class="sxs-lookup"><span data-stu-id="6afde-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="6afde-118">**ErrCheckDbPages**に**rgPageInfo**パラメーターでは、配列の各要素が**ulPgno**メンバーの値が正しく初期化されると、 **PAGE_INFO**構造体である必要があります。</span><span class="sxs-lookup"><span data-stu-id="6afde-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="6afde-119">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **PgnoFromFileOffset**関数を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="6afde-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="6afde-120">通常この関数を複数回呼び出すデータベースごとにチェックされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6afde-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="6afde-121">必要条件</span><span class="sxs-lookup"><span data-stu-id="6afde-121">Requirements</span></span>

<span data-ttu-id="6afde-122">Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="6afde-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="6afde-123">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="6afde-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

