---
title: CChkSGFiles.ErrCheckDbHeaders 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455248"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="0dcd8-103">CChkSGFiles.ErrCheckDbHeaders 関数</span><span class="sxs-lookup"><span data-stu-id="0dcd8-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="0dcd8-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0dcd8-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="0dcd8-105">**ErrInit** 関数で指定されたデータベース ファイルのヘッダーを検証します。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="0dcd8-106">この関数は、指定されたデータベースごとのページ サイズとページ数も返します。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="0dcd8-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0dcd8-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="0dcd8-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="0dcd8-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="0dcd8-p102">出力パラメーター。指定されたデータベースごとのページ サイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-p102">Output parameter. The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="0dcd8-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="0dcd8-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="0dcd8-112">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-112">Output parameter.</span></span> <span data-ttu-id="0dcd8-113">データベースエンジンによって内部使用のために予約されている、指定された各データベースの最初のページ数。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="0dcd8-114">検証のために、ヘッダーページを**Errcheckdbpages**関数に渡さ*ない*ように注意してください。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="0dcd8-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="0dcd8-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="0dcd8-116">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-116">Output parameter.</span></span> <span data-ttu-id="0dcd8-117">関数の戻り値がエラーを示している場合、このパラメーターは **ErrInit** 関数に渡した **rgwszDb[]** 配列のインデックスになります。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="0dcd8-118">インデックスで示された配列の要素は、エラーが発生したデータベースを表します。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="0dcd8-119">関数がエラー値を返さない場合、このパラメーターの値は無効になります。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="0dcd8-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="0dcd8-120">ulFlags</span></span> 
  
<span data-ttu-id="0dcd8-p105">オプションの入力パラメーター。この値は、将来使用するために予約されています。渡された値は、0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-p105">Optional input parameter. This value is reserved for future use. The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="0dcd8-124">戻り値</span><span class="sxs-lookup"><span data-stu-id="0dcd8-124">Return value</span></span>

<span data-ttu-id="0dcd8-125">この関数は、 [CChkSGFiles 列挙](cchksgfiles-err-enumeration.md)からエラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0dcd8-126">注釈</span><span class="sxs-lookup"><span data-stu-id="0dcd8-126">Remarks</span></span>

<span data-ttu-id="0dcd8-127">**ErrCheckDbHeaders** は、**ErrInit** によって登録したすべてのデータベースで、ログ署名とデータベース ページ サイズが同じであることを検証します。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="0dcd8-128">また、最小の **genMin** パラメーター値と、最大の **genMax** パラメーター値を使用することで、登録されたすべてのデータベースをクリーン シャットダウン状態にするために必要になるログ ファイルのセットを決定することもできます。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="0dcd8-129">**piDbErrorEncountered** パラメーターは、ゼロ以外の **ErrCheckDbHeaders** の戻り値で示されるエラーが検出された場合にのみ設定されます。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="0dcd8-130">この関数でエラーが発生すると、エラー イベントが Windows エラー イベント ログに追加されます。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="0dcd8-131">**ErrCheckDbHeaders** は、**ErrInit** を呼び出した後にのみ呼び出せるようになり、**ErrCheckDbPages** および **ErrCheckLogs** を呼び出す前に呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="0dcd8-132">マルチスレッドアプリケーションで CHKSGFILES を使用している場合は、単一スレッドの部分で**Errcheckdbheaders**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに1回だけ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="0dcd8-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="0dcd8-133">Requirements</span></span>

<span data-ttu-id="0dcd8-134">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="0dcd8-135">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dcd8-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

