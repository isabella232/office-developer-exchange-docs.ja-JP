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
ms.openlocfilehash: bda6607be20f2a21bc22d472d63615d46634d8ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457145"
---
# <a name="new-and-updated-exchange-management-shell-cmdlets"></a><span data-ttu-id="46d34-103">新規および更新された Exchange 管理シェル コマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-103">New and updated Exchange Management Shell cmdlets</span></span>

<span data-ttu-id="46d34-104">Exchange の Exchange 管理シェルの新機能に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="46d34-104">Find information about what's new in the Exchange Management Shell in Exchange.</span></span>
  
<span data-ttu-id="46d34-105">**適用対象:** Exchange Online |Exchange Server 2013 |Office 365</span><span class="sxs-lookup"><span data-stu-id="46d34-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="46d34-106">この記事では、新しい Exchange 管理シェル コマンドレット、変更されたコマンドレットに関する情報を提供します。また、Exchange Online、Office 365 の一部としての Exchange Online、オンプレミスの Exchange から削除されたコマンドレットに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="46d34-106">This article provides information about new Exchange Management shell cmdlets, cmdlets that were modified in, and cmdlets that were removed from Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange.</span></span>
  
## <a name="new-and-updated-cmdlets-in-exchange-2013-sp1"></a><span data-ttu-id="46d34-107">Exchange 2013 SP1 の新規コマンドレットと更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-107">New and updated cmdlets in Exchange 2013 SP1</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="46d34-108">新規コマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-108">New cmdlets</span></span>

<span data-ttu-id="46d34-109">ビルド 15.00.0847.032 (Exchange Server 2013 SP1) で次のコマンドレットが導入されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-109">The following cmdlets were introduced in build 15.00.0847.032 (Exchange Server 2013 SP1):</span></span>
  
- <span data-ttu-id="46d34-110">**取得-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="46d34-110">**Get-AuthRedirect**</span></span>
    
- <span data-ttu-id="46d34-111">**New-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="46d34-111">**New-AuthRedirect**</span></span>
    
- <span data-ttu-id="46d34-112">**削除-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="46d34-112">**Remove-AuthRedirect**</span></span>
    
- <span data-ttu-id="46d34-113">**Set-AuthRedirect**</span><span class="sxs-lookup"><span data-stu-id="46d34-113">**Set-AuthRedirect**</span></span>
    
- <span data-ttu-id="46d34-114">**新しい-Datacl/認定**</span><span class="sxs-lookup"><span data-stu-id="46d34-114">**New-DataClassification**</span></span>
    
- <span data-ttu-id="46d34-115">**削除-Datacl/認定**</span><span class="sxs-lookup"><span data-stu-id="46d34-115">**Remove-DataClassification**</span></span>
    
- <span data-ttu-id="46d34-116">**Set-Datacl/認定**</span><span class="sxs-lookup"><span data-stu-id="46d34-116">**Set-DataClassification**</span></span>
    
- <span data-ttu-id="46d34-117">**新規-指紋**</span><span class="sxs-lookup"><span data-stu-id="46d34-117">**New-FingerPrint**</span></span>
    
- <span data-ttu-id="46d34-118">**MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="46d34-118">**Get-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="46d34-119">**MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="46d34-119">**New-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="46d34-120">**MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="46d34-120">**Remove-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="46d34-121">**MapiVirtualDirectory\***</span><span class="sxs-lookup"><span data-stu-id="46d34-121">**Set-MapiVirtualDirectory\***</span></span>
    
- <span data-ttu-id="46d34-122">**取得-OMEConfiguration 低**</span><span class="sxs-lookup"><span data-stu-id="46d34-122">**Get-OMEConfiguration**</span></span>
    
- <span data-ttu-id="46d34-123">**設定-OMEConfiguration 設定**</span><span class="sxs-lookup"><span data-stu-id="46d34-123">**Set-OMEConfiguration**</span></span>
    
- <span data-ttu-id="46d34-124">**Get-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-124">**Get-SmimeConfig**</span></span>
    
- <span data-ttu-id="46d34-125">**Set-SmimeConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-125">**Set-SmimeConfig**</span></span>
    
- <span data-ttu-id="46d34-126">**Get-intraorganizationconfiguration**</span><span class="sxs-lookup"><span data-stu-id="46d34-126">**Get-IntraOrganizationConfiguration**</span></span>
    
- <span data-ttu-id="46d34-127">**New-intraorganizationconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-127">**Get-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="46d34-128">**New-intraorganizationconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-128">**New-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="46d34-129">**New-intraorganizationconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-129">**Remove-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="46d34-130">**New-intraorganizationconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-130">**Set-IntraOrganizationConnector**</span></span>
    
- <span data-ttu-id="46d34-131">**Start-historicalsearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-131">**Get-HistoricalSearch**</span></span>
    
- <span data-ttu-id="46d34-132">**Start-historicalsearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-132">**Start-HistoricalSearch**</span></span>
    
- <span data-ttu-id="46d34-133">**Start-historicalsearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-133">**Stop-HistoricalSearch**</span></span>
    
- <span data-ttu-id="46d34-134">**新しい-SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="46d34-134">**New-SearchDocumentFormat**</span></span>
    
- <span data-ttu-id="46d34-135">**削除-SearchDocumentFormat**</span><span class="sxs-lookup"><span data-stu-id="46d34-135">**Remove-SearchDocumentFormat**</span></span>
    
### <a name="updated-cmdlets"></a><span data-ttu-id="46d34-136">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-136">Updated cmdlets</span></span>

<span data-ttu-id="46d34-137">次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) で更新されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-137">The following cmdlets were updated in build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="46d34-138">**取得-AuditLogSearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-138">**Get-AuditLogSearch**</span></span>
    
- <span data-ttu-id="46d34-139">**Get-quarantinemessage**</span><span class="sxs-lookup"><span data-stu-id="46d34-139">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="46d34-140">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-140">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-141">**Set-mailboxdatabase**</span><span class="sxs-lookup"><span data-stu-id="46d34-141">**New-MailboxDatabase**</span></span>
    
- <span data-ttu-id="46d34-142">**Get-publicfoldermoverequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-142">**New-PublicFolderMoveRequest**</span></span>
    
- <span data-ttu-id="46d34-143">**New-transportrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-143">**New-TransportRule**</span></span>
    
- <span data-ttu-id="46d34-144">**Set-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-144">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="46d34-145">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-145">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-146">**Set-Mailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-146">**Set-Mailbox**</span></span>
    
- <span data-ttu-id="46d34-147">**Set-mailboxtransportservice**</span><span class="sxs-lookup"><span data-stu-id="46d34-147">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="46d34-148">**New-moverequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-148">**Set-MoveRequest**</span></span>
    
- <span data-ttu-id="46d34-149">**Set-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-149">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="46d34-150">**セット-Owam/Boxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-150">**Set-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-151">**Set-owavirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-151">**Set-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="46d34-152">**設定-TransportConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-152">**Set-TransportConfig**</span></span>
    
- <span data-ttu-id="46d34-153">**New-transportrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-153">**Set-TransportRule**</span></span>
    
- <span data-ttu-id="46d34-154">**Set-TransportServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-154">**Set-TransportServer**</span></span>
    
- <span data-ttu-id="46d34-155">**Set-TransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-155">**Set-TransportService**</span></span>
    
- <span data-ttu-id="46d34-156">**Test-MRSHealth**</span><span class="sxs-lookup"><span data-stu-id="46d34-156">**Test-MRSHealth**</span></span>
    
- <span data-ttu-id="46d34-157">**テスト-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="46d34-157">**Test-OAuthConnectivity**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="46d34-158">削除されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-158">Removed cmdlets</span></span>

<span data-ttu-id="46d34-159">次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) から削除されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-159">The following cmdlets were removed from build 15.00.0847.032 (Exchange 2013 SP1):</span></span>
  
- <span data-ttu-id="46d34-160">**New-availabilityreportoutage**</span><span class="sxs-lookup"><span data-stu-id="46d34-160">**Get-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="46d34-161">**New-availabilityreportoutage**</span><span class="sxs-lookup"><span data-stu-id="46d34-161">**New-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="46d34-162">**New-availabilityreportoutage**</span><span class="sxs-lookup"><span data-stu-id="46d34-162">**Remove-AvailabilityReportOutage**</span></span>
    
- <span data-ttu-id="46d34-163">**New-availabilityreportoutage**</span><span class="sxs-lookup"><span data-stu-id="46d34-163">**Set-AvailabilityReportOutage**</span></span>
    
## <a name="new-and-updated-cmdlets-in-exchange-2013"></a><span data-ttu-id="46d34-164">Exchange 2013 の新規コマンドレットと更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-164">New and updated cmdlets in Exchange 2013</span></span>

### <a name="new-cmdlets"></a><span data-ttu-id="46d34-165">新規コマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-165">New cmdlets</span></span>
<span data-ttu-id="46d34-166"><a name="bk_new"> </a></span><span class="sxs-lookup"><span data-stu-id="46d34-166"><a name="bk_new"> </a></span></span>

<span data-ttu-id="46d34-167">次のコマンドレットが Exchange 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-167">The following cmdlets were introduced in Exchange 2013:</span></span>
  
- <span data-ttu-id="46d34-168">**ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="46d34-168">**Get-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="46d34-169">**ActiveSyncDeviceAutoblockThreshold**</span><span class="sxs-lookup"><span data-stu-id="46d34-169">**Set-ActiveSyncDeviceAutoblockThreshold**</span></span>
    
- <span data-ttu-id="46d34-170">**Disable-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-170">**Disable-App**</span></span>
    
- <span data-ttu-id="46d34-171">**Enable-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-171">**Enable-App**</span></span>
    
- <span data-ttu-id="46d34-172">**Get-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-172">**Get-App**</span></span>
    
- <span data-ttu-id="46d34-173">**New-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-173">**New-App**</span></span>
    
- <span data-ttu-id="46d34-174">**Remove-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-174">**Remove-App**</span></span>
    
- <span data-ttu-id="46d34-175">**Set-App**</span><span class="sxs-lookup"><span data-stu-id="46d34-175">**Set-App**</span></span>
    
- <span data-ttu-id="46d34-176">**取得-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-176">**Get-AuthConfig**</span></span>
    
- <span data-ttu-id="46d34-177">**設定-AuthConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-177">**Set-AuthConfig**</span></span>
    
- <span data-ttu-id="46d34-178">**取得-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-178">**Get-AuthServer**</span></span>
    
- <span data-ttu-id="46d34-179">**新しい-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-179">**New-AuthServer**</span></span>
    
- <span data-ttu-id="46d34-180">**削除-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-180">**Remove-AuthServer**</span></span>
    
- <span data-ttu-id="46d34-181">**Set-AuthServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-181">**Set-AuthServer**</span></span>
    
- <span data-ttu-id="46d34-182">**Get-availabilityconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-182">**New-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="46d34-183">**Get-availabilityconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-183">**Remove-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="46d34-184">**CalendarDiagnosticAnalysis**</span><span class="sxs-lookup"><span data-stu-id="46d34-184">**Get-CalendarDiagnosticAnalysis**</span></span>
    
- <span data-ttu-id="46d34-185">**Get-classificationrulecollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-185">**Get-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="46d34-186">**Get-classificationrulecollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-186">**New-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="46d34-187">**Get-classificationrulecollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-187">**Remove-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="46d34-188">**Get-classificationrulecollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-188">**Set-ClassificationRuleCollection**</span></span>
    
- <span data-ttu-id="46d34-189">**取得-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="46d34-189">**Get-ConnectSubscription**</span></span>
    
- <span data-ttu-id="46d34-190">**新しい-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="46d34-190">**New-ConnectSubscription**</span></span>
    
- <span data-ttu-id="46d34-191">**削除-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="46d34-191">**Remove-ConnectSubscription**</span></span>
    
- <span data-ttu-id="46d34-192">**設定-ConnectSubscription**</span><span class="sxs-lookup"><span data-stu-id="46d34-192">**Set-ConnectSubscription**</span></span>
    
- <span data-ttu-id="46d34-193">**取得-Datacl/確認**</span><span class="sxs-lookup"><span data-stu-id="46d34-193">**Get-DataClassification**</span></span>
    
- <span data-ttu-id="46d34-194">**Get-dataclassificationconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-194">**Get-DataClassificationConfig**</span></span>
    
- <span data-ttu-id="46d34-195">**取得-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-195">**Get-DlpPolicy**</span></span>
    
- <span data-ttu-id="46d34-196">**新-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-196">**New-DlpPolicy**</span></span>
    
- <span data-ttu-id="46d34-197">**削除-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-197">**Remove-DlpPolicy**</span></span>
    
- <span data-ttu-id="46d34-198">**設定-DlpPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-198">**Set-DlpPolicy**</span></span>
    
- <span data-ttu-id="46d34-199">**Export-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-199">**Export-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="46d34-200">**Import-DlpPolicyCollection**</span><span class="sxs-lookup"><span data-stu-id="46d34-200">**Import-DlpPolicyCollection**</span></span>
    
- <span data-ttu-id="46d34-201">**Remove-dlppolicytemplate**</span><span class="sxs-lookup"><span data-stu-id="46d34-201">**Get-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="46d34-202">**Remove-dlppolicytemplate**</span><span class="sxs-lookup"><span data-stu-id="46d34-202">**Import-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="46d34-203">**Remove-dlppolicytemplate**</span><span class="sxs-lookup"><span data-stu-id="46d34-203">**Remove-DlpPolicyTemplate**</span></span>
    
- <span data-ttu-id="46d34-204">**ExchangeServerAccessLicense**</span><span class="sxs-lookup"><span data-stu-id="46d34-204">**Get-ExchangeServerAccessLicense**</span></span>
    
- <span data-ttu-id="46d34-205">**ExchangeServerAccessLicenseUser**</span><span class="sxs-lookup"><span data-stu-id="46d34-205">**Get-ExchangeServerAccessLicenseUser**</span></span>
    
- <span data-ttu-id="46d34-206">**FfoMigrationReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-206">**Get-FfoMigrationReport**</span></span>
    
- <span data-ttu-id="46d34-207">**Get-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-207">**Get-FrontendTransportService**</span></span>
    
- <span data-ttu-id="46d34-208">**Set-FrontendTransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-208">**Set-FrontendTransportService**</span></span>
    
- <span data-ttu-id="46d34-209">**追加-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="46d34-209">**Add-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="46d34-210">**取得-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="46d34-210">**Get-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="46d34-211">**削除-GlobalMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="46d34-211">**Remove-GlobalMonitoringOverride**</span></span>
    
- <span data-ttu-id="46d34-212">**Get-GroupActivityReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-212">**Get-GroupActivityReport**</span></span>
    
- <span data-ttu-id="46d34-213">**HealthReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-213">**Get-HealthReport**</span></span>
    
- <span data-ttu-id="46d34-214">**Remove-hostedconnectionfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-214">**Get-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-215">**Remove-hostedconnectionfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-215">**New-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-216">**Remove-hostedconnectionfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-216">**Remove-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-217">**Remove-hostedconnectionfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-217">**Set-HostedConnectionFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-218">**Set-hostedcontentfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-218">**Get-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-219">**Set-hostedcontentfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-219">**New-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-220">**Set-hostedcontentfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-220">**Remove-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-221">**Set-hostedcontentfilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-221">**Set-HostedContentFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-222">**HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-222">**Get-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-223">**HostedOutboundSpamFilterPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-223">**Set-HostedOutboundSpamFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-224">**HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="46d34-224">**Remove-HybridConfiguration**</span></span>
    
- <span data-ttu-id="46d34-225">**Get-hybridmailflow**</span><span class="sxs-lookup"><span data-stu-id="46d34-225">**Get-HybridMailflow**</span></span>
    
- <span data-ttu-id="46d34-226">**Get-hybridmailflow**</span><span class="sxs-lookup"><span data-stu-id="46d34-226">**Set-HybridMailflow**</span></span>
    
- <span data-ttu-id="46d34-227">**HybridMailflowDatacenterIPs**</span><span class="sxs-lookup"><span data-stu-id="46d34-227">**Get-HybridMailflowDatacenterIPs**</span></span>
    
- <span data-ttu-id="46d34-228">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-228">**Get-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-229">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-229">**New-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-230">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-230">**Remove-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-231">**New-inboundconnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-231">**Set-InboundConnector**</span></span>
    
- <span data-ttu-id="46d34-232">**Get-mailboxactivityreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-232">**Get-MailboxActivityReport**</span></span>
    
- <span data-ttu-id="46d34-233">**MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="46d34-233">**Disable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="46d34-234">**MailboxQuarantine**</span><span class="sxs-lookup"><span data-stu-id="46d34-234">**Enable-MailboxQuarantine**</span></span>
    
- <span data-ttu-id="46d34-235">**Set-mailboxtransportservice**</span><span class="sxs-lookup"><span data-stu-id="46d34-235">**Get-MailboxTransportService**</span></span>
    
- <span data-ttu-id="46d34-236">**Set-mailboxtransportservice**</span><span class="sxs-lookup"><span data-stu-id="46d34-236">**Set-MailboxTransportService**</span></span>
    
- <span data-ttu-id="46d34-237">**Get-MailDetailDlpPolicyReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-237">**Get-MailDetailDlpPolicyReport**</span></span>
    
- <span data-ttu-id="46d34-238">**Get-maildetailmalwarereport**</span><span class="sxs-lookup"><span data-stu-id="46d34-238">**Get-MailDetailMalwareReport**</span></span>
    
- <span data-ttu-id="46d34-239">**取得-MailDetailReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-239">**Get-MailDetailReport**</span></span>
    
- <span data-ttu-id="46d34-240">**Get-maildetailspamreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-240">**Get-MailDetailSpamReport**</span></span>
    
- <span data-ttu-id="46d34-241">**Get-maildetailtransportrulereport**</span><span class="sxs-lookup"><span data-stu-id="46d34-241">**Get-MailDetailTransportRuleReport**</span></span>
    
- <span data-ttu-id="46d34-242">**Get-MailFilterListReport**</span><span class="sxs-lookup"><span data-stu-id="46d34-242">**Get-MailFilterListReport**</span></span>
    
- <span data-ttu-id="46d34-243">**Get-mailtrafficpolicyreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-243">**Get-MailTrafficPolicyReport**</span></span>
    
- <span data-ttu-id="46d34-244">**Get-mailtrafficreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-244">**Get-MailTrafficReport**</span></span>
    
- <span data-ttu-id="46d34-245">**Get-mailtrafficsummaryreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-245">**Get-MailTrafficSummaryReport**</span></span>
    
- <span data-ttu-id="46d34-246">**Get-mailtraffictopreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-246">**Get-MailTrafficTopReport**</span></span>
    
- <span data-ttu-id="46d34-247">**Set-malwarefilteringserver**</span><span class="sxs-lookup"><span data-stu-id="46d34-247">**Get-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="46d34-248">**Set-malwarefilteringserver**</span><span class="sxs-lookup"><span data-stu-id="46d34-248">**Set-MalwareFilteringServer**</span></span>
    
- <span data-ttu-id="46d34-249">**New-malwarefilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-249">**Get-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-250">**New-malwarefilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-250">**New-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-251">**New-malwarefilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-251">**Remove-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-252">**New-malwarefilterpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-252">**Set-MalwareFilterPolicy**</span></span>
    
- <span data-ttu-id="46d34-253">**MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="46d34-253">**Get-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="46d34-254">**MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="46d34-254">**Remove-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="46d34-255">**MalwareFilterRecoveryItem**</span><span class="sxs-lookup"><span data-stu-id="46d34-255">**Resume-MalwareFilterRecoveryItem**</span></span>
    
- <span data-ttu-id="46d34-256">**MapiSubmitSystemProbe**</span><span class="sxs-lookup"><span data-stu-id="46d34-256">**Send-MapiSubmitSystemProbe**</span></span>
    
- <span data-ttu-id="46d34-257">**Redirect-Message**</span><span class="sxs-lookup"><span data-stu-id="46d34-257">**Redirect-Message**</span></span>
    
- <span data-ttu-id="46d34-258">**メッセージトレースの取得**</span><span class="sxs-lookup"><span data-stu-id="46d34-258">**Get-MessageTrace**</span></span>
    
- <span data-ttu-id="46d34-259">**MessageTraceDetail の取得**</span><span class="sxs-lookup"><span data-stu-id="46d34-259">**Get-MessageTraceDetail**</span></span>
    
- <span data-ttu-id="46d34-260">**完了-New-migrationbatch**</span><span class="sxs-lookup"><span data-stu-id="46d34-260">**Complete-MigrationBatch**</span></span>
    
- <span data-ttu-id="46d34-261">**New-migrationbatch**</span><span class="sxs-lookup"><span data-stu-id="46d34-261">**Remove-MigrationBatch**</span></span>
    
- <span data-ttu-id="46d34-262">**は、get-migrationconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-262">**Get-MigrationConfig**</span></span>
    
- <span data-ttu-id="46d34-263">**は、get-migrationconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-263">**Set-MigrationConfig**</span></span>
    
- <span data-ttu-id="46d34-264">**New-migrationendpoint**</span><span class="sxs-lookup"><span data-stu-id="46d34-264">**Get-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="46d34-265">**New-migrationendpoint**</span><span class="sxs-lookup"><span data-stu-id="46d34-265">**New-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="46d34-266">**New-migrationendpoint**</span><span class="sxs-lookup"><span data-stu-id="46d34-266">**Remove-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="46d34-267">**New-migrationendpoint**</span><span class="sxs-lookup"><span data-stu-id="46d34-267">**Set-MigrationEndpoint**</span></span>
    
- <span data-ttu-id="46d34-268">**MigrationStatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-268">**Get-MigrationStatistics**</span></span>
    
- <span data-ttu-id="46d34-269">**MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="46d34-269">**Get-MigrationUser**</span></span>
    
- <span data-ttu-id="46d34-270">**MigrationUser**</span><span class="sxs-lookup"><span data-stu-id="46d34-270">**Remove-MigrationUser**</span></span>
    
- <span data-ttu-id="46d34-271">**Get-migrationuserstatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-271">**Get-MigrationUserStatistics**</span></span>
    
- <span data-ttu-id="46d34-272">**Clear-mobiledevice**</span><span class="sxs-lookup"><span data-stu-id="46d34-272">**Clear-MobileDevice**</span></span>
    
- <span data-ttu-id="46d34-273">**Get-MobileDevice**</span><span class="sxs-lookup"><span data-stu-id="46d34-273">**Get-MobileDevice**</span></span>
    
- <span data-ttu-id="46d34-274">**Clear-mobiledevice**</span><span class="sxs-lookup"><span data-stu-id="46d34-274">**Remove-MobileDevice**</span></span>
    
- <span data-ttu-id="46d34-275">**New-mobiledevicemailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-275">**Get-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-276">**New-mobiledevicemailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-276">**New-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-277">**New-mobiledevicemailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-277">**Remove-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-278">**New-mobiledevicemailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-278">**Set-MobileDeviceMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-279">**MobileDeviceStatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-279">**Get-MobileDeviceStatistics**</span></span>
    
- <span data-ttu-id="46d34-280">**取得-MonitoringItemHelp**</span><span class="sxs-lookup"><span data-stu-id="46d34-280">**Get-MonitoringItemHelp**</span></span>
    
- <span data-ttu-id="46d34-281">**取得-MonitoringItemIdentity**</span><span class="sxs-lookup"><span data-stu-id="46d34-281">**Get-MonitoringItemIdentity**</span></span>
    
- <span data-ttu-id="46d34-282">**呼び出し-MonitoringProbe**</span><span class="sxs-lookup"><span data-stu-id="46d34-282">**Invoke-MonitoringProbe**</span></span>
    
- <span data-ttu-id="46d34-283">**取得-通知**</span><span class="sxs-lookup"><span data-stu-id="46d34-283">**Get-Notification**</span></span>
    
- <span data-ttu-id="46d34-284">**設定-通知**</span><span class="sxs-lookup"><span data-stu-id="46d34-284">**Set-Notification**</span></span>
    
- <span data-ttu-id="46d34-285">**テスト-OAuthConnectivity**</span><span class="sxs-lookup"><span data-stu-id="46d34-285">**Test-OAuthConnectivity**</span></span>
    
- <span data-ttu-id="46d34-286">**OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="46d34-286">**Get-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="46d34-287">**OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="46d34-287">**New-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="46d34-288">**OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="46d34-288">**Remove-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="46d34-289">**OnPremisesOrganization**</span><span class="sxs-lookup"><span data-stu-id="46d34-289">**Set-OnPremisesOrganization**</span></span>
    
- <span data-ttu-id="46d34-290">**組織のカスタマイズを有効にする**</span><span class="sxs-lookup"><span data-stu-id="46d34-290">**Enable-OrganizationCustomization**</span></span>
    
- <span data-ttu-id="46d34-291">**取得-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-291">**Get-OutboundConnector**</span></span>
    
- <span data-ttu-id="46d34-292">**新しい-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-292">**New-OutboundConnector**</span></span>
    
- <span data-ttu-id="46d34-293">**-OutboundConnector の削除**</span><span class="sxs-lookup"><span data-stu-id="46d34-293">**Remove-OutboundConnector**</span></span>
    
- <span data-ttu-id="46d34-294">**設定-OutboundConnector**</span><span class="sxs-lookup"><span data-stu-id="46d34-294">**Set-OutboundConnector**</span></span>
    
- <span data-ttu-id="46d34-295">**PartnerApplication の取得**</span><span class="sxs-lookup"><span data-stu-id="46d34-295">**Get-PartnerApplication**</span></span>
    
- <span data-ttu-id="46d34-296">**新しいパートナーアプリケーション**</span><span class="sxs-lookup"><span data-stu-id="46d34-296">**New-PartnerApplication**</span></span>
    
- <span data-ttu-id="46d34-297">**削除-パートナーアプリケーション**</span><span class="sxs-lookup"><span data-stu-id="46d34-297">**Remove-PartnerApplication**</span></span>
    
- <span data-ttu-id="46d34-298">**セットパートナーアプリケーション**</span><span class="sxs-lookup"><span data-stu-id="46d34-298">**Set-PartnerApplication**</span></span>
    
- <span data-ttu-id="46d34-299">**Get-pendingfederateddomain**</span><span class="sxs-lookup"><span data-stu-id="46d34-299">**Get-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="46d34-300">**Get-pendingfederateddomain**</span><span class="sxs-lookup"><span data-stu-id="46d34-300">**Set-PendingFederatedDomain**</span></span>
    
- <span data-ttu-id="46d34-301">**取得-ポリシーヒント Config**</span><span class="sxs-lookup"><span data-stu-id="46d34-301">**Get-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="46d34-302">**新しいポリシーヒントの構成**</span><span class="sxs-lookup"><span data-stu-id="46d34-302">**New-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="46d34-303">**削除-ポリシーヒント Config**</span><span class="sxs-lookup"><span data-stu-id="46d34-303">**Remove-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="46d34-304">**設定-ポリシーヒント Config**</span><span class="sxs-lookup"><span data-stu-id="46d34-304">**Set-PolicyTipConfig**</span></span>
    
- <span data-ttu-id="46d34-305">**ダンプ-プロビジョニングキャッシュ**</span><span class="sxs-lookup"><span data-stu-id="46d34-305">**Dump-ProvisioningCache**</span></span>
    
- <span data-ttu-id="46d34-306">**リセット-プロビジョニングキャッシュ**</span><span class="sxs-lookup"><span data-stu-id="46d34-306">**Reset-ProvisioningCache**</span></span>
    
- <span data-ttu-id="46d34-307">**Update-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-307">**Update-PublicFolderMailbox**</span></span>
    
- <span data-ttu-id="46d34-308">**PublicFolderMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="46d34-308">**Get-PublicFolderMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="46d34-309">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-309">**Get-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-310">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-310">**New-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-311">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-311">**Remove-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-312">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-312">**Resume-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-313">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-313">**Set-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-314">**Set-publicfoldermigrationrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-314">**Suspend-PublicFolderMigrationRequest**</span></span>
    
- <span data-ttu-id="46d34-315">**PublicFolderMigrationRequestStatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-315">**Get-PublicFolderMigrationRequestStatistics**</span></span>
    
- <span data-ttu-id="46d34-316">**Get-quarantinemessage**</span><span class="sxs-lookup"><span data-stu-id="46d34-316">**Get-QuarantineMessage**</span></span>
    
- <span data-ttu-id="46d34-317">**Get-quarantinemessage**</span><span class="sxs-lookup"><span data-stu-id="46d34-317">**Release-QuarantineMessage**</span></span>
    
- <span data-ttu-id="46d34-318">**Get-queuedigest**</span><span class="sxs-lookup"><span data-stu-id="46d34-318">**Get-QueueDigest**</span></span>
    
- <span data-ttu-id="46d34-319">**取得-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-319">**Get-ResourcePolicy**</span></span>
    
- <span data-ttu-id="46d34-320">**新しい-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-320">**New-ResourcePolicy**</span></span>
    
- <span data-ttu-id="46d34-321">**削除-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-321">**Remove-ResourcePolicy**</span></span>
    
- <span data-ttu-id="46d34-322">**設定-ResourcePolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-322">**Set-ResourcePolicy**</span></span>
    
- <span data-ttu-id="46d34-323">**追加-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-323">**Add-ResubmitRequest**</span></span>
    
- <span data-ttu-id="46d34-324">**Get-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-324">**Get-ResubmitRequest**</span></span>
    
- <span data-ttu-id="46d34-325">**削除-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-325">**Remove-ResubmitRequest**</span></span>
    
- <span data-ttu-id="46d34-326">**設定-ResubmitRequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-326">**Set-ResubmitRequest**</span></span>
    
- <span data-ttu-id="46d34-327">**取得-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="46d34-327">**Get-ServerComponentState**</span></span>
    
- <span data-ttu-id="46d34-328">**Set-ServerComponentState**</span><span class="sxs-lookup"><span data-stu-id="46d34-328">**Set-ServerComponentState**</span></span>
    
- <span data-ttu-id="46d34-329">**取得-ServerHealth**</span><span class="sxs-lookup"><span data-stu-id="46d34-329">**Get-ServerHealth**</span></span>
    
- <span data-ttu-id="46d34-330">**Set-ServerMonitor**</span><span class="sxs-lookup"><span data-stu-id="46d34-330">**Set-ServerMonitor**</span></span>
    
- <span data-ttu-id="46d34-331">**追加-ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="46d34-331">**Add-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="46d34-332">**取得-ServerMonitoringOverride**</span><span class="sxs-lookup"><span data-stu-id="46d34-332">**Get-ServerMonitoringOverride**</span></span>
    
- <span data-ttu-id="46d34-333">**SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-333">**Get-SiteMailbox**</span></span>
    
- <span data-ttu-id="46d34-334">**SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-334">**New-SiteMailbox**</span></span>
    
- <span data-ttu-id="46d34-335">**SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-335">**Set-SiteMailbox**</span></span>
    
- <span data-ttu-id="46d34-336">**SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-336">**Test-SiteMailbox**</span></span>
    
- <span data-ttu-id="46d34-337">**SiteMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-337">**Update-SiteMailbox**</span></span>
    
- <span data-ttu-id="46d34-338">**Get-SiteMailboxDiagnostics**</span><span class="sxs-lookup"><span data-stu-id="46d34-338">**Get-SiteMailboxDiagnostics**</span></span>
    
- <span data-ttu-id="46d34-339">**Get-Sitemailboxプロビジョニングポリシー**</span><span class="sxs-lookup"><span data-stu-id="46d34-339">**Get-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="46d34-340">**新しい-Sitemailboxプロビジョニングポリシー**</span><span class="sxs-lookup"><span data-stu-id="46d34-340">**New-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="46d34-341">**削除-Sitemailboxプロビジョニングポリシー**</span><span class="sxs-lookup"><span data-stu-id="46d34-341">**Remove-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="46d34-342">**設定-Sitemailboxプロビジョニングポリシー**</span><span class="sxs-lookup"><span data-stu-id="46d34-342">**Set-SiteMailboxProvisioningPolicy**</span></span>
    
- <span data-ttu-id="46d34-343">**元に戻す-SoftDeletedMailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-343">**Undo-SoftDeletedMailbox**</span></span>
    
- <span data-ttu-id="46d34-344">**Get-stalemailboxdetailreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-344">**Get-StaleMailboxDetailReport**</span></span>
    
- <span data-ttu-id="46d34-345">**Get-stalemailboxreport**</span><span class="sxs-lookup"><span data-stu-id="46d34-345">**Get-StaleMailboxReport**</span></span>
    
- <span data-ttu-id="46d34-346">**更新-StoreMailboxState**</span><span class="sxs-lookup"><span data-stu-id="46d34-346">**Update-StoreMailboxState**</span></span>
    
- <span data-ttu-id="46d34-347">**SyncMailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-347">**New-SyncMailPublicFolder**</span></span>
    
- <span data-ttu-id="46d34-348">**取得-TransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-348">**Get-TransportService**</span></span>
    
- <span data-ttu-id="46d34-349">**Set-TransportService**</span><span class="sxs-lookup"><span data-stu-id="46d34-349">**Set-TransportService**</span></span>
    
- <span data-ttu-id="46d34-350">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-350">**Disable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-351">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-351">**Enable-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-352">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-352">**Get-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-353">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-353">**New-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-354">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-354">**Remove-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-355">**Enable-umcallansweringrule**</span><span class="sxs-lookup"><span data-stu-id="46d34-355">**Set-UMCallAnsweringRule**</span></span>
    
- <span data-ttu-id="46d34-356">**Get-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="46d34-356">**Get-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="46d34-357">**Set-UMCallRouterSettings**</span><span class="sxs-lookup"><span data-stu-id="46d34-357">**Set-UMCallRouterSettings**</span></span>
    
- <span data-ttu-id="46d34-358">**Disable-UMService**</span><span class="sxs-lookup"><span data-stu-id="46d34-358">**Disable-UMService**</span></span>
    
- <span data-ttu-id="46d34-359">**Enable-UMService**</span><span class="sxs-lookup"><span data-stu-id="46d34-359">**Enable-UMService**</span></span>
    
- <span data-ttu-id="46d34-360">**Get-UMService**</span><span class="sxs-lookup"><span data-stu-id="46d34-360">**Get-UMService**</span></span>
    
- <span data-ttu-id="46d34-361">**Set-UMService**</span><span class="sxs-lookup"><span data-stu-id="46d34-361">**Set-UMService**</span></span>
    
- <span data-ttu-id="46d34-362">**Get-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="46d34-362">**Get-UserPhoto**</span></span>
    
- <span data-ttu-id="46d34-363">**Remove-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="46d34-363">**Remove-UserPhoto**</span></span>
    
- <span data-ttu-id="46d34-364">**Set-UserPhoto**</span><span class="sxs-lookup"><span data-stu-id="46d34-364">**Set-UserPhoto**</span></span>
    
- <span data-ttu-id="46d34-365">**WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-365">**Get-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="46d34-366">**WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-366">**New-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="46d34-367">**WorkloadManagementPolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-367">**Remove-WorkloadManagementPolicy**</span></span>
    
- <span data-ttu-id="46d34-368">**Get-workloadpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-368">**Get-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="46d34-369">**Get-workloadpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-369">**New-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="46d34-370">**Get-workloadpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-370">**Remove-WorkloadPolicy**</span></span>
    
- <span data-ttu-id="46d34-371">**Get-workloadpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-371">**Set-WorkloadPolicy**</span></span>
    
### <a name="modified-cmdlets"></a><span data-ttu-id="46d34-372">変更されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-372">Modified cmdlets</span></span>
<span data-ttu-id="46d34-373"><a name="bk_update"> </a></span><span class="sxs-lookup"><span data-stu-id="46d34-373"><a name="bk_update"> </a></span></span>

<span data-ttu-id="46d34-374">Exchange 2013 では、次のコマンドレットの入力または出力の種類が変更されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-374">The input or output types for following cmdlets were modified in Exchange 2013:</span></span>
  
- <span data-ttu-id="46d34-375">**Clear-activesyncdevice**</span><span class="sxs-lookup"><span data-stu-id="46d34-375">**Clear-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="46d34-376">**Clear-activesyncdevice**</span><span class="sxs-lookup"><span data-stu-id="46d34-376">**Remove-ActiveSyncDevice**</span></span>
    
- <span data-ttu-id="46d34-377">**New-activesyncmailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-377">**Get-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-378">**New-activesyncmailboxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-378">**New-ActiveSyncMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-379">**Set-activesyncvirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-379">**New-ActiveSyncVirtualDirectory**</span></span>
    
- <span data-ttu-id="46d34-380">**New-autodiscovervirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-380">**New-AutodiscoverVirtualDirectory**</span></span>
    
- <span data-ttu-id="46d34-381">**Get-availabilityconfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-381">**Set-AvailabilityConfig**</span></span>
    
- <span data-ttu-id="46d34-382">**Get-exchangecertificate**</span><span class="sxs-lookup"><span data-stu-id="46d34-382">**Enable-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="46d34-383">**Get-exchangecertificate**</span><span class="sxs-lookup"><span data-stu-id="46d34-383">**Export-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="46d34-384">**Get-exchangecertificate**</span><span class="sxs-lookup"><span data-stu-id="46d34-384">**Import-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="46d34-385">**Get-exchangecertificate**</span><span class="sxs-lookup"><span data-stu-id="46d34-385">**Remove-ExchangeCertificate**</span></span>
    
- <span data-ttu-id="46d34-386">**取得-失敗 Contentindexdocuments**</span><span class="sxs-lookup"><span data-stu-id="46d34-386">**Get-FailedContentIndexDocuments**</span></span>
    
- <span data-ttu-id="46d34-387">**Get-federationinformation**</span><span class="sxs-lookup"><span data-stu-id="46d34-387">**Get-FederationInformation**</span></span>
    
- <span data-ttu-id="46d34-388">**HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="46d34-388">**New-HybridConfiguration**</span></span>
    
- <span data-ttu-id="46d34-389">**HybridConfiguration**</span><span class="sxs-lookup"><span data-stu-id="46d34-389">**Set-HybridConfiguration**</span></span>
    
- <span data-ttu-id="46d34-390">**New-Mailbox**</span><span class="sxs-lookup"><span data-stu-id="46d34-390">**New-Mailbox**</span></span>
    
- <span data-ttu-id="46d34-391">**Update-mailboxdatabasecopy**</span><span class="sxs-lookup"><span data-stu-id="46d34-391">**Resume-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="46d34-392">**Update-mailboxdatabasecopy**</span><span class="sxs-lookup"><span data-stu-id="46d34-392">**Set-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="46d34-393">**Update-mailboxdatabasecopy**</span><span class="sxs-lookup"><span data-stu-id="46d34-393">**Suspend-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="46d34-394">**Update-MailboxDatabaseCopy**</span><span class="sxs-lookup"><span data-stu-id="46d34-394">**Update-MailboxDatabaseCopy**</span></span>
    
- <span data-ttu-id="46d34-395">**New-mailboxexportrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-395">**Get-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="46d34-396">**New-mailboxexportrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-396">**Set-MailboxExportRequest**</span></span>
    
- <span data-ttu-id="46d34-397">**Add-mailboxfolderpermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-397">**Add-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="46d34-398">**Add-mailboxfolderpermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-398">**Remove-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="46d34-399">**Add-mailboxfolderpermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-399">**Set-MailboxFolderPermission**</span></span>
    
- <span data-ttu-id="46d34-400">**New-mailboximportrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-400">**Get-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="46d34-401">**New-mailboximportrequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-401">**Set-MailboxImportRequest**</span></span>
    
- <span data-ttu-id="46d34-402">**Get-mailboxrestorerequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-402">**Get-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="46d34-403">**Get-mailboxrestorerequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-403">**Set-MailboxRestoreRequest**</span></span>
    
- <span data-ttu-id="46d34-404">**Get-mailboxsearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-404">**Get-MailboxSearch**</span></span>
    
- <span data-ttu-id="46d34-405">**Get-mailboxsearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-405">**Remove-MailboxSearch**</span></span>
    
- <span data-ttu-id="46d34-406">**Set-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-406">**Set-MailboxSearch**</span></span>
    
- <span data-ttu-id="46d34-407">**Start-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-407">**Start-MailboxSearch**</span></span>
    
- <span data-ttu-id="46d34-408">**Stop-MailboxSearch**</span><span class="sxs-lookup"><span data-stu-id="46d34-408">**Stop-MailboxSearch**</span></span>
    
- <span data-ttu-id="46d34-409">**Set-mailpublicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-409">**Disable-MailPublicFolder**</span></span>
    
- <span data-ttu-id="46d34-410">**Get-MailPublicFolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-410">**Get-MailPublicFolder**</span></span>
    
- <span data-ttu-id="46d34-411">**Set-mailpublicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-411">**Set-MailPublicFolder**</span></span>
    
- <span data-ttu-id="46d34-412">**New-migrationbatch**</span><span class="sxs-lookup"><span data-stu-id="46d34-412">**Get-MigrationBatch**</span></span>
    
- <span data-ttu-id="46d34-413">**New-MigrationBatch**</span><span class="sxs-lookup"><span data-stu-id="46d34-413">**New-MigrationBatch**</span></span>
    
- <span data-ttu-id="46d34-414">**New-migrationbatch**</span><span class="sxs-lookup"><span data-stu-id="46d34-414">**Set-MigrationBatch**</span></span>
    
- <span data-ttu-id="46d34-415">**Test-migrationserveravailability**</span><span class="sxs-lookup"><span data-stu-id="46d34-415">**Test-MigrationServerAvailability**</span></span>
    
- <span data-ttu-id="46d34-416">**New-moverequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-416">**Get-MoveRequest**</span></span>
    
- <span data-ttu-id="46d34-417">**Update-offlineaddressbook**</span><span class="sxs-lookup"><span data-stu-id="46d34-417">**New-OfflineAddressBook**</span></span>
    
- <span data-ttu-id="46d34-418">**Get-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-418">**Get-OrganizationConfig**</span></span>
    
- <span data-ttu-id="46d34-419">**Set-OrganizationConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-419">**Set-OrganizationConfig**</span></span>
    
- <span data-ttu-id="46d34-420">**テスト-OutlookConnectivity**</span><span class="sxs-lookup"><span data-stu-id="46d34-420">**Test-OutlookConnectivity**</span></span>
    
- <span data-ttu-id="46d34-421">**テスト-OutlookWebServices 方法**</span><span class="sxs-lookup"><span data-stu-id="46d34-421">**Test-OutlookWebServices**</span></span>
    
- <span data-ttu-id="46d34-422">**取得-Owam/Boxpolicy**</span><span class="sxs-lookup"><span data-stu-id="46d34-422">**Get-OwaMailboxPolicy**</span></span>
    
- <span data-ttu-id="46d34-423">**Set-owavirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-423">**New-OwaVirtualDirectory**</span></span>
    
- <span data-ttu-id="46d34-424">**Get-powershellvirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-424">**New-PowerShellVirtualDirectory**</span></span>
    
- <span data-ttu-id="46d34-425">**New-publicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-425">**Get-PublicFolder**</span></span>
    
- <span data-ttu-id="46d34-426">**New-publicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-426">**New-PublicFolder**</span></span>
    
- <span data-ttu-id="46d34-427">**New-publicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-427">**Set-PublicFolder**</span></span>
    
- <span data-ttu-id="46d34-428">**Add-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-428">**Add-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="46d34-429">**Get-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-429">**Get-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="46d34-430">**Remove-PublicFolderClientPermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-430">**Remove-PublicFolderClientPermission**</span></span>
    
- <span data-ttu-id="46d34-431">**取得-PublicFolderItemStatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-431">**Get-PublicFolderItemStatistics**</span></span>
    
- <span data-ttu-id="46d34-432">**Get-PublicFolderStatistics**</span><span class="sxs-lookup"><span data-stu-id="46d34-432">**Get-PublicFolderStatistics**</span></span>
    
- <span data-ttu-id="46d34-433">**Get-Recipient**</span><span class="sxs-lookup"><span data-stu-id="46d34-433">**Get-Recipient**</span></span>
    
- <span data-ttu-id="46d34-434">**Set-ResourceConfig**</span><span class="sxs-lookup"><span data-stu-id="46d34-434">**Set-ResourceConfig**</span></span>
    
- <span data-ttu-id="46d34-435">**テスト-Webサービス接続**</span><span class="sxs-lookup"><span data-stu-id="46d34-435">**Test-WebServicesConnectivity**</span></span>
    
- <span data-ttu-id="46d34-436">**Set-webservicesvirtualdirectory**</span><span class="sxs-lookup"><span data-stu-id="46d34-436">**New-WebServicesVirtualDirectory**</span></span>
    
### <a name="removed-cmdlets"></a><span data-ttu-id="46d34-437">削除されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="46d34-437">Removed cmdlets</span></span>
<span data-ttu-id="46d34-438"><a name="bk_removed"> </a></span><span class="sxs-lookup"><span data-stu-id="46d34-438"><a name="bk_removed"> </a></span></span>

<span data-ttu-id="46d34-439">次のコマンドレットが Exchange 2013 から削除されました。</span><span class="sxs-lookup"><span data-stu-id="46d34-439">The following cmdlets were removed from Exchange 2013:</span></span>
  
- <span data-ttu-id="46d34-440">**FileDistributionService**</span><span class="sxs-lookup"><span data-stu-id="46d34-440">**Update-FileDistributionService**</span></span>
    
- <span data-ttu-id="46d34-441">**復元-メールボックス**</span><span class="sxs-lookup"><span data-stu-id="46d34-441">**Restore-Mailbox**</span></span>
    
- <span data-ttu-id="46d34-442">**Set-mailboxdatabase**</span><span class="sxs-lookup"><span data-stu-id="46d34-442">**Clean-MailboxDatabase**</span></span>
    
- <span data-ttu-id="46d34-443">**完全移行**</span><span class="sxs-lookup"><span data-stu-id="46d34-443">**Complete-Migration**</span></span>
    
- <span data-ttu-id="46d34-444">**MigrationStatus**</span><span class="sxs-lookup"><span data-stu-id="46d34-444">**Get-MigrationStatus**</span></span>
    
- <span data-ttu-id="46d34-445">**New-publicfolder**</span><span class="sxs-lookup"><span data-stu-id="46d34-445">**Update-PublicFolder**</span></span>
    
- <span data-ttu-id="46d34-446">**Add-publicfolderadministrativepermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-446">**Add-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="46d34-447">**Add-publicfolderadministrativepermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-447">**Get-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="46d34-448">**Add-publicfolderadministrativepermission**</span><span class="sxs-lookup"><span data-stu-id="46d34-448">**Remove-PublicFolderAdministrativePermission**</span></span>
    
- <span data-ttu-id="46d34-449">**新しい-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="46d34-449">**New-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="46d34-450">**削除-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="46d34-450">**Remove-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="46d34-451">**Set-PublicFolderDatabase**</span><span class="sxs-lookup"><span data-stu-id="46d34-451">**Set-PublicFolderDatabase**</span></span>
    
- <span data-ttu-id="46d34-452">**PublicFolderDatabaseRepairRequest**</span><span class="sxs-lookup"><span data-stu-id="46d34-452">**New-PublicFolderDatabaseRepairRequest**</span></span>
    
- <span data-ttu-id="46d34-453">**更新-PublicFolderHierarchy**</span><span class="sxs-lookup"><span data-stu-id="46d34-453">**Update-PublicFolderHierarchy**</span></span>
    
- <span data-ttu-id="46d34-454">**Resume-PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="46d34-454">**Resume-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="46d34-455">**Suspend-PublicFolderReplication**</span><span class="sxs-lookup"><span data-stu-id="46d34-455">**Suspend-PublicFolderReplication**</span></span>
    
- <span data-ttu-id="46d34-456">**RetentionAutoTagLearning**</span><span class="sxs-lookup"><span data-stu-id="46d34-456">**Start-RetentionAutoTagLearning**</span></span>
    
- <span data-ttu-id="46d34-457">**テスト-SystemHealth**</span><span class="sxs-lookup"><span data-stu-id="46d34-457">**Test-SystemHealth**</span></span>
    
- <span data-ttu-id="46d34-458">**Disable-UMServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-458">**Disable-UMServer**</span></span>
    
- <span data-ttu-id="46d34-459">**Enable-UMServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-459">**Enable-UMServer**</span></span>
    
- <span data-ttu-id="46d34-460">**取得-UMServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-460">**Get-UMServer**</span></span>
    
- <span data-ttu-id="46d34-461">**Set-UMServer**</span><span class="sxs-lookup"><span data-stu-id="46d34-461">**Set-UMServer**</span></span>
    
## <a name="see-also"></a><span data-ttu-id="46d34-462">関連項目</span><span class="sxs-lookup"><span data-stu-id="46d34-462">See also</span></span>

- [<span data-ttu-id="46d34-463">Exchange 管理シェル コマンドレットの入力と出力の種類</span><span class="sxs-lookup"><span data-stu-id="46d34-463">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)    
- [<span data-ttu-id="46d34-464">Exchange 管理シェルを使用してメールユーザーの一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="46d34-464">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)    
- [<span data-ttu-id="46d34-465">Exchange 2013 cmdlets</span><span class="sxs-lookup"><span data-stu-id="46d34-465">Exchange 2013 cmdlets</span></span>](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx)
    

