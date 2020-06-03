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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456340"
---
# <a name="cchksgfilespage_info-struct"></a><span data-ttu-id="8482a-103">CChkSGFiles.PAGE_INFO 構造体</span><span class="sxs-lookup"><span data-stu-id="8482a-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="8482a-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8482a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="8482a-105">Exchange データベース ページに関する情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="8482a-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="8482a-106">この構造体は、**ErrCheckDbPages** 関数で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8482a-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
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

## <a name="members"></a><span data-ttu-id="8482a-107">Members</span><span class="sxs-lookup"><span data-stu-id="8482a-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="8482a-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="8482a-108">ulPgNo</span></span>
  
<span data-ttu-id="8482a-109">Unsigned Long。</span><span class="sxs-lookup"><span data-stu-id="8482a-109">Unsigned Long.</span></span> <span data-ttu-id="8482a-110">確認するデータベース ページの論理ページ番号。</span><span class="sxs-lookup"><span data-stu-id="8482a-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="8482a-111">この値は、**ErrCheckDbPages** を呼び出す前に設定しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8482a-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="8482a-112">アプリケーションがファイルのオフセットに基づいてファイルを読み取る場合は、該当するファイルのオフセットを論理ページ番号にマップする必要がありますが、**PgnoFromFileOffset** メソッドは、このフィールドの値の決定に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="8482a-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="8482a-113">**ErrCheckDbPages** は、この値を変更しません。</span><span class="sxs-lookup"><span data-stu-id="8482a-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="8482a-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="8482a-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="8482a-115">ブール.</span><span class="sxs-lookup"><span data-stu-id="8482a-115">Boolean.</span></span> <span data-ttu-id="8482a-116">TRUE の値は、データベース ページにデータが含まれていることを表します。</span><span class="sxs-lookup"><span data-stu-id="8482a-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="8482a-117">FALSE の値は、ページにゼロのみが含まれていることを表します。</span><span class="sxs-lookup"><span data-stu-id="8482a-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="8482a-118">**ErrCheckDbPages** は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8482a-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="8482a-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="8482a-119">fCorrectableError</span></span>
  
<span data-ttu-id="8482a-120">ブール.</span><span class="sxs-lookup"><span data-stu-id="8482a-120">Boolean.</span></span> <span data-ttu-id="8482a-121">TRUE の値は、データベース ページに修正可能なチェックサムの不一致が検出されたことを表します。</span><span class="sxs-lookup"><span data-stu-id="8482a-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="8482a-122">**ErrCheckDbPages** は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8482a-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="8482a-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="8482a-123">checksumActual</span></span>
  
<span data-ttu-id="8482a-124">64 ビット符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="8482a-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8482a-125">この論理ページのデータベースに格納されているチェックサム値を表します。</span><span class="sxs-lookup"><span data-stu-id="8482a-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="8482a-126">**ErrCheckDbPages** は、この値を設定します。</span><span class="sxs-lookup"><span data-stu-id="8482a-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="8482a-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="8482a-127">checksumExpected</span></span>
  
<span data-ttu-id="8482a-128">64 ビット符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="8482a-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8482a-129">これは、データベースページに対して計算された、予想されるチェックサム値です。これは、 **Errcheckdbpages**によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="8482a-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="8482a-130">この値がデータベースページに格納されている値と異なる場合 (つまり、 **checksumActual**で返される値)、 **Errcheckdbpages**は、このデータベースページでエラーが検出されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="8482a-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="8482a-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="8482a-131">dbTime</span></span>
  
<span data-ttu-id="8482a-132">64 ビット符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="8482a-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8482a-133">**ErrCheckDbPages** は、このメンバーをデータベース ページのタイムスタンプに設定します。</span><span class="sxs-lookup"><span data-stu-id="8482a-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="8482a-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="8482a-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="8482a-135">Unsigned 64-bt 整数。</span><span class="sxs-lookup"><span data-stu-id="8482a-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="8482a-136">**Errcheckdbpages**は、このメンバーをページのコンテンツの計算されたチェックサム値に設定します。データは、論理的なページの同等性を決定するときには必要ありません。</span><span class="sxs-lookup"><span data-stu-id="8482a-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="8482a-137">たとえば、使用されていないデータベースページ領域のデータ値を考慮する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="8482a-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="8482a-138">このメンバーは、 **checksumActual**と**checksumExpected**の値が互いに等しい場合にのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="8482a-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="8482a-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="8482a-139">ulFlags</span></span>
  
<span data-ttu-id="8482a-140">64 ビット符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="8482a-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="8482a-141">将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="8482a-141">Reserved for future use.</span></span> <span data-ttu-id="8482a-142">このフィールドの値は、**ErrCheckDbPages** を呼び出す前に 0 (ゼロ) に設定しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8482a-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8482a-143">注釈</span><span class="sxs-lookup"><span data-stu-id="8482a-143">Remarks</span></span>

<span data-ttu-id="8482a-144">**Errcheckdbpages**関数を呼び出すとき、 **RgPageInfo**パラメーターは**ページ \_ 情報**構造の配列です。</span><span class="sxs-lookup"><span data-stu-id="8482a-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="8482a-145">チェックするデータベースページごとに1つの**ページ \_ 情報**構造が必要です。</span><span class="sxs-lookup"><span data-stu-id="8482a-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="8482a-146">アプリケーションでは、Errcheckdbpages を呼び出す前に、 **Ulcheckdbpage**を呼び出す前に、パラメーターの値を**ulpgno**に設定する必要があります。また、 **ulflags**メンバーを 0 (ゼロ) に設定する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="8482a-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="8482a-147">Requirements</span><span class="sxs-lookup"><span data-stu-id="8482a-147">Requirements</span></span>

<span data-ttu-id="8482a-148">Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8482a-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="8482a-149">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="8482a-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

