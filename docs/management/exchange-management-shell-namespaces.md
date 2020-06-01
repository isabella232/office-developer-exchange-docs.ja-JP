---
title: Exchange 管理シェルの名前空間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff849238-06b7-4891-884b-c51ce0f1ebbc
description: Exchange で Exchange 管理シェルの名前空間に関する情報を検索します。
ms.openlocfilehash: 370c3e6cde48662eba8c62ad20e42fb716e66f2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435815"
---
# <a name="exchange-management-shell-namespaces"></a><span data-ttu-id="4389a-103">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="4389a-103">Exchange Management Shell namespaces</span></span>

<span data-ttu-id="4389a-104">Exchange で Exchange 管理シェルの名前空間に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="4389a-104">Find information about the namespaces for the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="4389a-105">**適用対象:** Exchange Online |Exchange Server 2013 |Office 365</span><span class="sxs-lookup"><span data-stu-id="4389a-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="4389a-106">Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降のバージョンの Exchange で作動する Exchange 管理シェルのアプリケーションは、**System.Management.Automation** 名前空間が公開する型を通じて、Windows PowerShell 環境と対話します。</span><span class="sxs-lookup"><span data-stu-id="4389a-106">Exchange Management Shell applications for Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 interact with the Windows PowerShell environment through the types that are exposed by the **System.Management.Automation** namespace.</span></span> <span data-ttu-id="4389a-107">Exchange 管理シェル コマンドレットでは、多数の Exchange ライブラリにある型を使用します。</span><span class="sxs-lookup"><span data-stu-id="4389a-107">The Exchange Management Shell cmdlets use types from a number of Exchange libraries.</span></span> <span data-ttu-id="4389a-108">このセクションでは、Exchange 管理シェル コマンドレットが使用する Exchange ライブラリにある型およびインターフェイスに関する参照情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4389a-108">This section provides reference information about the types and interfaces from the Exchange libraries that are used by Exchange Management Shell cmdlets.</span></span> 
  
<span data-ttu-id="4389a-109">Exchange 管理シェルには、次の名前空間が格納されています。</span><span class="sxs-lookup"><span data-stu-id="4389a-109">The Exchange Management Shell contains the following namespaces:</span></span>
  
- [<span data-ttu-id="4389a-110">Microsoft の構成タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-110">Microsoft.Exchange.Configuration.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Configuration.Tasks.aspx)
    
- [<span data-ttu-id="4389a-111">Microsoft のデータ交換</span><span class="sxs-lookup"><span data-stu-id="4389a-111">Microsoft.Exchange.Data</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx)
    
- [<span data-ttu-id="4389a-112">Microsoft. ディレクトリ</span><span class="sxs-lookup"><span data-stu-id="4389a-112">Microsoft.Exchange.Data.Directory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.aspx)
    
- [<span data-ttu-id="4389a-113">「」の情報を管理する</span><span class="sxs-lookup"><span data-stu-id="4389a-113">Microsoft.Exchange.Data.Directory.Management</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Management.aspx)
    
- [<span data-ttu-id="4389a-114">(ディレクトリアクセス許可)</span><span class="sxs-lookup"><span data-stu-id="4389a-114">Microsoft.Exchange.Data.Directory.Permission</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Permission.aspx)
    
- [<span data-ttu-id="4389a-115">Microsoft Exchange. ディレクトリの受信者</span><span class="sxs-lookup"><span data-stu-id="4389a-115">Microsoft.Exchange.Data.Directory.Recipient</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Recipient.aspx)
    
- [<span data-ttu-id="4389a-116">SystemConfiguration を行います。</span><span class="sxs-lookup"><span data-stu-id="4389a-116">Microsoft.Exchange.Data.Directory.SystemConfiguration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.aspx)
    
- [<span data-ttu-id="4389a-117">Microsoft Exchange Server での Mapi</span><span class="sxs-lookup"><span data-stu-id="4389a-117">Microsoft.Exchange.Data.Mapi</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mapi.aspx)
    
- [<span data-ttu-id="4389a-118">Get-queuedigest です。</span><span class="sxs-lookup"><span data-stu-id="4389a-118">Microsoft.Exchange.Data.QueueDigest</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.QueueDigest.aspx)
    
- [<span data-ttu-id="4389a-119">Microsoft Exchange Server Viewer</span><span class="sxs-lookup"><span data-stu-id="4389a-119">Microsoft.Exchange.Data.QueueViewer</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.QueueViewer.aspx)
    
- [<span data-ttu-id="4389a-120">RightsManagement です。</span><span class="sxs-lookup"><span data-stu-id="4389a-120">Microsoft.Exchange.Data.RightsManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.RightsManagement.aspx)
    
- [<span data-ttu-id="4389a-121">Microsoft. データストレージ</span><span class="sxs-lookup"><span data-stu-id="4389a-121">Microsoft.Exchange.Data.Storage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.aspx)
    
- [<span data-ttu-id="4389a-122">その後、データを格納します。</span><span class="sxs-lookup"><span data-stu-id="4389a-122">Microsoft.Exchange.Data.Storage.ActiveMonitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.ActiveMonitoring.aspx)
    
- [<span data-ttu-id="4389a-123">Microsoft によるデータ管理</span><span class="sxs-lookup"><span data-stu-id="4389a-123">Microsoft.Exchange.Data.Storage.Management</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.Management.aspx)
    
- [<span data-ttu-id="4389a-124">Microsoft は、移行を行います。</span><span class="sxs-lookup"><span data-stu-id="4389a-124">Microsoft.Exchange.Data.Storage.Management.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.Management.Migration.aspx)
    
- [<span data-ttu-id="4389a-125">その後、Microsoft のデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="4389a-125">Microsoft.Exchange.Data.Storage.StoreConfigurableType</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.StoreConfigurableType.aspx)
    
- [<span data-ttu-id="4389a-126">Microsoft Exchange の認証</span><span class="sxs-lookup"><span data-stu-id="4389a-126">Microsoft.Exchange.EdgeSync.Validation</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.EdgeSync.Validation.aspx)
    
- [<span data-ttu-id="4389a-127">MailboxReplicationService</span><span class="sxs-lookup"><span data-stu-id="4389a-127">Microsoft.Exchange.MailboxReplicationService</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MailboxReplicationService.aspx)
    
- [<span data-ttu-id="4389a-128">エージェントの管理タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-128">Microsoft.Exchange.Management.AgentTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.AgentTasks.aspx)
    
- [<span data-ttu-id="4389a-129">ClassificationDefinitions の管理</span><span class="sxs-lookup"><span data-stu-id="4389a-129">Microsoft.Exchange.Management.ClassificationDefinitions</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ClassificationDefinitions.aspx)
    
- [<span data-ttu-id="4389a-130">Microsoft. 管理内線番号</span><span class="sxs-lookup"><span data-stu-id="4389a-130">Microsoft.Exchange.Management.Extension</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Extension.aspx)
    
- [<span data-ttu-id="4389a-131">「」を事前に移植する</span><span class="sxs-lookup"><span data-stu-id="4389a-131">Microsoft.Exchange.Management.FfoReporting</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.FfoReporting.aspx)
    
- [<span data-ttu-id="4389a-132">「」をお寄せください。</span><span class="sxs-lookup"><span data-stu-id="4389a-132">Microsoft.Exchange.Management.FfoReporting.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.FfoReporting.Common.aspx)
    
- [<span data-ttu-id="4389a-133">Microsoft Exchange 管理のためのポリシー。 AddressRewrite</span><span class="sxs-lookup"><span data-stu-id="4389a-133">Microsoft.Exchange.Management.MessagingPolicies.AddressRewrite</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.MessagingPolicies.AddressRewrite.aspx)
    
- [<span data-ttu-id="4389a-134">Microsoft 管理移行</span><span class="sxs-lookup"><span data-stu-id="4389a-134">Microsoft.Exchange.Management.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Migration.aspx)
    
- [<span data-ttu-id="4389a-135">Microsoft 管理用の OutlookProtectionRules</span><span class="sxs-lookup"><span data-stu-id="4389a-135">Microsoft.Exchange.Management.OutlookProtectionRules</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.OutlookProtectionRules.aspx)
    
- [<span data-ttu-id="4389a-136">PolicyNudges の管理</span><span class="sxs-lookup"><span data-stu-id="4389a-136">Microsoft.Exchange.Management.PolicyNudges</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.PolicyNudges.aspx)
    
- [<span data-ttu-id="4389a-137">Microsoft Exchange 管理タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-137">Microsoft.Exchange.Management.ProvisioningTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ProvisioningTasks.aspx)
    
- [<span data-ttu-id="4389a-138">Microsoft Exchange 管理タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-138">Microsoft.Exchange.Management.RecipientTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.RecipientTasks.aspx)
    
- [<span data-ttu-id="4389a-139">Microsoft 管理タスク。一般的な</span><span class="sxs-lookup"><span data-stu-id="4389a-139">Microsoft.Exchange.Management.ReportingTask.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.Common.aspx)
    
- [<span data-ttu-id="4389a-140">「」という Microsoft の管理タスク。</span><span class="sxs-lookup"><span data-stu-id="4389a-140">Microsoft.Exchange.Management.ReportingTask.Query</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.Query.aspx)
    
- [<span data-ttu-id="4389a-141">Microsoft の管理タスクのためのレポート</span><span class="sxs-lookup"><span data-stu-id="4389a-141">Microsoft.Exchange.Management.ReportingTask.TenantReport</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.TenantReport.aspx)
    
- [<span data-ttu-id="4389a-142">RightsManagement の管理</span><span class="sxs-lookup"><span data-stu-id="4389a-142">Microsoft.Exchange.Management.RightsManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.RightsManagement.aspx)
    
- [<span data-ttu-id="4389a-143">Microsoft 管理共有</span><span class="sxs-lookup"><span data-stu-id="4389a-143">Microsoft.Exchange.Management.Sharing</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Sharing.aspx)
    
- [<span data-ttu-id="4389a-144">Microsoft Exchange 管理タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-144">Microsoft.Exchange.Management.StoreTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.StoreTasks.aspx)
    
- [<span data-ttu-id="4389a-145">Microsoft 管理監督</span><span class="sxs-lookup"><span data-stu-id="4389a-145">Microsoft.Exchange.Management.Supervision</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Supervision.aspx)
    
- [<span data-ttu-id="4389a-146">「管理」の「SystemConfigurationTasks」</span><span class="sxs-lookup"><span data-stu-id="4389a-146">Microsoft.Exchange.Management.SystemConfigurationTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.SystemConfigurationTasks.aspx)
    
- [<span data-ttu-id="4389a-147">Microsoft 管理タスク</span><span class="sxs-lookup"><span data-stu-id="4389a-147">Microsoft.Exchange.Management.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tasks.aspx)
    
- [<span data-ttu-id="4389a-148">Microsoft の管理ツール</span><span class="sxs-lookup"><span data-stu-id="4389a-148">Microsoft.Exchange.Management.Tools</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tools.aspx)
    
- [<span data-ttu-id="4389a-149">Microsoft の管理</span><span class="sxs-lookup"><span data-stu-id="4389a-149">Microsoft.Exchange.Management.Tracking</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tracking.aspx)
    
- [<span data-ttu-id="4389a-150">Microsoft Exchange 管理. TransportLogSearchTasks</span><span class="sxs-lookup"><span data-stu-id="4389a-150">Microsoft.Exchange.Management.TransportLogSearchTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.TransportLogSearchTasks.aspx)
    
- [<span data-ttu-id="4389a-151">CompliancePrograms のようにします。</span><span class="sxs-lookup"><span data-stu-id="4389a-151">Microsoft.Exchange.MessagingPolicies.CompliancePrograms.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.CompliancePrograms.Tasks.aspx)
    
- [<span data-ttu-id="4389a-152">Microsoft Exchange Server のポリシージャーナリング</span><span class="sxs-lookup"><span data-stu-id="4389a-152">Microsoft.Exchange.MessagingPolicies.Journaling</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.Journaling.aspx)
    
- <span data-ttu-id="4389a-153">[[...]-[ルール]](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.Rules.Tasks.aspx)</span><span class="sxs-lookup"><span data-stu-id="4389a-153">[Microsoft.Exchange.MessagingPolicies.Rules.Tasks](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.Rules.Tasks.aspx)</span></span>
    
- [<span data-ttu-id="4389a-154">Microsoft Exchange の移行</span><span class="sxs-lookup"><span data-stu-id="4389a-154">Microsoft.Exchange.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Migration.aspx)
    
- [<span data-ttu-id="4389a-155">Microsoft Exchange の監視</span><span class="sxs-lookup"><span data-stu-id="4389a-155">Microsoft.Exchange.Monitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Monitoring.aspx)
    
- [<span data-ttu-id="4389a-156">「Microsoft Exchange Server の監視」</span><span class="sxs-lookup"><span data-stu-id="4389a-156">Microsoft.Exchange.Monitoring.ActiveMonitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Monitoring.ActiveMonitoring.aspx)
    
- [<span data-ttu-id="4389a-157">「」のようになります。</span><span class="sxs-lookup"><span data-stu-id="4389a-157">Microsoft.Exchange.Transport.Sync.Common.Subscription</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.aspx)
    
- [<span data-ttu-id="4389a-158">(サブスクリプションの接続のために)</span><span class="sxs-lookup"><span data-stu-id="4389a-158">Microsoft.Exchange.Transport.Sync.Common.Subscription.Connect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Connect.aspx)
    
- [<span data-ttu-id="4389a-159">「」のようにしてください。</span><span class="sxs-lookup"><span data-stu-id="4389a-159">Microsoft.Exchange.Transport.Sync.Common.Subscription.DeltaSync</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.DeltaSync.aspx)
    
- [<span data-ttu-id="4389a-160">「」というようになります。</span><span class="sxs-lookup"><span data-stu-id="4389a-160">Microsoft.Exchange.Transport.Sync.Common.Subscription.Imap</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Imap.aspx)
    
- [<span data-ttu-id="4389a-161">「」のようになります。</span><span class="sxs-lookup"><span data-stu-id="4389a-161">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pim</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Pim.aspx)
    
- [<span data-ttu-id="4389a-162">「」のようになります。</span><span class="sxs-lookup"><span data-stu-id="4389a-162">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pop</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Pop.aspx)
    
- [<span data-ttu-id="4389a-163">を行います。</span><span class="sxs-lookup"><span data-stu-id="4389a-163">Microsoft.Exchange.UM.Rpc</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.UM.Rpc.aspx)
    
- [<span data-ttu-id="4389a-164">Microsoft Exchange の共通</span><span class="sxs-lookup"><span data-stu-id="4389a-164">Microsoft.Exchange.UM.UMCommon</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.UM.UMCommon.aspx)
    
- [<span data-ttu-id="4389a-165">WorkloadManagement</span><span class="sxs-lookup"><span data-stu-id="4389a-165">Microsoft.Exchange.WorkloadManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.WorkloadManagement.aspx)
    
## <a name="see-also"></a><span data-ttu-id="4389a-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="4389a-166">See also</span></span>

- [<span data-ttu-id="4389a-167">Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="4389a-167">Exchange Management Shell</span></span>](exchange-management-shell.md)  
- [<span data-ttu-id="4389a-168">Exchange 管理シェル ツールの作成</span><span class="sxs-lookup"><span data-stu-id="4389a-168">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md) 
- [<span data-ttu-id="4389a-169">Exchange 管理シェル コマンドレットの入力と出力の種類</span><span class="sxs-lookup"><span data-stu-id="4389a-169">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
    

