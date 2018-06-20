---
title: CChkSGFiles.ErrInit 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: '最終更新日: 2013 年 3 月 3 日'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758860"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="5e8e9-103">CChkSGFiles.ErrInit 関数</span><span class="sxs-lookup"><span data-stu-id="5e8e9-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="5e8e9-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5e8e9-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="5e8e9-105">チェックするデータベースを指定することによって**CChkSGFiles**オブジェクトのパスおよびチェックするトランザクション ログ ファイルの基本名を初期化します。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="5e8e9-106">アプリケーションでは、**新規**の関数の呼び出しに成功した直後にこの関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="5e8e9-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="5e8e9-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="5e8e9-108">rgwszDb</span><span class="sxs-lookup"><span data-stu-id="5e8e9-108">rgwszDb[]</span></span>
  
<span data-ttu-id="5e8e9-p102">入力パラメーター。確認するデータベースを指定する配列。各配列要素には、確認するデータベースのパスとファイル名を NULL で終了する Unicode 文字列で格納します。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-p102">Input parameter. An array that specifies the databases to be checked. Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="5e8e9-112">cDB</span><span class="sxs-lookup"><span data-stu-id="5e8e9-112">cDB</span></span>
  
<span data-ttu-id="5e8e9-113">パラメーターを入力します。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-113">Input parameter.</span></span> <span data-ttu-id="5e8e9-114">**RgwszDb**配列内の有効なデータベースのパスの要素の数。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="5e8e9-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="5e8e9-115">wszLogPath</span></span>
  
<span data-ttu-id="5e8e9-p104">入力パラメーター。確認するトランザクション ログ ファイルのフルパス (NULL で終了する Unicode 文字列の形式)。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-p104">Input parameter. The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="5e8e9-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="5e8e9-118">wszBaseName</span></span>
  
<span data-ttu-id="5e8e9-p105">入力パラメーター。Exchange トランザクション ログ ファイルの 3 文字のベース名 (NULL で終了する Unicode 文字列の形式)。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-p105">Input parameter. The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="5e8e9-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="5e8e9-121">ulFlags</span></span>
  
<span data-ttu-id="5e8e9-p106">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-p106">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="5e8e9-125">�߂�l</span><span class="sxs-lookup"><span data-stu-id="5e8e9-125">Return value</span></span>

<span data-ttu-id="5e8e9-126">[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5e8e9-127">備考</span><span class="sxs-lookup"><span data-stu-id="5e8e9-127">Remarks</span></span>

<span data-ttu-id="5e8e9-128">**ErrInit**関数は、データベースとログ ファイルをチェックするを登録します。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="5e8e9-129">**新規**の関数が呼び出されますが、他の**ChkSGFiles**する前に関数が呼び出される後、この関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="5e8e9-130">すべてのデータベースの名前、ログ ファイルのパス、およびベース名を NULL で終了する Unicode 文字列で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="5e8e9-131">データベース ・ ファイルのみをチェックすることができますのみ、ログ ファイル、またはデータベース ファイルとログ ファイルの両方。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="5e8e9-132">ただし、この関数を呼び出す場合アプリケーションはチェックするには、少なくとも 1 つのエンティティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="5e8e9-133">**WszLogPath**の**cDB**と NULL は 0 (ゼロ) を渡すと、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="5e8e9-134">**CDB**の値が 0 (ゼロ) 以外の場合は、 **rgwszDb**に NULL を渡すことと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="5e8e9-135">データベース ファイルをチェックするには、アプリケーションがデータベース名を入力してください。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="5e8e9-136">**WszBaseName**に NULL が渡される**wszLogPath**が NULL でない場合は、エラーが戻ります。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="5e8e9-137">ログ ファイルのベース名は、ログ ファイルをチェックするときに常に必要です。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="5e8e9-138">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、アプリケーションの単一の部分に、 **ErrInit**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="5e8e9-139">必要条件</span><span class="sxs-lookup"><span data-stu-id="5e8e9-139">Requirements</span></span>

<span data-ttu-id="5e8e9-140">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="5e8e9-141">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5e8e9-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

