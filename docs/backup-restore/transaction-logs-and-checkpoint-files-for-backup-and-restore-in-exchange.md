---
title: Exchange でのバックアップと復元のトランザクションログとチェックポイントファイル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: トランザクションログとチェックポイントファイルについての情報と、Exchange 2013 データのバックアップと復元にどのように使用されているかを確認します。
ms.openlocfilehash: 5b01fc6924f82e76943795df877ae84b1fde087b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456389"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a><span data-ttu-id="b0a04-103">Exchange でのバックアップと復元のトランザクションログとチェックポイントファイル</span><span class="sxs-lookup"><span data-stu-id="b0a04-103">Transaction logs and checkpoint files for backup and restore in Exchange</span></span>

<span data-ttu-id="b0a04-104">トランザクションログとチェックポイントファイルについての情報と、Exchange 2013 データのバックアップと復元にどのように使用されているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b0a04-104">Find information about transaction logs and checkpoint files and how they are used to back up and restore Exchange 2013 data.</span></span>
  
<span data-ttu-id="b0a04-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b0a04-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="b0a04-106">この記事では、Exchange Server 2013 がトランザクションログとチェックポイントファイルを使用してデータ損失を防ぐ方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0a04-106">This article describes how Exchange Server 2013 uses transaction logs and checkpoint files to help prevent data loss.</span></span> <span data-ttu-id="b0a04-107">この情報は、Windows Server 2008 以降の Windows Server の各バージョンでボリューム シャドウ コピー サービス (VSS) を使用するバックアップおよび復元アプリケーションを開発するときに重要になります。</span><span class="sxs-lookup"><span data-stu-id="b0a04-107">It is important to be aware of this information when you develop backup and restore applications that use the Volume Shadow Copy Service (VSS) in versions of Windows Server starting with Windows Server 2008.</span></span>
  
## <a name="transaction-logs-in-exchange-2013"></a><span data-ttu-id="b0a04-108">Exchange 2013 のトランザクション ログ</span><span class="sxs-lookup"><span data-stu-id="b0a04-108">Transaction logs in Exchange 2013</span></span>

<span data-ttu-id="b0a04-109">Exchange 2013 は、データベースごとに1つのトランザクションログファイルセットを保持します。</span><span class="sxs-lookup"><span data-stu-id="b0a04-109">Exchange 2013 maintains a single set of transaction log files for each database.</span></span> <span data-ttu-id="b0a04-110">トランザクションは、データベースの状態または内容を変更する任意の操作として定義されます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-110">A transaction is defined as any operation that changes the state or contents of the database.</span></span> <span data-ttu-id="b0a04-111">各データベースのトランザクションログファイルには、データベースで実行されたすべてのトランザクションが記録されます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-111">The transaction log files for an individual database record all the transactions performed on the database.</span></span> <span data-ttu-id="b0a04-112">トランザクションのレコードは、データベース内で実行される前にトランザクションログに書き込まれます。これにより、データベースの障害が発生した場合に、コミットされたすべてのトランザクションを回復できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b0a04-112">Records of the transactions are written to the transaction logs before they are made in the database itself, to ensure that all committed transactions can be recovered in the event of a database failure.</span></span> <span data-ttu-id="b0a04-113">Exchange 2013 データベースのトランザクションログは、トランザクションがデータベースファイルにコミットされる前にディスクに格納されます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-113">Exchange 2013 database transaction logs are stored on disk before the transactions are committed to the database file.</span></span> 
  
<span data-ttu-id="b0a04-114">データベースが更新される前のトランザクションの記録は、先行書き込みログと呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-114">The recording of the transactions before the database is updated is called write-ahead logging.</span></span> <span data-ttu-id="b0a04-115">データベースが正しい状態に戻されるようにするために、Exchange 2013 は、ページベースの書き込みとチェックポイントを使用してデータベースファイルにデータを書き込みます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-115">To help ensure that the database is correctly brought back to the proper state, Exchange 2013 writes data into the database files by using page-based writes and checkpoints.</span></span> <span data-ttu-id="b0a04-116">通常の操作では、Exchange ストアは最初にデータベースの変更をトランザクションログに記録した後、データベースのメモリ内コピーにその変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-116">During regular operations, the Exchange store first records database changes in the transaction logs, and then makes those changes on an in-memory copy of the database.</span></span> <span data-ttu-id="b0a04-117">トランザクションログには、各トランザクションの開始と終了が記録されます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-117">The transaction logs record the beginning and end of each transaction.</span></span> <span data-ttu-id="b0a04-118">これにより、後でデータベースの操作を元に戻したりロールバックしたりするために十分な情報を利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b0a04-118">This ensures that sufficient information is available to later undo or roll back operations in the database.</span></span>
  
<span data-ttu-id="b0a04-119">ディスク上のデータベース ファイルが破損していても、トランザクション ログ ファイルが無事なときのエラーから回復する場合、復元アプリケーションでは、最初に正常だとわかっているデータベース ファイルのコピーを復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0a04-119">When recovering from errors in which the database file on disk is damaged, but the transaction logs are intact, your restore application must first restore a known good copy of the database file.</span></span>
  
<span data-ttu-id="b0a04-p104">Exchange ストアは、以前にバックアップしたトランザクション ログからトランザクションを再生してから、残りのトランザクションをディスク上のトランザクション ログ ファイルから再生します。トランザクションがトランザクション ログに記録される時点と、そのトランザクションが実際にデータベース ファイルに書き込まれる時点の間でシステムに障害が発生すると、トランザクションが失われる可能性がある点にご注意ください。 </span><span class="sxs-lookup"><span data-stu-id="b0a04-p104">The Exchange store replays the transactions from the previously backed up transaction logs, and then replays any remaining transactions from the on-disk transaction log files. Note that sometimes transactions can be lost if the system fails between when the transactions are recorded in the transaction logs, and when they are actually written to the database files.</span></span> 
  
<span data-ttu-id="b0a04-p105">Exchange ストアは、定期的にメモリ内のデータベース イメージを調べて、どのページに変更があったかを判断します。Exchange ストアは、保留中の変更を結合してから、該当するページをディスク上のデータベース ファイルに書き込みます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-p105">Periodically, the Exchange store checks the in-memory database image, and then determines which pages have changed. The Exchange store combines the pending changes, and then writes those pages to the database file on disk.</span></span>
  
## <a name="checkpoint-files-in-exchange-2013"></a><span data-ttu-id="b0a04-124">Exchange 2013 のチェックポイント ファイル</span><span class="sxs-lookup"><span data-stu-id="b0a04-124">Checkpoint files in Exchange 2013</span></span>

<span data-ttu-id="b0a04-p106">チェックポイント ファイルには、ログに記録されたトランザクションのどれがディスク上のデータベース ファイルに書き込まれたかを記録します。チェックポイント ファイルは、トランザクション ログのエントリで更新されたすべてのデータベース ページが正常にディスクに書き込まれた時点で先に進められます。チェックポイント ファイルは、既にディスク上のデータベース イメージに含まれるトランザクションを記録しているため、Exchange ストアは、チェックポイントの後に発生したトランザクションを再生するだけで十分です。バックアップ周期の長さによっては、システム障害時にデータベースに再生する必要のあるトランザクションの数を大幅に削減できます。</span><span class="sxs-lookup"><span data-stu-id="b0a04-p106">A checkpoint file records which logged transactions have been written to the on-disk database files. The checkpoint is advanced when all the database pages that have been modified by entries in the transaction logs are successfully written to disk. Because the checkpoint file records which transactions are already in the on-disk database image, the Exchange store only needs to replay transactions that occurred after the checkpoint. Depending on the time period between backups, this can greatly decrease the number of transactions that must be replayed into the database if a system failure occurs.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b0a04-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0a04-129">See also</span></span>

- [<span data-ttu-id="b0a04-130">Exchange 2013 のバックアップと復元の概念</span><span class="sxs-lookup"><span data-stu-id="b0a04-130">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
- [<span data-ttu-id="b0a04-131">Exchange 2013 のバックアップ操作の種類</span><span class="sxs-lookup"><span data-stu-id="b0a04-131">Types of backup operations for Exchange 2013</span></span>](types-of-backup-operations-for-exchange-2013.md)
- [<span data-ttu-id="b0a04-132">Exchange 2013 のデータベースを復元する</span><span class="sxs-lookup"><span data-stu-id="b0a04-132">Restoring Exchange 2013 databases</span></span>](restoring-exchange-2013-databases.md)
    

