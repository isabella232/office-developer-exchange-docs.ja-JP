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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526726"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="9d68c-103">CChkSGFiles.ErrCheckDbPages 関数</span><span class="sxs-lookup"><span data-stu-id="9d68c-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="9d68c-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9d68c-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="9d68c-105">指定したデータベースのページの範囲を検証します。</span><span class="sxs-lookup"><span data-stu-id="9d68c-105">Validates a range of pages in a specified database.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="9d68c-106">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d68c-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="9d68c-107">.Idb</span><span class="sxs-lookup"><span data-stu-id="9d68c-107">iDb</span></span>
  
<span data-ttu-id="9d68c-108">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="9d68c-108">Input parameter.</span></span> <span data-ttu-id="9d68c-109">**ErrInit** 関数への **rgwszDb[]** パラメーターで指定したデータベースの配列のインデックス。</span><span class="sxs-lookup"><span data-stu-id="9d68c-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="9d68c-110">このパラメーターでインデックス指定されたデータベースが確認の対象になります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="9d68c-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="9d68c-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="9d68c-112">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="9d68c-112">Input parameter.</span></span> <span data-ttu-id="9d68c-113">確認対象のデータベース ページを 1 ページ以上格納しているバッファーへのポインター。</span><span class="sxs-lookup"><span data-stu-id="9d68c-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="9d68c-114">バッファーのサイズは、**ErrCheckDbHeaders** 関数の **pcbDbPageSize** パラメーターで返されるデータベース ページのサイズの倍数になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="9d68c-115">呼び出し元のアプリケーションでは、**ErrCheckDbPages** を呼び出す前に、データベース ページのコンテンツでバッファーを満たしておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="9d68c-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="9d68c-116">cbPageBuffer</span></span>
  
<span data-ttu-id="9d68c-117">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="9d68c-117">Input parameter.</span></span> <span data-ttu-id="9d68c-118">**pvPageBuffer** パラメーターのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="9d68c-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="9d68c-119">この値は、**ErrCheckDbHeaders** 関数の **pcbDbPageSize** パラメーターで返されるデータベース ページのサイズの倍数になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="9d68c-120">rgPageInfo[]</span><span class="sxs-lookup"><span data-stu-id="9d68c-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="9d68c-121">入力/出力パラメータ。</span><span class="sxs-lookup"><span data-stu-id="9d68c-121">Input/output parameter.</span></span> <span data-ttu-id="9d68c-122">入力された各データベースページの詳細結果を、 **Errcheckdbpages**が設定した**ページ \_ 情報**構造の配列です。</span><span class="sxs-lookup"><span data-stu-id="9d68c-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="9d68c-123">配列には、 **pvPageBuffer**パラメーターで渡されたデータベースページごとに1つの要素が必要で、各**ページ \_ 情報**構造の**ulpgno**フィールドは、データベースページに対応する論理ページ番号に設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="9d68c-124">詳細については、このトピックで後述する「解説」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d68c-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="9d68c-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="9d68c-125">cPageInfo</span></span>
  
<span data-ttu-id="9d68c-p105">入力パラメーター。**rgPageInfo[]** 配列のエントリ数。この値は、**pvPageBuffer** パラメーターで渡したデータベース ページの数と等しくなっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-p105">Input parameter. The number of entries in the **rgPageInfo[]** array. This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="9d68c-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="9d68c-129">ulFlags</span></span> 
  
<span data-ttu-id="9d68c-p106">オプションの入力パラメーター。この値は、将来使用するために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-p106">Optional input parameter. This value is reserved for future use. The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="9d68c-133">戻り値</span><span class="sxs-lookup"><span data-stu-id="9d68c-133">Return value</span></span>

<span data-ttu-id="9d68c-134">[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="9d68c-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d68c-135">注釈</span><span class="sxs-lookup"><span data-stu-id="9d68c-135">Remarks</span></span>

<span data-ttu-id="9d68c-136">指定するデータベースは、**ErrInit** 関数に渡したデータベースの配列内のものにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="9d68c-137">また、**ErrCheckDbPages** の前に **ErrCheckDbHeaders** を呼び出す必要もあります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="9d68c-p108">呼び出し元のアプリケーションでは、確認対象のデータベース ページを保持できる大きさのメモリ バッファーを割り当てる必要があります。アプリケーションでは、このバッファーに、1 つ以上の該当するデータベース ページのコンテンツを設定する必要があります。 </span><span class="sxs-lookup"><span data-stu-id="9d68c-p108">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked. The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="9d68c-140">呼び出し元アプリケーションは、 **Errcheckdbheaders**を呼び出す前に、 **Errcheckdbheaders**を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="9d68c-141">この関数は、すべてのデータベース ファイルに含まれる確認対象のすべてのページをカバーするために必要になる回数だけ呼び出しできます。</span><span class="sxs-lookup"><span data-stu-id="9d68c-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="9d68c-142">**RgPageInfo []** パラメーターでは、返される各要素には、**ページ \_ 情報**構造内のデータベースページに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d68c-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="9d68c-143">**Errcheckdbpages**関数がエラーを返した場合、アプリケーションは各**ページ \_ 情報**構造をチェックして、エラーが検出されたページを特定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="9d68c-144">たとえば、**checksumActual** と **checksumExpected** の値を比較することで、そのデータベース ページでチェックサム エラーが検出されたかどうかがわかります。</span><span class="sxs-lookup"><span data-stu-id="9d68c-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="9d68c-145">**ErrCheckDbPages** は、データベース コンテンツにエラーを検出すると、Windows エラーのイベント ログのエントリを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d68c-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="9d68c-146">**CChkSGFiles** オブジェクトは、**ErrInit** 関数に登録されているすべてのデータベースが実際にチェックされたかどうかを判別します。</span><span class="sxs-lookup"><span data-stu-id="9d68c-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="9d68c-147">具体的には、**CChkSGFiles** は **ErrCheckDbPages** 関数を使用することで、**ErrCheckDbHeaders** によって示されたデータベース ページ数が実際に検証されたページ数と同じかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="9d68c-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="9d68c-148">各データベースで適切なページ数が正常にチェックされていなかった場合、**ErrTerm** 関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="9d68c-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="9d68c-149">マルチスレッド アプリケーションで CHKSGFILES を使用している場合、**ErrCheckDbPages** 関数は、そのアプリケーションのシングルスレッドの部分で呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="9d68c-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="9d68c-150">通常、**ErrCheckDbPages** は確認対象のデータベースごとに複数回呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="9d68c-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="9d68c-151">Requirements</span><span class="sxs-lookup"><span data-stu-id="9d68c-151">Requirements</span></span>

<span data-ttu-id="9d68c-152">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d68c-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="9d68c-153">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d68c-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

