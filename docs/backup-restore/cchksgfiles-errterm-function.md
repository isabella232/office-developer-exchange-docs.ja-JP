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
description: '最終更新日: 2013 年2月25日'
ms.openlocfilehash: 12b07fba69054d327c7250bbf83e4c77016e8b3f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466200"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="8a870-103">CChkSGFiles.ErrTerm 関数</span><span class="sxs-lookup"><span data-stu-id="8a870-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="8a870-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8a870-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="8a870-105">すべてのデータベース ページとログが正常に検証されたかどうかを示す、データベースとログの検証の全体的な状態を提供します。</span><span class="sxs-lookup"><span data-stu-id="8a870-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="8a870-106">ストレージグループは、Exchange 2013 では使用できません。</span><span class="sxs-lookup"><span data-stu-id="8a870-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="8a870-107">Exchange Server 2010 より前のバージョンの Exchange でデータベースおよびストレージグループとの下位互換性を維持するために、CHKSGFILES API ではストレージグループを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="8a870-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="8a870-108">Exchange 2013 データベースに対して CHKSGFILES を実行するときは、ストレージグループ識別子を指定するパラメーターを空の文字列に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a870-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="8a870-109">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a870-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="8a870-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="8a870-110">ulFlags</span></span>
  
<span data-ttu-id="8a870-p102">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="8a870-p102">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="8a870-114">戻り値</span><span class="sxs-lookup"><span data-stu-id="8a870-114">Return value</span></span>

<span data-ttu-id="8a870-115">[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="8a870-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8a870-116">注釈</span><span class="sxs-lookup"><span data-stu-id="8a870-116">Remarks</span></span>

<span data-ttu-id="8a870-117">**CChkSGFiles** オブジェクトは、**ErrInit** 関数に登録されているすべてのデータベースが実際にチェックされたかどうかを判別します。</span><span class="sxs-lookup"><span data-stu-id="8a870-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="8a870-118">このオブジェクトは **ErrCheckDbPages** 関数を使って、**ErrCheckDbHeaders** 関数で示されているのと同じ数のデータベース ページが実際に検証されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="8a870-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="8a870-119">各データベースで適切な数のページが正常にチェックされていない場合、**ErrTerm** 関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="8a870-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="8a870-120">**ErrCheckDbPages** でチェックしたデータベース ページの数が **ErrCheckDbHeaders** で示されている数よりも少ない場合、この関数は Windows イベント ログにエラーを作成し、**ErrTerm** がエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="8a870-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="8a870-121">**ErrCheckDbPages** でチェックしたデータベース ページの数が **ErrCheckDbHeaders** で示されている数よりも多い場合、この関数は、アプリケーションが一部のデータベース ページを複数回にわたり不必要にチェックした可能性を示す警告を Windows イベント ログに作成します。</span><span class="sxs-lookup"><span data-stu-id="8a870-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="8a870-122">ただし、この場合には **ErrTerm** 関数は成功します。</span><span class="sxs-lookup"><span data-stu-id="8a870-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="8a870-123">また、**CChkSGFiles** オブジェクトは **ErrInit** に登録されたログ ファイルが実際にチェックされたかどうかを判別します。</span><span class="sxs-lookup"><span data-stu-id="8a870-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="8a870-124">正常にチェックされなかったログがあると、**ErrTerm** 関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="8a870-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="8a870-125">**ErrTerm** がエラーを返す場合、この関数は **ErrInit** に登録されているすべてのデータベースの検証状態をチェックしますが、このエラーが最初に検出されます。</span><span class="sxs-lookup"><span data-stu-id="8a870-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="8a870-126">マルチスレッドアプリケーションで CHKSGFILES を使用している場合は、アプリケーションの単一スレッドの部分で**Errterm**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに1回だけ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="8a870-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="8a870-127">Requirements</span><span class="sxs-lookup"><span data-stu-id="8a870-127">Requirements</span></span>

<span data-ttu-id="8a870-128">Exchange 2013 には、CHKSGFILES の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a870-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="8a870-129">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a870-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

