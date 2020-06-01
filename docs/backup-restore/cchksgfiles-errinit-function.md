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
description: '最終更新日: 2013 年3月3日'
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457012"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="7dae3-103">CChkSGFiles.ErrInit 関数</span><span class="sxs-lookup"><span data-stu-id="7dae3-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="7dae3-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="7dae3-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="7dae3-105">確認するデータベース、およびトランザクション ログ ファイルのパスとベース名を指定することで **CChkSGFiles** オブジェクトを初期化します。</span><span class="sxs-lookup"><span data-stu-id="7dae3-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="7dae3-106">アプリケーションでは、**New** 関数の呼び出しが成功した直後に、この関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="7dae3-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7dae3-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="7dae3-108">rgwszDb[]</span><span class="sxs-lookup"><span data-stu-id="7dae3-108">rgwszDb[]</span></span>
  
<span data-ttu-id="7dae3-p102">入力パラメーター。確認するデータベースを指定する配列。各配列要素には、確認するデータベースのパスとファイル名を NULL で終了する Unicode 文字列で格納します。</span><span class="sxs-lookup"><span data-stu-id="7dae3-p102">Input parameter. An array that specifies the databases to be checked. Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="7dae3-112">cDB</span><span class="sxs-lookup"><span data-stu-id="7dae3-112">cDB</span></span>
  
<span data-ttu-id="7dae3-113">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="7dae3-113">Input parameter.</span></span> <span data-ttu-id="7dae3-114">**rgwszDb** 配列に含まれる有効なデータベース パスの要素数。</span><span class="sxs-lookup"><span data-stu-id="7dae3-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="7dae3-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="7dae3-115">wszLogPath</span></span>
  
<span data-ttu-id="7dae3-116">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="7dae3-116">Input parameter.</span></span> <span data-ttu-id="7dae3-117">確認するトランザクション ログ ファイルのフルパス (NULL で終了する Unicode 文字列の形式)。</span><span class="sxs-lookup"><span data-stu-id="7dae3-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="7dae3-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="7dae3-118">wszBaseName</span></span>
  
<span data-ttu-id="7dae3-119">入力パラメーター。</span><span class="sxs-lookup"><span data-stu-id="7dae3-119">Input parameter.</span></span> <span data-ttu-id="7dae3-120">Exchange トランザクション ログ ファイルの 3 文字のベース名 (NULL で終了する Unicode 文字列の形式)。</span><span class="sxs-lookup"><span data-stu-id="7dae3-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="7dae3-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="7dae3-121">ulFlags</span></span>
  
<span data-ttu-id="7dae3-p106">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-p106">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="7dae3-125">戻り値</span><span class="sxs-lookup"><span data-stu-id="7dae3-125">Return value</span></span>

<span data-ttu-id="7dae3-126">[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="7dae3-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7dae3-127">注釈</span><span class="sxs-lookup"><span data-stu-id="7dae3-127">Remarks</span></span>

<span data-ttu-id="7dae3-128">**ErrInit** 関数により、確認するデータベースとログ ファイルを登録します。</span><span class="sxs-lookup"><span data-stu-id="7dae3-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="7dae3-129">この関数は、**New** 関数が呼び出された直後に呼び出す必要があり、その後で、それ以外の **ChkSGFiles** 関数を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="7dae3-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="7dae3-130">すべてのデータベースの名前、ログ ファイルのパス、およびベース名を NULL で終了する Unicode 文字列で指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="7dae3-131">データベースファイルのみ、ログファイルのみ、またはデータベースファイルとログファイルの両方をチェックできます。</span><span class="sxs-lookup"><span data-stu-id="7dae3-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="7dae3-132">ただし、この関数を呼び出す場合は、少なくとも1つのエンティティをチェックするようにアプリケーションを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="7dae3-133">**WszLogPath**では、 **cDB**に 0 (ゼロ) を渡すと NULL が返され、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="7dae3-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="7dae3-134">**CDB**の値が 0 (ゼロ) 以外の場合、 **rgwszDb**に NULL を渡すと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="7dae3-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="7dae3-135">データベース ファイルを確認する場合、アプリケーションではデータベース名を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="7dae3-136">**WszBaseName**に null が渡されても、 **wszLogPath**が null でない場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="7dae3-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="7dae3-137">ログ ファイルを確認する場合は、必ずログ ファイルのベース名が必要になります。</span><span class="sxs-lookup"><span data-stu-id="7dae3-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="7dae3-138">マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **ErrInit** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。 </span><span class="sxs-lookup"><span data-stu-id="7dae3-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="7dae3-139">Requirements</span><span class="sxs-lookup"><span data-stu-id="7dae3-139">Requirements</span></span>

<span data-ttu-id="7dae3-140">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7dae3-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="7dae3-141">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dae3-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

