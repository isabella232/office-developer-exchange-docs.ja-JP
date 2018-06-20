---
title: CChkSGFiles.ErrCheckDbPages 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758861"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="d884f-103">CChkSGFiles.ErrCheckDbPages 関数</span><span class="sxs-lookup"><span data-stu-id="d884f-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="d884f-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="d884f-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="d884f-105">指定したデータベースのページの範囲を検証します。 </span><span class="sxs-lookup"><span data-stu-id="d884f-105">Validates a range of pages in a specified database.</span></span> 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="d884f-106">Parameters</span><span class="sxs-lookup"><span data-stu-id="d884f-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="d884f-107">iDb</span><span class="sxs-lookup"><span data-stu-id="d884f-107">iDb</span></span>
  
<span data-ttu-id="d884f-108">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="d884f-108">Input parameter.</span></span> <span data-ttu-id="d884f-109">**ErrInit**関数に**rgwszDb の**パラメーターで指定されたデータベースの配列へのインデックスです。</span><span class="sxs-lookup"><span data-stu-id="d884f-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="d884f-110">このパラメーターでインデックス付けされたデータベースがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="d884f-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="d884f-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="d884f-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="d884f-112">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="d884f-112">Input parameter.</span></span> <span data-ttu-id="d884f-113">チェックする 1 つまたは複数のデータベース ページを格納するバッファーへのポインター。</span><span class="sxs-lookup"><span data-stu-id="d884f-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="d884f-114">バッファーのサイズは、 **ErrCheckDbHeaders**関数によって、 **pcbDbPageSize**パラメーターで返されると、データベースのページ サイズの倍数にすることがあります。</span><span class="sxs-lookup"><span data-stu-id="d884f-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="d884f-115">呼び出し元のアプリケーションは、 **ErrCheckDbPages**を呼び出す前にデータベース ページの内容をバッファーに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="d884f-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="d884f-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="d884f-116">cbPageBuffer</span></span>
  
<span data-ttu-id="d884f-117">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="d884f-117">Input parameter.</span></span> <span data-ttu-id="d884f-118">**PvPageBuffer**パラメーターのバイト単位のサイズです。</span><span class="sxs-lookup"><span data-stu-id="d884f-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="d884f-119">この値は、 **ErrCheckDbHeaders**関数によって、 **pcbDbPageSize**パラメーターで返されると、データベースのページ サイズの倍数にすることがあります。</span><span class="sxs-lookup"><span data-stu-id="d884f-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="d884f-120">rgPageInfo</span><span class="sxs-lookup"><span data-stu-id="d884f-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="d884f-121">入力/出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="d884f-121">Input/output parameter.</span></span> <span data-ttu-id="d884f-122">配列の**ページ\_情報**構造体の**ErrCheckDbPages**が、チェックされている各データベース ・ ページの結果を詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="d884f-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="d884f-123">配列の各**ulPgno**フィールドと、 **pvPageBuffer**パラメーターで渡された各データベース ・ ページの要素が 1 つ必要があります**ページ\_情報**構造は、データベースのページに対応する論理ページ番号を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d884f-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="d884f-124">詳細については、このトピックの後半の「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d884f-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="d884f-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="d884f-125">cPageInfo</span></span>
  
<span data-ttu-id="d884f-126">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="d884f-126">Input parameter.</span></span> <span data-ttu-id="d884f-127">**RgPageInfo**配列内のエントリの数です。</span><span class="sxs-lookup"><span data-stu-id="d884f-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="d884f-128">この値は、 **pvPageBuffer**パラメーターで渡されたデータベース ・ ページの数と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d884f-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="d884f-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="d884f-129">ulFlags</span></span> 
  
<span data-ttu-id="d884f-p106">オプションの入力パラメーター。この値は、将来使用するために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="d884f-p106">Optional input parameter. This value is reserved for future use. The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="d884f-133">�߂�l</span><span class="sxs-lookup"><span data-stu-id="d884f-133">Return value</span></span>

<span data-ttu-id="d884f-134">[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="d884f-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d884f-135">備考</span><span class="sxs-lookup"><span data-stu-id="d884f-135">Remarks</span></span>

<span data-ttu-id="d884f-136">データベースのデータベースは、 **ErrInit**関数に渡される配列に指定する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d884f-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="d884f-137">また、 **ErrCheckDbHeaders**を**ErrCheckDbPages**する前に呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="d884f-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="d884f-p108">呼び出し元のアプリケーションでは、確認対象のデータベース ページを保持できる大きさのメモリ バッファーを割り当てる必要があります。アプリケーションでは、このバッファーに、1 つ以上の該当するデータベース ページのコンテンツを設定する必要があります。 </span><span class="sxs-lookup"><span data-stu-id="d884f-p108">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked. The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="d884f-140">呼び出し元のアプリケーションでは、 **ErrCheckDbPages**を呼び出す前に**ErrCheckDbHeaders**を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="d884f-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="d884f-141">確認されるすべてのデータベース ファイル内のすべてのページをカバーするために必要な回数だけこの関数を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="d884f-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="d884f-142">**RgPageInfo**のパラメーターに返される各要素にで [データベース] ページについての情報が含まれています、**ページ\_情報**構造体です。</span><span class="sxs-lookup"><span data-stu-id="d884f-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="d884f-143">アプリケーションをそれぞれ確認する**ErrCheckDbPages**関数がエラーを返した場合は、**ページ\_情報**ページで、エラーが検出されましたを決定します。</span><span class="sxs-lookup"><span data-stu-id="d884f-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="d884f-144">たとえば、 **checksumActual**および**checksumExpected**の値を比較するには、そのデータベース ページのチェックサム エラーが検出されたかどうか示されます。</span><span class="sxs-lookup"><span data-stu-id="d884f-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="d884f-145">**ErrCheckDbPages**がデータベースの内容のすべてのエラーを検出すると、Windows のエラーのイベント ログ エントリを作成します。</span><span class="sxs-lookup"><span data-stu-id="d884f-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="d884f-146">**CChkSGFiles**オブジェクトは、 **ErrInit**関数を使用して登録されているすべてのデータベースが実際にチェック アウトするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d884f-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="d884f-147">具体的には、 **CChkSGFiles**では、 **ErrCheckDbPages**関数を使用して、 **ErrCheckDbHeaders**で指定されたデータベース ・ ページ数が同じが実際に検証されたかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="d884f-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="d884f-148">正しい数の各データベース内のページが正常にチェックしない場合、 **ErrTerm**関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="d884f-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="d884f-149">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **ErrCheckDbPages**関数を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="d884f-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="d884f-150">**ErrCheckDbPages**は、通常という名前の複数回チェックされているデータベースごとに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d884f-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="d884f-151">必要条件</span><span class="sxs-lookup"><span data-stu-id="d884f-151">Requirements</span></span>

<span data-ttu-id="d884f-152">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d884f-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="d884f-153">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="d884f-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

