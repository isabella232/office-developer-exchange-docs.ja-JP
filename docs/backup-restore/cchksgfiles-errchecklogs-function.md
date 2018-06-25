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
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758864"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="3fbfc-103">CChkSGFiles.ErrCheckLogs 関数</span><span class="sxs-lookup"><span data-stu-id="3fbfc-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="3fbfc-104">**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3fbfc-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="3fbfc-105">**ErrInit**関数で指定されたすべてのデータベース ファイルのログ ファイルを検証します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="3fbfc-106">検証済みのログは、パス内に存在し、 **ErrInit**に渡される 3 文字ベースのログ ファイル名があります。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="3fbfc-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="3fbfc-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="3fbfc-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="3fbfc-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="3fbfc-109">出力パラメーターです。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-109">Output parameter.</span></span> <span data-ttu-id="3fbfc-110">**True の場合**、このパラメーターを示しますが、トランザクション ・ ログ ・ ファイル、これらのエラーのエラーが検出されたことがとされたに不要なログ ファイル内に見つかったすべてデータベース クリーン シャット ダウン状態にデータを失わずにします。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="3fbfc-111">このパラメーターに返される**場合は true**の値は、 **ErrCheckLogs**には、 **errSuccess**が返されるときにのみに有効です。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="3fbfc-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="3fbfc-112">ulFlags</span></span>
  
<span data-ttu-id="3fbfc-p103">オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-p103">Optional input parameter. This value is reserved for future use. The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="3fbfc-116">�߂�l</span><span class="sxs-lookup"><span data-stu-id="3fbfc-116">Return value</span></span>

<span data-ttu-id="3fbfc-117">[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="3fbfc-118">ログ ファイルにエラーが検出された場合でも、この関数に**errSuccess**を返すことができますを覚えておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="3fbfc-119">したがって、 **ErrCheckLogs**に**errSuccess**が返されるとき、アプリケーションもを確認する**pfOnlyUnnecessaryLogsCorrupt**の戻り値パラメーター。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="3fbfc-120">**ErrCheckLogs**に**errSuccess**が返されるときに**pfOnlyUnnecessaryLogsCorrupts**が**true**の場合は、データベースを最新にする必要がないログ ファイルでは、1 つまたは複数のエラーが検出されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3fbfc-121">備考</span><span class="sxs-lookup"><span data-stu-id="3fbfc-121">Remarks</span></span>

<span data-ttu-id="3fbfc-122">**ErrCheckLogs**関数が呼び出される前に、 **ErrCheckDbHeaders**関数を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="3fbfc-123">Exchange データベースのトランザクション ログ ファイルをチェックすると、ログ ファイルのいくつか必要がありますデータが失われることがなく、クリーン シャット ダウン状態にストレージ グループ内のデータベースをオンラインにその他のログ ファイルは必要はありませんが。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="3fbfc-124">**ErrCheckLogs**関数は、最も古いと最新のデータベースを表示するために必要な最新のログ ファイルの両方を決定します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="3fbfc-125">**ErrCheckLogs**関数は、 **ErrInit**関数に渡されるときにも、指定した 3 文字ベース ファイル名を持つ、指定したパス内のすべてのログ ファイルを確認します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="3fbfc-126">ログ ファイルでエラーが見つからない場合、 **ErrCheckLogs**は**errSuccess**を返します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="3fbfc-127">必要なログ ファイルのいずれかが壊れている可能性がある、 **ErrCheckLogs**はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="3fbfc-128">必要な最初のものよりも古いログ ファイルでのみエラーが見つかった場合、この関数は**errSuccess**を返し、 **pfOnlyUnnecessaryLogCorrupt**の戻り値パラメーターを**true**に設定。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="3fbfc-129">これら古いログ ・ ファイルの一部にエラーがある場合は、その可能性がある警告が表示されます、アプリケーションが認識する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="3fbfc-130">いずれの場合も、これらのエラーしないデータベースの全体的な整合性に影響を与えるか、ログ フォワードを実行が成功するかどうかに影響を与えます。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="3fbfc-131">最も早く訪れる後に作成された任意のログ ファイルにエラーが見つかった場合は、 **ErrCheckLogs**を決定するログが必要な関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="3fbfc-132">後に生成されたログ ファイルは、ログ ファイルのエラーが見つかった場合でも最新状態にするために必要なのエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="3fbfc-133">特定のログ ファイルを使用してクリーン シャット ダウンの状態にデータベースを移動することですが、後で破損したログ ファイルで指定されているトランザクションは適用されません、データベースが復元されたときにデータが失われる結果。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="3fbfc-134">**CChkSGFiles**オブジェクトは、実際にチェック アウトされたすべてのログ ファイルを**ErrInit**関数に登録されているかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="3fbfc-135">表示しない場合は、すべてのログがない正常にチェック、 **ErrTerm**関数はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="3fbfc-136">マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **ErrCheckLogs**関数を呼び出すことができますが、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="3fbfc-137">必要条件</span><span class="sxs-lookup"><span data-stu-id="3fbfc-137">Requirements</span></span>

<span data-ttu-id="3fbfc-138">Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="3fbfc-139">アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fbfc-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

