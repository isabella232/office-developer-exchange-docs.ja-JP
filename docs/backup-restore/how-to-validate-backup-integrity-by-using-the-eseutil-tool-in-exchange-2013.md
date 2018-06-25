---
title: Exchange 2013 の Eseutil ツールを使用してバックアップの整合性を検証します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。
ms.openlocfilehash: 03c4c23d433418911240bbe7c337308a989f3739
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758857"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a><span data-ttu-id="4d8c8-103">Exchange 2013 の Eseutil ツールを使用してバックアップの整合性を検証します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-103">Validate backup integrity by using the Eseutil tool in Exchange 2013</span></span>

<span data-ttu-id="4d8c8-104">Exchange ストアのバックアップを検証するための Eseutil コマンドライン ツールの使用方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-104">Find out how to use the Eseutil command-line tool to validate a backup of the Exchange store.</span></span> 
  
<span data-ttu-id="4d8c8-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4d8c8-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="4d8c8-106">ボリューム シャドウ コピー サービス (VSS) は、Exchange のデータベースへの書き込み中に、バックアップを作成できます、ため、サーバーはすべてのページを修正されず、必要な整合性チェックを実行します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-106">Because the Volume Shadow Copy Service (VSS) can create backups while Exchange continues to write to the database, the server does not touch all the pages and perform the necessary consistency checks.</span></span> <span data-ttu-id="4d8c8-107">このため、VSS を使用するバックアップと復元のアプリケーションは、スナップショットの整合性を確認してください。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-107">For this reason, any backup and restore application that uses VSS must verify snapshot consistency.</span></span> <span data-ttu-id="4d8c8-108">Exchange Server 2013 には、スナップショットの整合性をチェックするための次の 2 つの方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-108">Exchange Server 2013 supports the following two methods for checking snapshot consistency:</span></span> 
  
- <span data-ttu-id="4d8c8-109">CHKSGFILES API</span><span class="sxs-lookup"><span data-stu-id="4d8c8-109">The CHKSGFILES API</span></span>
    
- <span data-ttu-id="4d8c8-110">Eseutil コマンドライン ツール</span><span class="sxs-lookup"><span data-stu-id="4d8c8-110">The Eseutil command-line tool</span></span>
    
<span data-ttu-id="4d8c8-111">検出、診断、バックアップ ・ アプリケーションをより簡単にし、CHKSGFILES の一貫性の時に検出されたエラーの報告を確認するためには、CHKSGFILES API を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-111">We recommend that you use the CHKSGFILES API because it is easier for the backup application to detect, diagnose, and report errors that are found during the CHKSGFILES consistency check.</span></span> <span data-ttu-id="4d8c8-112">CHKSGFILES API を使用する方法の詳細については、 [Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-112">For information about how to use the CHKSGFILES API, see [Validate backup integrity by using the CHKSGFILES API in Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).</span></span>
  
## <a name="running-the-eseutil-tool"></a><span data-ttu-id="4d8c8-113">Eseutil ツールの実行</span><span class="sxs-lookup"><span data-stu-id="4d8c8-113">Running the Eseutil tool</span></span>

<span data-ttu-id="4d8c8-114">スナップショットの整合性を検査するには、次の表で特定されるデータベース ファイルとログ ファイルに対して Eseutil コマンドを実行します。 </span><span class="sxs-lookup"><span data-stu-id="4d8c8-114">To check the snapshot consistency, run the eseutil command against the database and log files that are identified in the following table.</span></span> 
  
<span data-ttu-id="4d8c8-115">**表 1 です。バックアップの種類ごとに、Eseutil.exe コマンド**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-115">**Table 1. Eseutil.exe commands for each backup type**</span></span>

|<span data-ttu-id="4d8c8-116">**ファイルの種類とバックアップの種類**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-116">**File type/backup type**</span></span>|<span data-ttu-id="4d8c8-117">**フル ・ バックアップ**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-117">**Full backup**</span></span>|<span data-ttu-id="4d8c8-118">**コピー バックアップ**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-118">**Copy backup**</span></span>|<span data-ttu-id="4d8c8-119">**インクリメンタル ・ バックアップ**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-119">**Incremental backup**</span></span>|<span data-ttu-id="4d8c8-120">**差分バックアップ**</span><span class="sxs-lookup"><span data-stu-id="4d8c8-120">**Differential backup**</span></span>|
|:-----|:-----|:-----|:-----|:-----|
|<span data-ttu-id="4d8c8-121">.edb</span><span class="sxs-lookup"><span data-stu-id="4d8c8-121">.edb</span></span>  <br/> |<span data-ttu-id="4d8c8-122">"eseutil /k /i"</span><span class="sxs-lookup"><span data-stu-id="4d8c8-122">"eseutil /k /i"</span></span>  <br/> |<span data-ttu-id="4d8c8-123">"eseutil /k /i"</span><span class="sxs-lookup"><span data-stu-id="4d8c8-123">"eseutil /k /i"</span></span>  <br/> |<span data-ttu-id="4d8c8-124">適用できません</span><span class="sxs-lookup"><span data-stu-id="4d8c8-124">Not applicable</span></span>  <br/> |<span data-ttu-id="4d8c8-125">適用できません</span><span class="sxs-lookup"><span data-stu-id="4d8c8-125">Not applicable</span></span>  <br/> |
|<span data-ttu-id="4d8c8-126">.log</span><span class="sxs-lookup"><span data-stu-id="4d8c8-126">.log</span></span>  <br/> |<span data-ttu-id="4d8c8-127">"eseutil /k" (1)</span><span class="sxs-lookup"><span data-stu-id="4d8c8-127">"eseutil /k" (1)</span></span>  <br/> |<span data-ttu-id="4d8c8-128">"eseutil /k" (1)</span><span class="sxs-lookup"><span data-stu-id="4d8c8-128">"eseutil /k" (1)</span></span>  <br/> |<span data-ttu-id="4d8c8-129">"eseutil /k" (2)</span><span class="sxs-lookup"><span data-stu-id="4d8c8-129">"eseutil /k" (2)</span></span>  <br/> |<span data-ttu-id="4d8c8-130">"eseutil /k" (2)</span><span class="sxs-lookup"><span data-stu-id="4d8c8-130">"eseutil /k" (2)</span></span>  <br/> |
   
> [!NOTE]
> <span data-ttu-id="4d8c8-131">.stm ファイルと .chk ファイルには、Eseutil コマンドを実行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-131">You do not need to run the eseutil command against .stm and .chk files.</span></span> 
  
<span data-ttu-id="4d8c8-132">番号、ログ ファイルの生成を持つすべてのログ ファイルは、生成のチェックポイントのログ ファイルの数、スナップショット データベースをリカバリするために必要以上には。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-132">All the log files that have a log file generation number that is equal to or greater than the generation number of the checkpoint log file are required in order to recover a snapshot database.</span></span> <span data-ttu-id="4d8c8-133">、存在する場合は現在のログ ファイル (Enn.log) がデータベースのリカバリに必要なも。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-133">If it exists, the current log file (Enn.log) is also required for database recovery.</span></span> <span data-ttu-id="4d8c8-134">必要なログ ファイルには、整合性チェックが失敗した場合、依頼者は、 [BackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382651%28v=vs.85%29.aspx)メソッドを呼び出す前に、バックアップ コンポーネントの状態を FALSE に設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-134">If any of the required log files fail the consistency check, the requester must make sure that the status of the backup component is set to FALSE before it calls the [BackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382651%28v=vs.85%29.aspx) method.</span></span> <span data-ttu-id="4d8c8-135">チェックポイント ・ ログ ・ ファイルを識別するには、スナップショットのチェックポイント ファイルに対して Eseutil.exe を実行し、解析の出力」のチェックポイント:.」</span><span class="sxs-lookup"><span data-stu-id="4d8c8-135">To identify the checkpoint log file, run Eseutil.exe against the snapshot checkpoint file and parse the output for "Checkpoint:."</span></span> <span data-ttu-id="4d8c8-136">次の例では、チェックポイント ・ ファイルに対して Eseutil.exe を実行する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-136">The following example shows how to run Eseutil.exe against a checkpoint file.</span></span> 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

<span data-ttu-id="4d8c8-p104">この例の 2 行目は戻り値です。0x20 は、チェックポイント ログ ファイルのログ世代番号 (16 進数) です。この例では、スナップショット データベースの復旧には E01000020.log 以降のログ ファイルに破損がないことが必要です。これは、データベース自体が物理的な整合性検査に合格していても同じことです。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-p104">The second line in the example is the return value, where 0x20 is the hexadecimal log generation number of the checkpoint log file. In this example, any log files, including E01000020.log and greater, must not be corrupt in order to recover the snapshot database, even if the database itself has already passed the physical consistency check.</span></span>
  
<span data-ttu-id="4d8c8-p105">データベースの復旧には、増分バックアップまたは差分バックアップのセットに含まれるすべてのログ ファイルが必要になります。ログ シーケンスの整合性は、ログ ファイルのプレフィックスに対して Eseutil.exe を実行することで検査できます。次の例は、特定のパスにある E01xxxxx.log という形式のすべてのログ ファイルに対して整合性検査を実行する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-p105">All log files in an incremental or differential backup set are required for database recovery. You can check the consistency of a log sequence by running Eseutil.exe against the log file prefix. The following example shows how to run consistency checks against all the files of the form E01xxxxx.log on a given path.</span></span>
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a><span data-ttu-id="4d8c8-142">Eseutil.exe の出力の確認</span><span class="sxs-lookup"><span data-stu-id="4d8c8-142">Checking the Eseutil.exe output</span></span>

<span data-ttu-id="4d8c8-143">依頼者は、すべて終了 ERRORLEVEL エラー値が返されますが負でないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-143">The requester must verify that all the exit ERRORLEVEL error values that are returned are nonnegative.</span></span> <span data-ttu-id="4d8c8-144">ERRORLEVEL の値については、[一般的な Eseutil エラーのリファレンス](http://technet.microsoft.com/en-us/library/aa996759%28v=exchg.80%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-144">For information about ERRORLEVEL values, see [Reference for Common Eseutil Errors](http://technet.microsoft.com/en-us/library/aa996759%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="4d8c8-145">コマンドラインで ERRORLEVEL を表示するには、入力「エコー % エラーレベル %」Eseutil.exe の実行が完了した後です。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-145">To see the ERRORLEVEL at the command line, type "echo %errorlevel%" after Eseutil.exe finishes running.</span></span> <span data-ttu-id="4d8c8-146">負のエラー レベルは、1 つまたは複数のファイルが破損していることを示します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-146">A negative ERRORLEVEL indicates that one or more files is corrupted.</span></span>
  
<span data-ttu-id="4d8c8-147">リクエスターは、 **BackupComplete**メソッドを呼び出して、前に、バックアップ コンポーネントの状態に整合性チェックの結果が反映されていることを確認してくださいする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-147">Before the requester calls the **BackupComplete** method, it must make sure that the status of the backup component reflects the result of the consistency check.</span></span> <span data-ttu-id="4d8c8-148">破損が見つかった場合はステータスになります。破損が検出されず、状態が TRUE になります。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-148">If any corruption was found, the status will be FALSE; if no corruption was found, the status will be TRUE.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4d8c8-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d8c8-149">See also</span></span>

- [<span data-ttu-id="4d8c8-150">Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-150">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [<span data-ttu-id="4d8c8-151">バックアップを作成し、Exchange 2013 のアプリケーションを復元します。</span><span class="sxs-lookup"><span data-stu-id="4d8c8-151">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="4d8c8-152">CChkSGFiles クラスの参照</span><span class="sxs-lookup"><span data-stu-id="4d8c8-152">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="4d8c8-153">Exchange 2013 のバックアップと復元の概念</span><span class="sxs-lookup"><span data-stu-id="4d8c8-153">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

