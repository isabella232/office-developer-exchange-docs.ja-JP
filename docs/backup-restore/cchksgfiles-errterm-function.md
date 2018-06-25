---
title: CChkSGFiles.ErrTerm 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: '最終更新日: 2013 年 2 月 25 日'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758866"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="182fe-103">CChkSGFiles.ErrTerm 関数</span><span class="sxs-lookup"><span data-stu-id="182fe-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="182fe-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="182fe-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="182fe-105">すべてのデータベース ページとログが正常に検証されたかどうかを示す、データベースとログの検証の全体的な状態を提供します。</span><span class="sxs-lookup"><span data-stu-id="182fe-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="182fe-106">ストレージ ・ グループは利用可能な Exchange 2013 です。</span><span class="sxs-lookup"><span data-stu-id="182fe-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="182fe-107">CHKSGFILES API では、データベースと Exchange Server 2010 より前のバージョンの Exchange ストレージ ・ グループの下位互換性のため、ストレージ ・ グループを指定できます。</span><span class="sxs-lookup"><span data-stu-id="182fe-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="182fe-108">Exchange 2013 のデータベースに対して CHKSGFILES を実行するときは、空の文字列にストレージ ・ グループの識別子を指定するパラメーターを設定してください。</span><span class="sxs-lookup"><span data-stu-id="182fe-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="182fe-109">Parameters</span><span class="sxs-lookup"><span data-stu-id="182fe-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="182fe-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="182fe-110">ulFlags</span></span>
  
<span data-ttu-id="182fe-p102">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="182fe-p102">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="182fe-114">�߂�l</span><span class="sxs-lookup"><span data-stu-id="182fe-114">Return value</span></span>

<span data-ttu-id="182fe-115">[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="182fe-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="182fe-116">備考</span><span class="sxs-lookup"><span data-stu-id="182fe-116">Remarks</span></span>

<span data-ttu-id="182fe-117">**CChkSGFiles**オブジェクトは、 **ErrInit**関数を使用して登録されているすべてのデータベースが実際にチェック アウトするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="182fe-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="182fe-118">このオブジェクト関数を使用して、 **ErrCheckDbPages**のことを確認するのには、 **ErrCheckDbHeaders**関数で指定されたページが実際にいることを確認するデータベースの数が同じです。</span><span class="sxs-lookup"><span data-stu-id="182fe-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="182fe-119">正しい数の各データベース内のページが正常にチェックされていない場合、 **ErrTerm**関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="182fe-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="182fe-120">**ErrCheckDbPages**でチェックするデータベース ページの数が**ErrCheckDbHeaders**で示されるよりも短い場合は、この関数は、Windows イベント ログに、エラーを作成し、 **ErrTerm**には、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="182fe-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="182fe-121">**ErrCheckDbPages**でチェックするデータベース ページの数が**ErrCheckDbHeaders**で示されるよりも大きい場合は、この関数は、アプリケーションが不必要をチェックするいくつかを示すために Windows イベント ログに警告を作成します。データベースのページが 2 回以上。</span><span class="sxs-lookup"><span data-stu-id="182fe-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="182fe-122">この場合、ただし、 **ErrTerm**関数は成功します。</span><span class="sxs-lookup"><span data-stu-id="182fe-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="182fe-123">**CChkSGFiles**オブジェクトは、 **ErrInit**に登録されているログ ファイルが実際にチェック アウトするかどうかも決定します。</span><span class="sxs-lookup"><span data-stu-id="182fe-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="182fe-124">表示しない場合は、すべてのログが正常にチェック、 **ErrTerm**関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="182fe-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="182fe-125">**ErrTerm**にエラーが返されるときも、 **ErrInit**に登録されているすべてのデータベースの検証の状態をチェックすることが見つかると、最初のエラーになります。</span><span class="sxs-lookup"><span data-stu-id="182fe-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="182fe-126">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、シングル スレッド アプリケーションの部分に、 **ErrTerm**関数を呼び出す必要があり、呼び出すことができます 1 回の**CCheckSGFiles**オブジェクトごとに。</span><span class="sxs-lookup"><span data-stu-id="182fe-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="182fe-127">必要条件</span><span class="sxs-lookup"><span data-stu-id="182fe-127">Requirements</span></span>

<span data-ttu-id="182fe-128">Exchange 2013 には、CHKSGFILES の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="182fe-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="182fe-129">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="182fe-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

