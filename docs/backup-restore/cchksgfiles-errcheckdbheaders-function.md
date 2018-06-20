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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758868"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="93b3e-103">CChkSGFiles.ErrCheckDbHeaders 関数</span><span class="sxs-lookup"><span data-stu-id="93b3e-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="93b3e-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="93b3e-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="93b3e-105">**ErrInit**関数によって指定されているデータベース ファイルのヘッダーを検証します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="93b3e-106">この関数では、ページ サイズとページ数も、指定されたデータベースのそれぞれに返します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="93b3e-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="93b3e-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="93b3e-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="93b3e-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="93b3e-p102">出力パラメーター。指定されたデータベースごとのページ サイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="93b3e-p102">Output parameter. The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="93b3e-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="93b3e-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="93b3e-112">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="93b3e-112">Output parameter.</span></span> <span data-ttu-id="93b3e-113">それぞれの先頭ページの数は、内部で使用するデータベース エンジンによって予約されているデータベースを指定します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="93b3e-114">*検証のための**ErrCheckDbPages**関数をヘッダー ページをパス*する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="93b3e-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="93b3e-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="93b3e-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="93b3e-116">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="93b3e-116">Output parameter.</span></span> <span data-ttu-id="93b3e-117">関数の戻り値がエラーを示す場合、このパラメーターは、 **ErrInit**関数に渡される**rgwszDb の**配列へのインデックスを指定します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="93b3e-118">インデックス付きの配列要素は、エラーが検出されたデータベースを表します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="93b3e-119">関数がエラー値を返さない場合、このパラメーターの値は有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="93b3e-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="93b3e-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="93b3e-120">ulFlags</span></span> 
  
<span data-ttu-id="93b3e-p105">オプションの入力パラメーター。この値は、将来使用するために予約されています。渡された値は、0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="93b3e-p105">Optional input parameter. This value is reserved for future use. The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="93b3e-124">�߂�l</span><span class="sxs-lookup"><span data-stu-id="93b3e-124">Return value</span></span>

<span data-ttu-id="93b3e-125">この関数は、 [CChkSGFiles.ERR 列挙型](cchksgfiles-err-enumeration.md)のエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93b3e-126">備考</span><span class="sxs-lookup"><span data-stu-id="93b3e-126">Remarks</span></span>

<span data-ttu-id="93b3e-127">**ErrCheckDbHeaders**は、同じログとデータベースの署名ページのサイズを**ErrInit**に登録されているすべてのデータベースがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="93b3e-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="93b3e-128">クリーン シャット ダウン状態にするためのすべての登録されているデータベースに必要なログ ファイルのセットを決定するのには、 **genMin**パラメーターの値が最小と最大の**genMax**パラメーターの値を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="93b3e-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="93b3e-129">エラーが検出された場合にのみ、 **piDbErrorEncountered**パラメーターが設定されて、 **ErrCheckDbHeaders**の戻り値に 0 以外で示されるようにします。</span><span class="sxs-lookup"><span data-stu-id="93b3e-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="93b3e-130">この関数でエラーが発生すると、エラー イベントが Windows エラー イベント ログに追加されます。</span><span class="sxs-lookup"><span data-stu-id="93b3e-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="93b3e-131">**ErrInit**を呼び出した後にだけ、 **ErrCheckDbHeaders**を呼び出すことができますし、 **ErrCheckDbPages**と**ErrCheckLogs**を呼び出す前に呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="93b3e-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="93b3e-132">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、部分では、シングル スレッド、 **ErrCheckDbHeaders**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="93b3e-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="93b3e-133">必要条件</span><span class="sxs-lookup"><span data-stu-id="93b3e-133">Requirements</span></span>

<span data-ttu-id="93b3e-134">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="93b3e-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="93b3e-135">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="93b3e-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

