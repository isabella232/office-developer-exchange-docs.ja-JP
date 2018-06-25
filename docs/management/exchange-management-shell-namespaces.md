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
ms.openlocfilehash: d1683f99fbd233c1b878eb86d529b58ea1ebd8c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759191"
---
# <a name="exchange-management-shell-namespaces"></a><span data-ttu-id="2af03-103">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="2af03-103">Exchange Management Shell namespaces</span></span>

<span data-ttu-id="2af03-104">Exchange で Exchange 管理シェルの名前空間に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="2af03-104">Find information about the namespaces for the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="2af03-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="2af03-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="2af03-106">Exchange のオンライン、Office 365 の一部として Exchange のオンラインまたは Exchange 2013 で開始する Exchange のバージョンの Exchange 管理シェルのアプリケーションが、**によって公開されている型を使って Windows PowerShell 環境と対話します。System.Management.Automation**名前空間です。</span><span class="sxs-lookup"><span data-stu-id="2af03-106">Exchange Management Shell applications for Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 interact with the Windows PowerShell environment through the types that are exposed by the **System.Management.Automation** namespace.</span></span> <span data-ttu-id="2af03-107">Exchange 管理シェル コマンドレットでは、多くの Exchange ライブラリから型を使用します。</span><span class="sxs-lookup"><span data-stu-id="2af03-107">The Exchange Management Shell cmdlets use types from a number of Exchange libraries.</span></span> <span data-ttu-id="2af03-108">このセクションでは、型と Exchange 管理シェル コマンドレットで使用されている Exchange ライブラリからインターフェイスに関するリファレンス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2af03-108">This section provides reference information about the types and interfaces from the Exchange libraries that are used by Exchange Management Shell cmdlets.</span></span> 
  
<span data-ttu-id="2af03-109">Exchange 管理シェルには、次の名前空間が格納されています。</span><span class="sxs-lookup"><span data-stu-id="2af03-109">The Exchange Management Shell contains the following namespaces:</span></span>
  
- [<span data-ttu-id="2af03-110">Microsoft.Exchange.Configuration.Tasks</span><span class="sxs-lookup"><span data-stu-id="2af03-110">Microsoft.Exchange.Configuration.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Configuration.Tasks.aspx)
    
- [<span data-ttu-id="2af03-111">Microsoft.Exchange.Data</span><span class="sxs-lookup"><span data-stu-id="2af03-111">Microsoft.Exchange.Data</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx)
    
- [<span data-ttu-id="2af03-112">Microsoft.Exchange.Data.Directory</span><span class="sxs-lookup"><span data-stu-id="2af03-112">Microsoft.Exchange.Data.Directory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.aspx)
    
- [<span data-ttu-id="2af03-113">Microsoft.Exchange.Data.Directory.Management</span><span class="sxs-lookup"><span data-stu-id="2af03-113">Microsoft.Exchange.Data.Directory.Management</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Management.aspx)
    
- [<span data-ttu-id="2af03-114">Microsoft.Exchange.Data.Directory.Permission</span><span class="sxs-lookup"><span data-stu-id="2af03-114">Microsoft.Exchange.Data.Directory.Permission</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Permission.aspx)
    
- [<span data-ttu-id="2af03-115">Microsoft.Exchange.Data.Directory.Recipient</span><span class="sxs-lookup"><span data-stu-id="2af03-115">Microsoft.Exchange.Data.Directory.Recipient</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.Recipient.aspx)
    
- [<span data-ttu-id="2af03-116">Microsoft.Exchange.Data.Directory.SystemConfiguration</span><span class="sxs-lookup"><span data-stu-id="2af03-116">Microsoft.Exchange.Data.Directory.SystemConfiguration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.aspx)
    
- [<span data-ttu-id="2af03-117">Microsoft.Exchange.Data.Mapi</span><span class="sxs-lookup"><span data-stu-id="2af03-117">Microsoft.Exchange.Data.Mapi</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mapi.aspx)
    
- [<span data-ttu-id="2af03-118">Microsoft.Exchange.Data.QueueDigest</span><span class="sxs-lookup"><span data-stu-id="2af03-118">Microsoft.Exchange.Data.QueueDigest</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.QueueDigest.aspx)
    
- [<span data-ttu-id="2af03-119">Microsoft.Exchange.Data.QueueViewer</span><span class="sxs-lookup"><span data-stu-id="2af03-119">Microsoft.Exchange.Data.QueueViewer</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.QueueViewer.aspx)
    
- [<span data-ttu-id="2af03-120">Microsoft.Exchange.Data.RightsManagement</span><span class="sxs-lookup"><span data-stu-id="2af03-120">Microsoft.Exchange.Data.RightsManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.RightsManagement.aspx)
    
- [<span data-ttu-id="2af03-121">Microsoft.Exchange.Data.Storage</span><span class="sxs-lookup"><span data-stu-id="2af03-121">Microsoft.Exchange.Data.Storage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.aspx)
    
- [<span data-ttu-id="2af03-122">Microsoft.Exchange.Data.Storage.ActiveMonitoring</span><span class="sxs-lookup"><span data-stu-id="2af03-122">Microsoft.Exchange.Data.Storage.ActiveMonitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.ActiveMonitoring.aspx)
    
- [<span data-ttu-id="2af03-123">Microsoft.Exchange.Data.Storage.Management</span><span class="sxs-lookup"><span data-stu-id="2af03-123">Microsoft.Exchange.Data.Storage.Management</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.Management.aspx)
    
- [<span data-ttu-id="2af03-124">Microsoft.Exchange.Data.Storage.Management.Migration</span><span class="sxs-lookup"><span data-stu-id="2af03-124">Microsoft.Exchange.Data.Storage.Management.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.Management.Migration.aspx)
    
- [<span data-ttu-id="2af03-125">Microsoft.Exchange.Data.Storage.StoreConfigurableType</span><span class="sxs-lookup"><span data-stu-id="2af03-125">Microsoft.Exchange.Data.Storage.StoreConfigurableType</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Storage.StoreConfigurableType.aspx)
    
- [<span data-ttu-id="2af03-126">Microsoft.Exchange.EdgeSync.Validation</span><span class="sxs-lookup"><span data-stu-id="2af03-126">Microsoft.Exchange.EdgeSync.Validation</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.EdgeSync.Validation.aspx)
    
- [<span data-ttu-id="2af03-127">Microsoft.Exchange.MailboxReplicationService</span><span class="sxs-lookup"><span data-stu-id="2af03-127">Microsoft.Exchange.MailboxReplicationService</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MailboxReplicationService.aspx)
    
- [<span data-ttu-id="2af03-128">Microsoft.Exchange.Management.AgentTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-128">Microsoft.Exchange.Management.AgentTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.AgentTasks.aspx)
    
- [<span data-ttu-id="2af03-129">Microsoft.Exchange.Management.ClassificationDefinitions</span><span class="sxs-lookup"><span data-stu-id="2af03-129">Microsoft.Exchange.Management.ClassificationDefinitions</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ClassificationDefinitions.aspx)
    
- [<span data-ttu-id="2af03-130">Microsoft.Exchange.Management.Extension</span><span class="sxs-lookup"><span data-stu-id="2af03-130">Microsoft.Exchange.Management.Extension</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Extension.aspx)
    
- [<span data-ttu-id="2af03-131">Microsoft.Exchange.Management.FfoReporting</span><span class="sxs-lookup"><span data-stu-id="2af03-131">Microsoft.Exchange.Management.FfoReporting</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.FfoReporting.aspx)
    
- [<span data-ttu-id="2af03-132">Microsoft.Exchange.Management.FfoReporting.Common</span><span class="sxs-lookup"><span data-stu-id="2af03-132">Microsoft.Exchange.Management.FfoReporting.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.FfoReporting.Common.aspx)
    
- [<span data-ttu-id="2af03-133">Microsoft.Exchange.Management.MessagingPolicies.AddressRewrite</span><span class="sxs-lookup"><span data-stu-id="2af03-133">Microsoft.Exchange.Management.MessagingPolicies.AddressRewrite</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.MessagingPolicies.AddressRewrite.aspx)
    
- [<span data-ttu-id="2af03-134">Microsoft.Exchange.Management.Migration</span><span class="sxs-lookup"><span data-stu-id="2af03-134">Microsoft.Exchange.Management.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Migration.aspx)
    
- [<span data-ttu-id="2af03-135">Microsoft.Exchange.Management.OutlookProtectionRules</span><span class="sxs-lookup"><span data-stu-id="2af03-135">Microsoft.Exchange.Management.OutlookProtectionRules</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.OutlookProtectionRules.aspx)
    
- [<span data-ttu-id="2af03-136">Microsoft.Exchange.Management.PolicyNudges</span><span class="sxs-lookup"><span data-stu-id="2af03-136">Microsoft.Exchange.Management.PolicyNudges</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.PolicyNudges.aspx)
    
- [<span data-ttu-id="2af03-137">Microsoft.Exchange.Management.ProvisioningTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-137">Microsoft.Exchange.Management.ProvisioningTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ProvisioningTasks.aspx)
    
- [<span data-ttu-id="2af03-138">Microsoft.Exchange.Management.RecipientTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-138">Microsoft.Exchange.Management.RecipientTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.RecipientTasks.aspx)
    
- [<span data-ttu-id="2af03-139">Microsoft.Exchange.Management.ReportingTask.Common</span><span class="sxs-lookup"><span data-stu-id="2af03-139">Microsoft.Exchange.Management.ReportingTask.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.Common.aspx)
    
- [<span data-ttu-id="2af03-140">Microsoft.Exchange.Management.ReportingTask.Query</span><span class="sxs-lookup"><span data-stu-id="2af03-140">Microsoft.Exchange.Management.ReportingTask.Query</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.Query.aspx)
    
- [<span data-ttu-id="2af03-141">Microsoft.Exchange.Management.ReportingTask.TenantReport</span><span class="sxs-lookup"><span data-stu-id="2af03-141">Microsoft.Exchange.Management.ReportingTask.TenantReport</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.ReportingTask.TenantReport.aspx)
    
- [<span data-ttu-id="2af03-142">Microsoft.Exchange.Management.RightsManagement</span><span class="sxs-lookup"><span data-stu-id="2af03-142">Microsoft.Exchange.Management.RightsManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.RightsManagement.aspx)
    
- [<span data-ttu-id="2af03-143">Microsoft.Exchange.Management.Sharing</span><span class="sxs-lookup"><span data-stu-id="2af03-143">Microsoft.Exchange.Management.Sharing</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Sharing.aspx)
    
- [<span data-ttu-id="2af03-144">Microsoft.Exchange.Management.StoreTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-144">Microsoft.Exchange.Management.StoreTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.StoreTasks.aspx)
    
- [<span data-ttu-id="2af03-145">Microsoft.Exchange.Management.Supervision</span><span class="sxs-lookup"><span data-stu-id="2af03-145">Microsoft.Exchange.Management.Supervision</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Supervision.aspx)
    
- [<span data-ttu-id="2af03-146">Microsoft.Exchange.Management.SystemConfigurationTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-146">Microsoft.Exchange.Management.SystemConfigurationTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.SystemConfigurationTasks.aspx)
    
- [<span data-ttu-id="2af03-147">Microsoft.Exchange.Management.Tasks</span><span class="sxs-lookup"><span data-stu-id="2af03-147">Microsoft.Exchange.Management.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tasks.aspx)
    
- [<span data-ttu-id="2af03-148">Microsoft.Exchange.Management.Tools</span><span class="sxs-lookup"><span data-stu-id="2af03-148">Microsoft.Exchange.Management.Tools</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tools.aspx)
    
- [<span data-ttu-id="2af03-149">Microsoft.Exchange.Management.Tracking</span><span class="sxs-lookup"><span data-stu-id="2af03-149">Microsoft.Exchange.Management.Tracking</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.Tracking.aspx)
    
- [<span data-ttu-id="2af03-150">Microsoft.Exchange.Management.TransportLogSearchTasks</span><span class="sxs-lookup"><span data-stu-id="2af03-150">Microsoft.Exchange.Management.TransportLogSearchTasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Management.TransportLogSearchTasks.aspx)
    
- [<span data-ttu-id="2af03-151">Microsoft.Exchange.MessagingPolicies.CompliancePrograms.Tasks</span><span class="sxs-lookup"><span data-stu-id="2af03-151">Microsoft.Exchange.MessagingPolicies.CompliancePrograms.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.CompliancePrograms.Tasks.aspx)
    
- [<span data-ttu-id="2af03-152">Microsoft.Exchange.MessagingPolicies.Journaling</span><span class="sxs-lookup"><span data-stu-id="2af03-152">Microsoft.Exchange.MessagingPolicies.Journaling</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.Journaling.aspx)
    
- [<span data-ttu-id="2af03-153">Microsoft.Exchange.MessagingPolicies.Rules.Tasks</span><span class="sxs-lookup"><span data-stu-id="2af03-153">Microsoft.Exchange.MessagingPolicies.Rules.Tasks</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.MessagingPolicies.Rules.Tasks.aspx)
    
- [<span data-ttu-id="2af03-154">Microsoft.Exchange.Migration</span><span class="sxs-lookup"><span data-stu-id="2af03-154">Microsoft.Exchange.Migration</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Migration.aspx)
    
- [<span data-ttu-id="2af03-155">Microsoft.Exchange.Monitoring</span><span class="sxs-lookup"><span data-stu-id="2af03-155">Microsoft.Exchange.Monitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Monitoring.aspx)
    
- [<span data-ttu-id="2af03-156">Microsoft.Exchange.Monitoring.ActiveMonitoring</span><span class="sxs-lookup"><span data-stu-id="2af03-156">Microsoft.Exchange.Monitoring.ActiveMonitoring</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Monitoring.ActiveMonitoring.aspx)
    
- [<span data-ttu-id="2af03-157">Microsoft.Exchange.Transport.Sync.Common.Subscription</span><span class="sxs-lookup"><span data-stu-id="2af03-157">Microsoft.Exchange.Transport.Sync.Common.Subscription</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.aspx)
    
- [<span data-ttu-id="2af03-158">Microsoft.Exchange.Transport.Sync.Common.Subscription.Connect</span><span class="sxs-lookup"><span data-stu-id="2af03-158">Microsoft.Exchange.Transport.Sync.Common.Subscription.Connect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Connect.aspx)
    
- [<span data-ttu-id="2af03-159">Microsoft.Exchange.Transport.Sync.Common.Subscription.DeltaSync</span><span class="sxs-lookup"><span data-stu-id="2af03-159">Microsoft.Exchange.Transport.Sync.Common.Subscription.DeltaSync</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.DeltaSync.aspx)
    
- [<span data-ttu-id="2af03-160">Microsoft.Exchange.Transport.Sync.Common.Subscription.Imap</span><span class="sxs-lookup"><span data-stu-id="2af03-160">Microsoft.Exchange.Transport.Sync.Common.Subscription.Imap</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Imap.aspx)
    
- [<span data-ttu-id="2af03-161">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pim</span><span class="sxs-lookup"><span data-stu-id="2af03-161">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pim</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Pim.aspx)
    
- [<span data-ttu-id="2af03-162">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pop</span><span class="sxs-lookup"><span data-stu-id="2af03-162">Microsoft.Exchange.Transport.Sync.Common.Subscription.Pop</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Transport.Sync.Common.Subscription.Pop.aspx)
    
- [<span data-ttu-id="2af03-163">Microsoft.Exchange.UM.Rpc</span><span class="sxs-lookup"><span data-stu-id="2af03-163">Microsoft.Exchange.UM.Rpc</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.UM.Rpc.aspx)
    
- [<span data-ttu-id="2af03-164">Microsoft.Exchange.UM.UMCommon</span><span class="sxs-lookup"><span data-stu-id="2af03-164">Microsoft.Exchange.UM.UMCommon</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.UM.UMCommon.aspx)
    
- [<span data-ttu-id="2af03-165">Microsoft.Exchange.WorkloadManagement</span><span class="sxs-lookup"><span data-stu-id="2af03-165">Microsoft.Exchange.WorkloadManagement</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.WorkloadManagement.aspx)
    
## <a name="see-also"></a><span data-ttu-id="2af03-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="2af03-166">See also</span></span>

- [<span data-ttu-id="2af03-167">Exchange 管理シェル</span><span class="sxs-lookup"><span data-stu-id="2af03-167">Exchange Management Shell</span></span>](exchange-management-shell.md)  
- [<span data-ttu-id="2af03-168">Exchange 管理シェルのツールを作成します。</span><span class="sxs-lookup"><span data-stu-id="2af03-168">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md) 
- [<span data-ttu-id="2af03-169">Exchange 管理シェル コマンドレットの入力と出力タイプ</span><span class="sxs-lookup"><span data-stu-id="2af03-169">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
    

