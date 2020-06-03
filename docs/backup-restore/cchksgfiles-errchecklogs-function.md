---
title: CChkSGFiles.ErrCheckLogs 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 71e21bb3a748a532f9e3167e0b36898acde71b02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526719"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="466e0-103">CChkSGFiles.ErrCheckLogs 関数</span><span class="sxs-lookup"><span data-stu-id="466e0-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="466e0-104">**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="466e0-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="466e0-105">**ErrInit** 関数で指定されたすべてのデータベース ファイルのログ ファイルを検証します。</span><span class="sxs-lookup"><span data-stu-id="466e0-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="466e0-106">検証済みログ ファイルは、**ErrInit** に渡されたパス内に存在し、3 文字のベース ログ ファイル名を持っているものです。</span><span class="sxs-lookup"><span data-stu-id="466e0-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="466e0-107">パラメーター</span><span class="sxs-lookup"><span data-stu-id="466e0-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="466e0-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="466e0-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="466e0-109">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="466e0-109">Output parameter.</span></span> <span data-ttu-id="466e0-110">**True**の場合、このパラメーターは、トランザクションログファイルにエラーが見つかったことを示しますが、データを失わずにデータベースをクリーンシャットダウン状態にするために必要ではないログファイルにこれらのエラーが含まれていました。</span><span class="sxs-lookup"><span data-stu-id="466e0-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="466e0-111">このパラメーターに返される**実際**の値は、 **Errchecklogs**が**errsuccess**を返す場合にのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="466e0-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="466e0-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="466e0-112">ulFlags</span></span>
  
<span data-ttu-id="466e0-p103">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="466e0-p103">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="466e0-116">戻り値</span><span class="sxs-lookup"><span data-stu-id="466e0-116">Return value</span></span>

<span data-ttu-id="466e0-117">[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="466e0-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="466e0-118">ログファイルでエラーが検出された場合でも、この関数は**Errsuccess**を返すことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="466e0-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="466e0-119">そのため、 **Errchecklogs**が**errsuccess**を返すと、アプリケーションは**pfOnlyUnnecessaryLogsCorrupt** return パラメーターも確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="466e0-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="466e0-120">**ErrCheckLogs** が **errSuccess** を返したときに、**pfOnlyUnnecessaryLogsCorrupts** が **true** の場合は、データベースを最新状態にする必要のないログ ファイルにのみ、1 つ以上のエラーが見つかったことを意味します。</span><span class="sxs-lookup"><span data-stu-id="466e0-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="466e0-121">注釈</span><span class="sxs-lookup"><span data-stu-id="466e0-121">Remarks</span></span>

<span data-ttu-id="466e0-122">**ErrCheckDbHeaders** 関数は、**ErrCheckLogs** 関数よりも先に呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="466e0-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="466e0-123">Exchange データベースのトランザクションログファイルがチェックされている場合、データを失わずにストレージグループ内のデータベースをクリーンシャットダウン状態にするために、一部のログファイルが必要になることがありますが、その他のログファイルは必要ない場合があります。</span><span class="sxs-lookup"><span data-stu-id="466e0-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="466e0-124">**Errchecklogs**関数は、データベースを最新の状態にするために必要な最古および最新のログファイルの両方を決定します。</span><span class="sxs-lookup"><span data-stu-id="466e0-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="466e0-125">**ErrCheckLogs** 関数は、**ErrInit** 関数に渡したものと同じに、指定したパス内にある指定した 3 文字のベース ファイル名を持つすべてのログ ファイルを検証します。</span><span class="sxs-lookup"><span data-stu-id="466e0-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="466e0-126">ログ ファイルにエラーが見つからない場合、**ErrCheckLogs** は **errSuccess** を返します。</span><span class="sxs-lookup"><span data-stu-id="466e0-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="466e0-127">必要とされるログ ファイルのいずれかに破損が見つかると、**ErrCheckLogs** はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="466e0-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="466e0-128">必要とされる最古のログ ファイルよりも古いログ ファイルにのみエラーが見つかった場合、この関数は **errSuccess** を返して、戻り値パラメーター **pfOnlyUnnecessaryLogCorrupt** を **true** に設定します。</span><span class="sxs-lookup"><span data-stu-id="466e0-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="466e0-129">アプリケーションでは、そうした古いログ ファイルの一部にエラーが存在することを認識する必要があり、該当する場合にはユーザーに警告するようにします。</span><span class="sxs-lookup"><span data-stu-id="466e0-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="466e0-130">いずれにしても、こうしたエラーがデータベースの全体的な整合性に影響することや、ログ フォワードの実行が成功するかどうかに影響することはありません。</span><span class="sxs-lookup"><span data-stu-id="466e0-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="466e0-131">**ErrCheckLogs** が必要であると判断した最古のログよりも後に作成されたログ ファイルにエラーが見つかった場合、この関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="466e0-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="466e0-132">データベースを最新状態にするために必要になるログ ファイルよりも後に生成されたものにログ ファイル エラーが見つかった場合にも、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="466e0-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="466e0-133">識別されたログ ファイルを使用してデータベースをクリーン シャットダウン状態にすることは可能ですが、それよりも後の破損したログ ファイルで指定されたトランザクションは適用されないため、データベースの復元時にデータを損失することになります。</span><span class="sxs-lookup"><span data-stu-id="466e0-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="466e0-134">**CChkSGFiles** オブジェクトでは、**ErrInit** 関数で登録したすべてのログ ファイルが実際に確認されたかどうかを判別します。</span><span class="sxs-lookup"><span data-stu-id="466e0-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="466e0-135">正常に確認されなかったログがあると、**ErrTerm** 関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="466e0-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="466e0-136">マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのマルチスレッドの部分で **ErrCheckLogs** 関数を呼び出すことができますが、**CCheckSGFiles** オブジェクトごとに 1 回しか呼び出せません。</span><span class="sxs-lookup"><span data-stu-id="466e0-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="466e0-137">Requirements</span><span class="sxs-lookup"><span data-stu-id="466e0-137">Requirements</span></span>

<span data-ttu-id="466e0-138">Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="466e0-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="466e0-139">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="466e0-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

