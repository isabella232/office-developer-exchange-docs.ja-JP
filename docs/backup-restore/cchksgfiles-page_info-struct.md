---
title: CChkSGFiles.PAGE_INFO 構造体
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759801"
---
# <a name="cchksgfilespageinfo-struct"></a><span data-ttu-id="8e711-103">CChkSGFiles.PAGE_INFO 構造体</span><span class="sxs-lookup"><span data-stu-id="8e711-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="8e711-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8e711-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="8e711-105">Exchange データベース ページの情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="8e711-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="8e711-106">この構造体は、 **ErrCheckDbPages**関数で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8e711-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a><span data-ttu-id="8e711-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8e711-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="8e711-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="8e711-108">ulPgNo</span></span>
  
<span data-ttu-id="8e711-109">Unsigned Long です。</span><span class="sxs-lookup"><span data-stu-id="8e711-109">Unsigned Long.</span></span> <span data-ttu-id="8e711-110">チェックするデータベースのページの論理ページ数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="8e711-111">**ErrCheckDbPages**を呼び出す前にこの値を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e711-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="8e711-112">アプリケーション、ファイル ・ オフセットに基づいてファイルを読み込み、そのためこれらのファイルのオフセットを論理ページ番号に対応する必要がありますに役立つ**PgnoFromFileOffset**メソッドにこのフィールドの値を決定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="8e711-113">**ErrCheckDbPages**では、この値は変更されません。</span><span class="sxs-lookup"><span data-stu-id="8e711-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="8e711-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="8e711-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="8e711-115">ブール値です。</span><span class="sxs-lookup"><span data-stu-id="8e711-115">Boolean.</span></span> <span data-ttu-id="8e711-116">TRUE の値は、データベースのページにデータが含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e711-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="8e711-117">FALSE の値は、ページにのみゼロが含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e711-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="8e711-118">**ErrCheckDbPages**は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="8e711-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="8e711-119">fCorrectableError</span></span>
  
<span data-ttu-id="8e711-120">ブール値です。</span><span class="sxs-lookup"><span data-stu-id="8e711-120">Boolean.</span></span> <span data-ttu-id="8e711-121">TRUE の値は、データベース ページにチェックサムの不一致が発生しましたが、修正可能なエラーであることを示します。</span><span class="sxs-lookup"><span data-stu-id="8e711-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="8e711-122">**ErrCheckDbPages**は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="8e711-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="8e711-123">checksumActual</span></span>
  
<span data-ttu-id="8e711-124">64 ビットの符号なし整数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8e711-125">この論理ページのデータベースに格納されているチェックサム値を示します。</span><span class="sxs-lookup"><span data-stu-id="8e711-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="8e711-126">**ErrCheckDbPages**は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="8e711-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="8e711-127">checksumExpected</span></span>
  
<span data-ttu-id="8e711-128">64 ビットの符号なし整数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8e711-129">これは、データベース ページに対して計算されたチェックサムの予想値**ErrCheckDbPages**で設定されています。</span><span class="sxs-lookup"><span data-stu-id="8e711-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="8e711-130">この値は、データベースのページに格納されている場合と異なるかどうか (つまり、値が返されます**checksumActual**で)、 **ErrCheckDbPages**はこのデータベースのページでエラーが検出されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="8e711-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="8e711-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="8e711-131">dbTime</span></span>
  
<span data-ttu-id="8e711-132">64 ビットの符号なし整数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8e711-133">**ErrCheckDbPages**では、データベース ページのタイムスタンプにこのメンバーを設定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="8e711-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="8e711-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="8e711-135">64 bt の符号なし整数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="8e711-136">**ErrCheckDbPages**は、このメンバーを計算されたチェックサムの値は、論理ページの等価性を決定する際に、必要なデータを除外するページの内容に設定します。</span><span class="sxs-lookup"><span data-stu-id="8e711-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="8e711-137">たとえば、使用されていないデータベース ページの領域のデータの値を考慮する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="8e711-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="8e711-138">このメンバーは、 **checksumActual**および**checksumExpected**の値は互いに等しい場合に有効なだけです。</span><span class="sxs-lookup"><span data-stu-id="8e711-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="8e711-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="8e711-139">ulFlags</span></span>
  
<span data-ttu-id="8e711-140">64 ビットの符号なし整数です。</span><span class="sxs-lookup"><span data-stu-id="8e711-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8e711-141">将来の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="8e711-141">Reserved for future use.</span></span> <span data-ttu-id="8e711-142">このフィールドの値は、 **ErrCheckDbPages**を呼び出す前に 0 (ゼロ) に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e711-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8e711-143">備考</span><span class="sxs-lookup"><span data-stu-id="8e711-143">Remarks</span></span>

<span data-ttu-id="8e711-144">**RgPageInfo**パラメーターの配列では、 **ErrCheckDbPages**関数を呼び出すときに**ページ\_情報**の構造体です。</span><span class="sxs-lookup"><span data-stu-id="8e711-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="8e711-145">必要がありますいずれかの**ページ\_情報**をチェックするには、各データベース ページの構造体です。</span><span class="sxs-lookup"><span data-stu-id="8e711-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="8e711-146">アプリケーションは、適切な値に**ulPgno**のメンバーを設定する必要があり、0 (ゼロ) に**ErrCheckDbPages**を呼び出す前に**ulFlags**メンバーを設定する必要がありますも。</span><span class="sxs-lookup"><span data-stu-id="8e711-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="8e711-147">必要条件</span><span class="sxs-lookup"><span data-stu-id="8e711-147">Requirements</span></span>

<span data-ttu-id="8e711-148">Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8e711-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="8e711-149">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e711-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

