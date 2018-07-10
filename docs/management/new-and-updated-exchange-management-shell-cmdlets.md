---
title: 新規および更新された Exchange 管理シェル コマンドレット
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5941a439-94d2-4133-81fc-7240863a13df
description: Exchange の Exchange 管理シェルの新機能に関する情報を検索します。
ms.openlocfilehash: 906e078ab6d500a2cb3d364957ffc2fee67a06b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759240"
---
# <a name="new-and-updated-exchange-management-shell-cmdlets"></a><span data-ttu-id="ad049-103">新規および更新された Exchange 管理シェル コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-103">New and updated Exchange Management Shell cmdlets</span></span>

<span data-ttu-id="ad049-104">Exchange の Exchange 管理シェルの新機能に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="ad049-104">Find information about what's new in the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="ad049-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="ad049-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="ad049-106">この記事では、新しい Exchange 管理シェル コマンドレット、変更されたコマンドレットに関する情報を提供します。また、Exchange Online、Office 365 の一部としての Exchange Online、オンプレミスの Exchange から削除されたコマンドレットに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ad049-106">This article provides information about new Exchange Management shell cmdlets, cmdlets that were modified in, and cmdlets that were removed from Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange.</span></span>
  
## <a name="new-and-updated-cmdlets-in-exchange-2013-sp1"></a><span data-ttu-id="ad049-107">Exchange 2013 SP1 の新規コマンドレットと更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-107">New and updated cmdlets in Exchange 2013 SP1</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="ad049-108">新規コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-108">New cmdlets</span></span>

<span data-ttu-id="ad049-109">ビルド 15.00.0847.032 (Exchange Server 2013 SP1) で次のコマンドレットが導入されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-109">The following cmdlets were introduced in build 15.00.0847.032 (Exchange Server 2013 SP1):</span></span>
  
- <span data-ttu-id="ad049-110">**Get AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="ad049-110">**Get-AuthRedirect**</span></span>
    
- <span data-ttu-id="ad049-111">**新しい-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="ad049-111">**New-AuthRedirect**</span></span>
    
- <span data-ttu-id="ad049-112">**削除 AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="ad049-112">**Remove-AuthRedirect**</span></span>
    
- <span data-ttu-id="ad049-113">**セット AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="ad049-113">**Set-AuthRedirect**</span></span>
    
- <span data-ttu-id="ad049-114">**新しい-DataClassification**</span><span class="sxs-lookup"><span data-stu-id="ad049-114">**New-DataClassification**</span></span>
    
- <span data-ttu-id="ad049-115">**削除 DataClassification**</span><span class="sxs-lookup"><span data-stu-id="ad049-115">**Remove-DataClassification**</span></span>
    
- <span data-ttu-id="ad049-116">**セット DataClassification**</span><span class="sxs-lookup"><span data-stu-id="ad049-116">**Set-DataClassification**</span></span>
    
- <span data-ttu-id="ad049-117">**新しいフィンガー プリント**</span><span class="sxs-lookup"><span data-stu-id="ad049-117">**New-FingerPrint**</span></span>
    
- <span data-ttu-id="ad049-118">**Get MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="ad049-118">**Get-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="ad049-119">**新しい-MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="ad049-119">**New-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="ad049-120">**削除 MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="ad049-120">**Remove-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="ad049-121">**セット MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="ad049-121">**Set-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="ad049-122">**Get OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-122">**Get-OMEConfiguration**</span></span>
    
- <span data-ttu-id="ad049-123">**セット OMEConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-123">**Set-OMEConfiguration**</span></span>
    
- <span data-ttu-id="ad049-124">**Get SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-124">**Get-SmimeConfig**</span></span>
    
- <span data-ttu-id="ad049-125">**セット SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-125">**Set-SmimeConfig**</span></span>
    
- <span data-ttu-id="ad049-126">**Get IntraOrganizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-126">**Get-IntraOrganizationConfiguration**</span></span>
    
- <span data-ttu-id="ad049-127">**Get IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-127">**Get-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="ad049-128">**新しい-IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-128">**New-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="ad049-129">**削除 IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-129">**Remove-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="ad049-130">**セット IntraOrganizationConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-130">**Set-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="ad049-131">**Get HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-131">**Get-HistoricalSearch**</span></span>
    
- <span data-ttu-id="ad049-132">**開始 HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-132">**Start-HistoricalSearch**</span></span>
    
- <span data-ttu-id="ad049-133">**Stop HistoricalSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-133">**Stop-HistoricalSearch**</span></span>
    
- <span data-ttu-id="ad049-134">**新しい-SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="ad049-134">**New-SearchDocumentFormat**</span></span>
    
- <span data-ttu-id="ad049-135">**削除 SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="ad049-135">**Remove-SearchDocumentFormat**</span></span>
    
### <a name="updated-cmdlets"></a><span data-ttu-id="ad049-136">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-136">Updated cmdlets</span></span>

<span data-ttu-id="ad049-137">次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) で更新されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-137">The following cmdlets were updated in build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="ad049-138">**Get AuditLogSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-138">**Get-AuditLogSearch**</span></span>
    
- <span data-ttu-id="ad049-139">**Get QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="ad049-139">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="ad049-140">**新しい-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-140">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-141">**新しい-MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="ad049-141">**New-MailboxDatabase**</span></span>
    
- <span data-ttu-id="ad049-142">**新しい-PublicFolderMoveRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-142">**New-PublicFolderMoveRequest**</span></span>
    
- <span data-ttu-id="ad049-143">**新しい-TransportRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-143">**New-TransportRule**</span></span>
    
- <span data-ttu-id="ad049-144">**セット FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-144">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="ad049-145">**セット InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-145">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-146">**セット-メールボックス**</span><span class="sxs-lookup"><span data-stu-id="ad049-146">**Set-Mailbox**</span></span>
    
- <span data-ttu-id="ad049-147">**セット MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-147">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="ad049-148">**セット MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-148">**Set-MoveRequest**</span></span>
    
- <span data-ttu-id="ad049-149">**セット OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-149">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="ad049-150">**セット OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-150">**Set-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-151">**セット OwaVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="ad049-151">**Set-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="ad049-152">**セット組織**</span><span class="sxs-lookup"><span data-stu-id="ad049-152">**Set-TransportConfig**</span></span>
    
- <span data-ttu-id="ad049-153">**セット TransportRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-153">**Set-TransportRule**</span></span>
    
- <span data-ttu-id="ad049-154">**セット TransportServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-154">**Set-TransportServer**</span></span>
    
- <span data-ttu-id="ad049-155">**セット TransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-155">**Set-TransportService**</span></span>
    
- <span data-ttu-id="ad049-156">**テスト MRSHealth**</span><span class="sxs-lookup"><span data-stu-id="ad049-156">**Test-MRSHealth**</span></span>
    
- <span data-ttu-id="ad049-157">**テスト OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="ad049-157">**Test-OAuthConnectivity**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="ad049-158">削除されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-158">Removed cmdlets</span></span>

<span data-ttu-id="ad049-159">次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) から削除されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-159">The following cmdlets were removed from build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="ad049-160">**Get AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="ad049-160">**Get-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="ad049-161">**新しい-AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="ad049-161">**New-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="ad049-162">**削除 AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="ad049-162">**Remove-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="ad049-163">**セット AvailabilityReportOutage**</span><span class="sxs-lookup"><span data-stu-id="ad049-163">**Set-AvailabilityReportOutage**</span></span>
    
## <a name="new-and-updated-cmdlets-in-exchange-2013"></a><span data-ttu-id="ad049-164">Exchange 2013 の新規コマンドレットと更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-164">New and updated cmdlets in Exchange 2013</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="ad049-165">新規コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-165">New cmdlets</span></span>
<span data-ttu-id="ad049-166"><a name="bk_new"> </a></span><span class="sxs-lookup"><span data-stu-id="ad049-166"></span></span>

<span data-ttu-id="ad049-167">次のコマンドレットは、Exchange 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-167">The following cmdlets were introduced in Exchange 2013:</span></span>
  
- <span data-ttu-id="ad049-168">**Get ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="ad049-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="ad049-169">**セット ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="ad049-169">**Set-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="ad049-170">**無効にするアプリケーション**</span><span class="sxs-lookup"><span data-stu-id="ad049-170">**Disable-App**</span></span>
    
- <span data-ttu-id="ad049-171">**有効にするアプリケーション**</span><span class="sxs-lookup"><span data-stu-id="ad049-171">**Enable-App**</span></span>
    
- <span data-ttu-id="ad049-172">**取得アプリケーション**</span><span class="sxs-lookup"><span data-stu-id="ad049-172">**Get-App**</span></span>
    
- <span data-ttu-id="ad049-173">**新アプリ**</span><span class="sxs-lookup"><span data-stu-id="ad049-173">**New-App**</span></span>
    
- <span data-ttu-id="ad049-174">**削除アプリ**</span><span class="sxs-lookup"><span data-stu-id="ad049-174">**Remove-App**</span></span>
    
- <span data-ttu-id="ad049-175">**セット アプリケーション**</span><span class="sxs-lookup"><span data-stu-id="ad049-175">**Set-App**</span></span>
    
- <span data-ttu-id="ad049-176">**Get AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-176">**Get-AuthConfig**</span></span>
    
- <span data-ttu-id="ad049-177">**セット AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-177">**Set-AuthConfig**</span></span>
    
- <span data-ttu-id="ad049-178">**Get AuthServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-178">**Get-AuthServer**</span></span>
    
- <span data-ttu-id="ad049-179">**新しい-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-179">**New-AuthServer**</span></span>
    
- <span data-ttu-id="ad049-180">**削除 AuthServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-180">**Remove-AuthServer**</span></span>
    
- <span data-ttu-id="ad049-181">**セット AuthServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-181">**Set-AuthServer**</span></span>
    
- <span data-ttu-id="ad049-182">**新しい-AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-182">**New-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="ad049-183">**削除 AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-183">**Remove-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="ad049-184">**Get CalendarDiagnosticAnalysis**</span><span class="sxs-lookup"><span data-stu-id="ad049-184">**Get-CalendarDiagnosticAnalysis**</span></span>
    
- <span data-ttu-id="ad049-185">**Get ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-185">**Get-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="ad049-186">**新しい-ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-186">**New-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="ad049-187">**削除 ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-187">**Remove-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="ad049-188">**セット ClassificationRuleCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-188">**Set-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="ad049-189">**Get ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="ad049-189">**Get-ConnectSubscription**</span></span>
    
- <span data-ttu-id="ad049-190">**新しい-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="ad049-190">**New-ConnectSubscription**</span></span>
    
- <span data-ttu-id="ad049-191">**削除 ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="ad049-191">**Remove-ConnectSubscription**</span></span>
    
- <span data-ttu-id="ad049-192">**セット ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="ad049-192">**Set-ConnectSubscription**</span></span>
    
- <span data-ttu-id="ad049-193">**Get DataClassification**</span><span class="sxs-lookup"><span data-stu-id="ad049-193">**Get-DataClassification**</span></span>
    
- <span data-ttu-id="ad049-194">**Get DataClassificationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-194">**Get-DataClassificationConfig**</span></span>
    
- <span data-ttu-id="ad049-195">**Get DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-195">**Get-DlpPolicy**</span></span>
    
- <span data-ttu-id="ad049-196">**新しい-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-196">**New-DlpPolicy**</span></span>
    
- <span data-ttu-id="ad049-197">**削除 DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-197">**Remove-DlpPolicy**</span></span>
    
- <span data-ttu-id="ad049-198">**セット DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-198">**Set-DlpPolicy**</span></span>
    
- <span data-ttu-id="ad049-199">**エクスポート DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-199">**Export-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="ad049-200">**インポート-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="ad049-200">**Import-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="ad049-201">**Get DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="ad049-201">**Get-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="ad049-202">**インポート-DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="ad049-202">**Import-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="ad049-203">**削除 DlpPolicyTemplate**</span><span class="sxs-lookup"><span data-stu-id="ad049-203">**Remove-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="ad049-204">**Get ExchangeServerAccessLicense**</span><span class="sxs-lookup"><span data-stu-id="ad049-204">**Get-ExchangeServerAccessLicense**</span></span>
    
- <span data-ttu-id="ad049-205">**Get ExchangeServerAccessLicenseUser**</span><span class="sxs-lookup"><span data-stu-id="ad049-205">**Get-ExchangeServerAccessLicenseUser**</span></span>
    
- <span data-ttu-id="ad049-206">**Get FfoMigrationReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-206">**Get-FfoMigrationReport**</span></span>
    
- <span data-ttu-id="ad049-207">**Get FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-207">**Get-FrontendTransportService**</span></span>
    
- <span data-ttu-id="ad049-208">**セット FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-208">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="ad049-209">**追加 GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="ad049-209">**Add-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="ad049-210">**Get GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="ad049-210">**Get-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="ad049-211">**削除 GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="ad049-211">**Remove-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="ad049-212">**Get GroupActivityReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-212">**Get-GroupActivityReport**</span></span>
    
- <span data-ttu-id="ad049-213">**Get HealthReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-213">**Get-HealthReport**</span></span>
    
- <span data-ttu-id="ad049-214">**Get HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-214">**Get-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-215">**新しい-HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-215">**New-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-216">**削除 HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-216">**Remove-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-217">**セット HostedConnectionFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-217">**Set-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-218">**Get HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-218">**Get-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-219">**新しい-HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-219">**New-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-220">**削除 HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-220">**Remove-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-221">**セット HostedContentFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-221">**Set-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-222">**Get HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-222">**Get-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-223">**セット HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-223">**Set-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-224">**削除 HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-224">**Remove-HybridConfiguration**</span></span>
    
- <span data-ttu-id="ad049-225">**Get HybridMailflow**</span><span class="sxs-lookup"><span data-stu-id="ad049-225">**Get-HybridMailflow**</span></span>
    
- <span data-ttu-id="ad049-226">**セット HybridMailflow**</span><span class="sxs-lookup"><span data-stu-id="ad049-226">**Set-HybridMailflow**</span></span>
    
- <span data-ttu-id="ad049-227">**Get HybridMailflowDatacenterIPs**</span><span class="sxs-lookup"><span data-stu-id="ad049-227">**Get-HybridMailflowDatacenterIPs**</span></span>
    
- <span data-ttu-id="ad049-228">**Get InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-228">**Get-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-229">**新しい-InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-229">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-230">**削除 InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-230">**Remove-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-231">**セット InboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-231">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="ad049-232">**Get MailboxActivityReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-232">**Get-MailboxActivityReport**</span></span>
    
- <span data-ttu-id="ad049-233">**無効にする MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="ad049-233">**Disable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="ad049-234">**有効にする MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="ad049-234">**Enable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="ad049-235">**Get MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-235">**Get-MailboxTransportService**</span></span>
    
- <span data-ttu-id="ad049-236">**セット MailboxTransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-236">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="ad049-237">**Get MailDetailDlpPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-237">**Get-MailDetailDlpPolicyReport**</span></span>
    
- <span data-ttu-id="ad049-238">**Get MailDetailMalwareReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-238">**Get-MailDetailMalwareReport**</span></span>
    
- <span data-ttu-id="ad049-239">**Get MailDetailReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-239">**Get-MailDetailReport**</span></span>
    
- <span data-ttu-id="ad049-240">**Get MailDetailSpamReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-240">**Get-MailDetailSpamReport**</span></span>
    
- <span data-ttu-id="ad049-241">**Get MailDetailTransportRuleReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-241">**Get-MailDetailTransportRuleReport**</span></span>
    
- <span data-ttu-id="ad049-242">**Get MailFilterListReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-242">**Get-MailFilterListReport**</span></span>
    
- <span data-ttu-id="ad049-243">**Get MailTrafficPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-243">**Get-MailTrafficPolicyReport**</span></span>
    
- <span data-ttu-id="ad049-244">**Get MailTrafficReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-244">**Get-MailTrafficReport**</span></span>
    
- <span data-ttu-id="ad049-245">**Get MailTrafficSummaryReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-245">**Get-MailTrafficSummaryReport**</span></span>
    
- <span data-ttu-id="ad049-246">**Get MailTrafficTopReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-246">**Get-MailTrafficTopReport**</span></span>
    
- <span data-ttu-id="ad049-247">**Get MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-247">**Get-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="ad049-248">**セット MalwareFilteringServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-248">**Set-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="ad049-249">**Get MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-249">**Get-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-250">**新しい-MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-250">**New-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-251">**削除 MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-251">**Remove-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-252">**セット MalwareFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-252">**Set-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="ad049-253">**Get MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="ad049-253">**Get-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="ad049-254">**削除 MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="ad049-254">**Remove-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="ad049-255">**再開 MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="ad049-255">**Resume-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="ad049-256">**送信 MapiSubmitSystemProbe**</span><span class="sxs-lookup"><span data-stu-id="ad049-256">**Send-MapiSubmitSystemProbe**</span></span>
    
- <span data-ttu-id="ad049-257">**"リダイレクト"メッセージ**</span><span class="sxs-lookup"><span data-stu-id="ad049-257">**Redirect-Message**</span></span>
    
- <span data-ttu-id="ad049-258">**Get MessageTrace**</span><span class="sxs-lookup"><span data-stu-id="ad049-258">**Get-MessageTrace**</span></span>
    
- <span data-ttu-id="ad049-259">**Get MessageTraceDetail**</span><span class="sxs-lookup"><span data-stu-id="ad049-259">**Get-MessageTraceDetail**</span></span>
    
- <span data-ttu-id="ad049-260">**完了 MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="ad049-260">**Complete-MigrationBatch**</span></span>
    
- <span data-ttu-id="ad049-261">**削除 MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="ad049-261">**Remove-MigrationBatch**</span></span>
    
- <span data-ttu-id="ad049-262">**Get MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-262">**Get-MigrationConfig**</span></span>
    
- <span data-ttu-id="ad049-263">**セット MigrationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-263">**Set-MigrationConfig**</span></span>
    
- <span data-ttu-id="ad049-264">**Get MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="ad049-264">**Get-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="ad049-265">**新しい-MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="ad049-265">**New-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="ad049-266">**削除 MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="ad049-266">**Remove-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="ad049-267">**セット MigrationEndpoint**</span><span class="sxs-lookup"><span data-stu-id="ad049-267">**Set-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="ad049-268">**Get MigrationStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-268">**Get-MigrationStatistics**</span></span>
    
- <span data-ttu-id="ad049-269">**Get MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="ad049-269">**Get-MigrationUser**</span></span>
    
- <span data-ttu-id="ad049-270">**削除 MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="ad049-270">**Remove-MigrationUser**</span></span>
    
- <span data-ttu-id="ad049-271">**Get MigrationUserStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-271">**Get-MigrationUserStatistics**</span></span>
    
- <span data-ttu-id="ad049-272">**クリア MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="ad049-272">**Clear-MobileDevice**</span></span>
    
- <span data-ttu-id="ad049-273">**Get MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="ad049-273">**Get-MobileDevice**</span></span>
    
- <span data-ttu-id="ad049-274">**削除 MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="ad049-274">**Remove-MobileDevice**</span></span>
    
- <span data-ttu-id="ad049-275">**Get MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-275">**Get-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-276">**新しい-MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-276">**New-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-277">**削除 MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-277">**Remove-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-278">**セット MobileDeviceMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-278">**Set-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-279">**Get MobileDeviceStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-279">**Get-MobileDeviceStatistics**</span></span>
    
- <span data-ttu-id="ad049-280">**Get MonitoringItemHelp**</span><span class="sxs-lookup"><span data-stu-id="ad049-280">**Get-MonitoringItemHelp**</span></span>
    
- <span data-ttu-id="ad049-281">**Get MonitoringItemIdentity**</span><span class="sxs-lookup"><span data-stu-id="ad049-281">**Get-MonitoringItemIdentity**</span></span>
    
- <span data-ttu-id="ad049-282">**呼び出す MonitoringProbe**</span><span class="sxs-lookup"><span data-stu-id="ad049-282">**Invoke-MonitoringProbe**</span></span>
    
- <span data-ttu-id="ad049-283">**取得通知**</span><span class="sxs-lookup"><span data-stu-id="ad049-283">**Get-Notification**</span></span>
    
- <span data-ttu-id="ad049-284">**設定通知**</span><span class="sxs-lookup"><span data-stu-id="ad049-284">**Set-Notification**</span></span>
    
- <span data-ttu-id="ad049-285">**テスト OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="ad049-285">**Test-OAuthConnectivity**</span></span>
    
- <span data-ttu-id="ad049-286">**Get OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="ad049-286">**Get-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="ad049-287">**新しい-OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="ad049-287">**New-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="ad049-288">**削除 OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="ad049-288">**Remove-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="ad049-289">**セット OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="ad049-289">**Set-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="ad049-290">**有効にする OrganizationCustomization**</span><span class="sxs-lookup"><span data-stu-id="ad049-290">**Enable-OrganizationCustomization**</span></span>
    
- <span data-ttu-id="ad049-291">**Get OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-291">**Get-OutboundConnector**</span></span>
    
- <span data-ttu-id="ad049-292">**新しい-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-292">**New-OutboundConnector**</span></span>
    
- <span data-ttu-id="ad049-293">**削除 OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-293">**Remove-OutboundConnector**</span></span>
    
- <span data-ttu-id="ad049-294">**セット OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="ad049-294">**Set-OutboundConnector**</span></span>
    
- <span data-ttu-id="ad049-295">**Get PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-295">**Get-PartnerApplication**</span></span>
    
- <span data-ttu-id="ad049-296">**新しい-PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-296">**New-PartnerApplication**</span></span>
    
- <span data-ttu-id="ad049-297">**削除 PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-297">**Remove-PartnerApplication**</span></span>
    
- <span data-ttu-id="ad049-298">**セット PartnerApplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-298">**Set-PartnerApplication**</span></span>
    
- <span data-ttu-id="ad049-299">**Get PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="ad049-299">**Get-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="ad049-300">**セット PendingFederatedDomain**</span><span class="sxs-lookup"><span data-stu-id="ad049-300">**Set-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="ad049-301">**Get PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-301">**Get-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="ad049-302">**新しい-PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-302">**New-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="ad049-303">**削除 PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-303">**Remove-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="ad049-304">**セット PolicyTipConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-304">**Set-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="ad049-305">**ダンプ ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="ad049-305">**Dump-ProvisioningCache**</span></span>
    
- <span data-ttu-id="ad049-306">**リセット ProvisioningCache**</span><span class="sxs-lookup"><span data-stu-id="ad049-306">**Reset-ProvisioningCache**</span></span>
    
- <span data-ttu-id="ad049-307">**更新 PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-307">**Update-PublicFolderMailbox**</span></span>
    
- <span data-ttu-id="ad049-308">**Get PublicFolderMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="ad049-308">**Get-PublicFolderMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="ad049-309">**Get PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-309">**Get-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-310">**新しい-PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-310">**New-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-311">**削除 PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-311">**Remove-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-312">**再開 PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-312">**Resume-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-313">**セット PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-313">**Set-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-314">**中断 PublicFolderMigrationRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-314">**Suspend-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="ad049-315">**Get PublicFolderMigrationRequestStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-315">**Get-PublicFolderMigrationRequestStatistics**</span></span>
    
- <span data-ttu-id="ad049-316">**Get QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="ad049-316">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="ad049-317">**リリース QuarantineMessage**</span><span class="sxs-lookup"><span data-stu-id="ad049-317">**Release-QuarantineMessage**</span></span>
    
- <span data-ttu-id="ad049-318">**Get QueueDigest**</span><span class="sxs-lookup"><span data-stu-id="ad049-318">**Get-QueueDigest**</span></span>
    
- <span data-ttu-id="ad049-319">**Get ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-319">**Get-ResourcePolicy**</span></span>
    
- <span data-ttu-id="ad049-320">**新しい-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-320">**New-ResourcePolicy**</span></span>
    
- <span data-ttu-id="ad049-321">**削除 ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-321">**Remove-ResourcePolicy**</span></span>
    
- <span data-ttu-id="ad049-322">**セット ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-322">**Set-ResourcePolicy**</span></span>
    
- <span data-ttu-id="ad049-323">**追加 ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-323">**Add-ResubmitRequest**</span></span>
    
- <span data-ttu-id="ad049-324">**Get ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-324">**Get-ResubmitRequest**</span></span>
    
- <span data-ttu-id="ad049-325">**削除 ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-325">**Remove-ResubmitRequest**</span></span>
    
- <span data-ttu-id="ad049-326">**セット ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-326">**Set-ResubmitRequest**</span></span>
    
- <span data-ttu-id="ad049-327">**Get ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="ad049-327">**Get-ServerComponentState**</span></span>
    
- <span data-ttu-id="ad049-328">**セット ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="ad049-328">**Set-ServerComponentState**</span></span>
    
- <span data-ttu-id="ad049-329">**Get ServerHealth**</span><span class="sxs-lookup"><span data-stu-id="ad049-329">**Get-ServerHealth**</span></span>
    
- <span data-ttu-id="ad049-330">**セット ServerMonitor**</span><span class="sxs-lookup"><span data-stu-id="ad049-330">**Set-ServerMonitor**</span></span>
    
- <span data-ttu-id="ad049-331">**追加 ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="ad049-331">**Add-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="ad049-332">**Get ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="ad049-332">**Get-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="ad049-333">**Get SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-333">**Get-SiteMailbox**</span></span>
    
- <span data-ttu-id="ad049-334">**新しい-SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-334">**New-SiteMailbox**</span></span>
    
- <span data-ttu-id="ad049-335">**セット SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-335">**Set-SiteMailbox**</span></span>
    
- <span data-ttu-id="ad049-336">**テスト SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-336">**Test-SiteMailbox**</span></span>
    
- <span data-ttu-id="ad049-337">**更新 SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-337">**Update-SiteMailbox**</span></span>
    
- <span data-ttu-id="ad049-338">**Get SiteMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="ad049-338">**Get-SiteMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="ad049-339">**Get SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-339">**Get-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="ad049-340">**新しい-SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-340">**New-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="ad049-341">**削除 SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-341">**Remove-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="ad049-342">**セット SiteMailboxProvisioningPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-342">**Set-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="ad049-343">**[元に戻す-SoftDeletedMailbox**</span><span class="sxs-lookup"><span data-stu-id="ad049-343">**Undo-SoftDeletedMailbox**</span></span>
    
- <span data-ttu-id="ad049-344">**Get StaleMailboxDetailReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-344">**Get-StaleMailboxDetailReport**</span></span>
    
- <span data-ttu-id="ad049-345">**Get StaleMailboxReport**</span><span class="sxs-lookup"><span data-stu-id="ad049-345">**Get-StaleMailboxReport**</span></span>
    
- <span data-ttu-id="ad049-346">**更新 StoreMailboxState**</span><span class="sxs-lookup"><span data-stu-id="ad049-346">**Update-StoreMailboxState**</span></span>
    
- <span data-ttu-id="ad049-347">**新しい-SyncMailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="ad049-347">**New-SyncMailPublicFolder**</span></span>
    
- <span data-ttu-id="ad049-348">**Get TransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-348">**Get-TransportService**</span></span>
    
- <span data-ttu-id="ad049-349">**セット TransportService**</span><span class="sxs-lookup"><span data-stu-id="ad049-349">**Set-TransportService**</span></span>
    
- <span data-ttu-id="ad049-350">**無効にする UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-350">**Disable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-351">**有効にする UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-351">**Enable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-352">**Get UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-352">**Get-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-353">**新しい-UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-353">**New-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-354">**削除 UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-354">**Remove-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-355">**セット UMCallAnsweringRule**</span><span class="sxs-lookup"><span data-stu-id="ad049-355">**Set-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="ad049-356">**Get UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="ad049-356">**Get-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="ad049-357">**セット UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="ad049-357">**Set-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="ad049-358">**無効にする UMService**</span><span class="sxs-lookup"><span data-stu-id="ad049-358">**Disable-UMService**</span></span>
    
- <span data-ttu-id="ad049-359">**有効にする UMService**</span><span class="sxs-lookup"><span data-stu-id="ad049-359">**Enable-UMService**</span></span>
    
- <span data-ttu-id="ad049-360">**Get UMService**</span><span class="sxs-lookup"><span data-stu-id="ad049-360">**Get-UMService**</span></span>
    
- <span data-ttu-id="ad049-361">**セット UMService**</span><span class="sxs-lookup"><span data-stu-id="ad049-361">**Set-UMService**</span></span>
    
- <span data-ttu-id="ad049-362">**Get UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="ad049-362">**Get-UserPhoto**</span></span>
    
- <span data-ttu-id="ad049-363">**削除 UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="ad049-363">**Remove-UserPhoto**</span></span>
    
- <span data-ttu-id="ad049-364">**セット UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="ad049-364">**Set-UserPhoto**</span></span>
    
- <span data-ttu-id="ad049-365">**Get WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-365">**Get-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="ad049-366">**新しい-WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-366">**New-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="ad049-367">**削除 WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-367">**Remove-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="ad049-368">**Get WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-368">**Get-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="ad049-369">**新しい-WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-369">**New-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="ad049-370">**削除 WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-370">**Remove-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="ad049-371">**セット WorkloadPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-371">**Set-WorkloadPolicy**</span></span>
    
### <a name="modified-cmdlets"></a><span data-ttu-id="ad049-372">変更されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-372">Modified cmdlets</span></span>
<span data-ttu-id="ad049-373"><a name="bk_update"> </a></span><span class="sxs-lookup"><span data-stu-id="ad049-373"></span></span>

<span data-ttu-id="ad049-374">Exchange 2013 では、次のコマンドレットの入力または出力の種類が変更されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-374">The input or output types for following cmdlets were modified in Exchange 2013:</span></span>
  
- <span data-ttu-id="ad049-375">**クリア ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="ad049-375">**Clear-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="ad049-376">**削除 ActiveSyncDevice**</span><span class="sxs-lookup"><span data-stu-id="ad049-376">**Remove-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="ad049-377">**Get ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-377">**Get-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-378">**新しい-ActiveSyncMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-378">**New-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-379">**新しい-ActiveSyncVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="ad049-379">**New-ActiveSyncVirtualDirectory**</span></span>
    
- <span data-ttu-id="ad049-380">**新しい-AutodiscoverVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="ad049-380">**New-AutodiscoverVirtualDirectory**</span></span>
    
- <span data-ttu-id="ad049-381">**セット AvailabilityConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-381">**Set-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="ad049-382">**有効にする ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="ad049-382">**Enable-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="ad049-383">**エクスポート ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="ad049-383">**Export-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="ad049-384">**します**</span><span class="sxs-lookup"><span data-stu-id="ad049-384">**Import-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="ad049-385">**削除 ExchangeCertificate**</span><span class="sxs-lookup"><span data-stu-id="ad049-385">**Remove-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="ad049-386">**Get FailedContentIndexDocuments**</span><span class="sxs-lookup"><span data-stu-id="ad049-386">**Get-FailedContentIndexDocuments**</span></span>
    
- <span data-ttu-id="ad049-387">**Get FederationInformation**</span><span class="sxs-lookup"><span data-stu-id="ad049-387">**Get-FederationInformation**</span></span>
    
- <span data-ttu-id="ad049-388">**新しい-HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-388">**New-HybridConfiguration**</span></span>
    
- <span data-ttu-id="ad049-389">**セット HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="ad049-389">**Set-HybridConfiguration**</span></span>
    
- <span data-ttu-id="ad049-390">**新しいメールボックス**</span><span class="sxs-lookup"><span data-stu-id="ad049-390">**New-Mailbox**</span></span>
    
- <span data-ttu-id="ad049-391">**再開 MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="ad049-391">**Resume-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="ad049-392">**セット MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="ad049-392">**Set-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="ad049-393">**中断 MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="ad049-393">**Suspend-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="ad049-394">**更新 MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="ad049-394">**Update-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="ad049-395">**Get MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-395">**Get-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="ad049-396">**セット MailboxExportRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-396">**Set-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="ad049-397">**追加 MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-397">**Add-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="ad049-398">**削除 MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-398">**Remove-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="ad049-399">**セット MailboxFolderPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-399">**Set-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="ad049-400">**Get MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-400">**Get-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="ad049-401">**セット MailboxImportRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-401">**Set-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="ad049-402">**Get MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-402">**Get-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="ad049-403">**セット MailboxRestoreRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-403">**Set-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="ad049-404">**Get MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-404">**Get-MailboxSearch**</span></span>
    
- <span data-ttu-id="ad049-405">**削除 MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-405">**Remove-MailboxSearch**</span></span>
    
- <span data-ttu-id="ad049-406">**セット MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-406">**Set-MailboxSearch**</span></span>
    
- <span data-ttu-id="ad049-407">**開始 MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-407">**Start-MailboxSearch**</span></span>
    
- <span data-ttu-id="ad049-408">**Stop MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="ad049-408">**Stop-MailboxSearch**</span></span>
    
- <span data-ttu-id="ad049-409">**無効にする MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="ad049-409">**Disable-MailPublicFolder**</span></span>
    
- <span data-ttu-id="ad049-410">**Get MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="ad049-410">**Get-MailPublicFolder**</span></span>
    
- <span data-ttu-id="ad049-411">**セット MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="ad049-411">**Set-MailPublicFolder**</span></span>
    
- <span data-ttu-id="ad049-412">**Get MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="ad049-412">**Get-MigrationBatch**</span></span>
    
- <span data-ttu-id="ad049-413">**新しい-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="ad049-413">**New-MigrationBatch**</span></span>
    
- <span data-ttu-id="ad049-414">**セット MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="ad049-414">**Set-MigrationBatch**</span></span>
    
- <span data-ttu-id="ad049-415">**テスト MigrationServerAvailability**</span><span class="sxs-lookup"><span data-stu-id="ad049-415">**Test-MigrationServerAvailability**</span></span>
    
- <span data-ttu-id="ad049-416">**Get MoveRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-416">**Get-MoveRequest**</span></span>
    
- <span data-ttu-id="ad049-417">**新しい-OfflineAddressBook**</span><span class="sxs-lookup"><span data-stu-id="ad049-417">**New-OfflineAddressBook**</span></span>
    
- <span data-ttu-id="ad049-418">**Get OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-418">**Get-OrganizationConfig**</span></span>
    
- <span data-ttu-id="ad049-419">**セット OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="ad049-419">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="ad049-420">**テスト OutlookConnectivity**</span><span class="sxs-lookup"><span data-stu-id="ad049-420">**Test-OutlookConnectivity**</span></span>
    
- <span data-ttu-id="ad049-421">**テスト OutlookWebServices**</span><span class="sxs-lookup"><span data-stu-id="ad049-421">**Test-OutlookWebServices**</span></span>
    
- <span data-ttu-id="ad049-422">**Get OwaMailboxPolicy**</span><span class="sxs-lookup"><span data-stu-id="ad049-422">**Get-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="ad049-423">**OwaVirtualDirectory で新しい**</span><span class="sxs-lookup"><span data-stu-id="ad049-423">**New-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="ad049-424">**新しい-PowerShellVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="ad049-424">**New-PowerShellVirtualDirectory**</span></span>
    
- <span data-ttu-id="ad049-425">**パブリック フォルダーの取得**</span><span class="sxs-lookup"><span data-stu-id="ad049-425">**Get-PublicFolder**</span></span>
    
- <span data-ttu-id="ad049-426">**新しいパブリック フォルダー**</span><span class="sxs-lookup"><span data-stu-id="ad049-426">**New-PublicFolder**</span></span>
    
- <span data-ttu-id="ad049-427">**パブリック フォルダーの設定**</span><span class="sxs-lookup"><span data-stu-id="ad049-427">**Set-PublicFolder**</span></span>
    
- <span data-ttu-id="ad049-428">**追加 PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-428">**Add-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="ad049-429">**Get PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-429">**Get-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="ad049-430">**削除 PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-430">**Remove-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="ad049-431">**Get PublicFolderItemStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-431">**Get-PublicFolderItemStatistics**</span></span>
    
- <span data-ttu-id="ad049-432">**Get PublicFolderStatistics**</span><span class="sxs-lookup"><span data-stu-id="ad049-432">**Get-PublicFolderStatistics**</span></span>
    
- <span data-ttu-id="ad049-433">**受信者の取得**</span><span class="sxs-lookup"><span data-stu-id="ad049-433">**Get-Recipient**</span></span>
    
- <span data-ttu-id="ad049-434">**Resourceconfig とのセット**</span><span class="sxs-lookup"><span data-stu-id="ad049-434">**Set-ResourceConfig**</span></span>
    
- <span data-ttu-id="ad049-435">**テスト WebServicesConnectivity**</span><span class="sxs-lookup"><span data-stu-id="ad049-435">**Test-WebServicesConnectivity**</span></span>
    
- <span data-ttu-id="ad049-436">**新しい-WebServicesVirtualDirectory**</span><span class="sxs-lookup"><span data-stu-id="ad049-436">**New-WebServicesVirtualDirectory**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="ad049-437">削除されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-437">Removed cmdlets</span></span>
<span data-ttu-id="ad049-438"><a name="bk_removed"> </a></span><span class="sxs-lookup"><span data-stu-id="ad049-438"></span></span>

<span data-ttu-id="ad049-439">次のコマンドレットは、Exchange 2013 から削除されました。</span><span class="sxs-lookup"><span data-stu-id="ad049-439">The following cmdlets were removed from Exchange 2013:</span></span>
  
- <span data-ttu-id="ad049-440">**更新 FileDistributionService**</span><span class="sxs-lookup"><span data-stu-id="ad049-440">**Update-FileDistributionService**</span></span>
    
- <span data-ttu-id="ad049-441">**復元メールボックス**</span><span class="sxs-lookup"><span data-stu-id="ad049-441">**Restore-Mailbox**</span></span>
    
- <span data-ttu-id="ad049-442">**クリーニング MailboxDatabase**</span><span class="sxs-lookup"><span data-stu-id="ad049-442">**Clean-MailboxDatabase**</span></span>
    
- <span data-ttu-id="ad049-443">**移行が完了**</span><span class="sxs-lookup"><span data-stu-id="ad049-443">**Complete-Migration**</span></span>
    
- <span data-ttu-id="ad049-444">**Get MigrationStatus**</span><span class="sxs-lookup"><span data-stu-id="ad049-444">**Get-MigrationStatus**</span></span>
    
- <span data-ttu-id="ad049-445">**パブリック フォルダーの更新**</span><span class="sxs-lookup"><span data-stu-id="ad049-445">**Update-PublicFolder**</span></span>
    
- <span data-ttu-id="ad049-446">**追加 PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-446">**Add-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="ad049-447">**Get PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-447">**Get-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="ad049-448">**削除 PublicFolderAdministrativePermission**</span><span class="sxs-lookup"><span data-stu-id="ad049-448">**Remove-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="ad049-449">**新しい-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="ad049-449">**New-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="ad049-450">**削除 PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="ad049-450">**Remove-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="ad049-451">**セット PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="ad049-451">**Set-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="ad049-452">**新しい-PublicFolderDatabaseRepairRequest**</span><span class="sxs-lookup"><span data-stu-id="ad049-452">**New-PublicFolderDatabaseRepairRequest**</span></span>
    
- <span data-ttu-id="ad049-453">**更新 PublicFolderHierarchy**</span><span class="sxs-lookup"><span data-stu-id="ad049-453">**Update-PublicFolderHierarchy**</span></span>
    
- <span data-ttu-id="ad049-454">**再開 PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-454">**Resume-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="ad049-455">**中断 PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="ad049-455">**Suspend-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="ad049-456">**開始 RetentionAutoTagLearning**</span><span class="sxs-lookup"><span data-stu-id="ad049-456">**Start-RetentionAutoTagLearning**</span></span>
    
- <span data-ttu-id="ad049-457">**テスト SystemHealth**</span><span class="sxs-lookup"><span data-stu-id="ad049-457">**Test-SystemHealth**</span></span>
    
- <span data-ttu-id="ad049-458">**無効にする UMServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-458">**Disable-UMServer**</span></span>
    
- <span data-ttu-id="ad049-459">**有効にする UMServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-459">**Enable-UMServer**</span></span>
    
- <span data-ttu-id="ad049-460">**Get UMServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-460">**Get-UMServer**</span></span>
    
- <span data-ttu-id="ad049-461">**セット UMServer**</span><span class="sxs-lookup"><span data-stu-id="ad049-461">**Set-UMServer**</span></span>
    
## <a name="see-also"></a><span data-ttu-id="ad049-462">関連項目</span><span class="sxs-lookup"><span data-stu-id="ad049-462">See also</span></span>

- [<span data-ttu-id="ad049-463">Exchange 管理シェル コマンドレットの入力と出力タイプ</span><span class="sxs-lookup"><span data-stu-id="ad049-463">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)    
- [<span data-ttu-id="ad049-464">Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad049-464">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)    
- [<span data-ttu-id="ad049-465">Exchange 2013 コマンドレット</span><span class="sxs-lookup"><span data-stu-id="ad049-465">Exchange 2013 cmdlets</span></span>](http://technet.microsoft.com/ja-jp/library/bb124413%28v=exchg.150%29.aspx)
    

