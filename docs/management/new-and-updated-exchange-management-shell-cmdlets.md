---
title: 新規および更新された Exchange 管理シェル コマンドレット
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5941a439-94d2-4133-81fc-7240863a13df
description: Exchange の Exchange 管理シェルの新機能に関する情報を検索します。
ms.openlocfilehash: b90d7edb83f3cdcaeed11c3692e6981931eaaae1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513872"
---
# <a name="new-and-updated-exchange-management-shell-cmdlets"></a>新規および更新された Exchange 管理シェル コマンドレット

Exchange の Exchange 管理シェルの新機能に関する情報を検索します。
  
**適用対象: Exchange Online |** Exchange Server 2013 |Office 365
  
この記事では、新しい Exchange 管理シェル コマンドレット、変更されたコマンドレットに関する情報を提供します。また、Exchange Online、Office 365 の一部としての Exchange Online、オンプレミスの Exchange から削除されたコマンドレットに関する情報を提供します。
  
## <a name="new-and-updated-cmdlets-in-exchange-2013-sp1"></a>Exchange 2013 SP1 の新規コマンドレットと更新されたコマンドレット

### <a name="new-cmdlets"></a>新規コマンドレット

ビルド 15.00.0847.032 (Exchange Server 2013 SP1) で次のコマンドレットが導入されました。
  
- **Get-AuthRedirect**
    
- **New-AuthRedirect**
    
- **Remove-AuthRedirect**
    
- **Set-AuthRedirect**
    
- **New-DataClassification**
    
- **Remove-DataClassification**
    
- **Set-DataClassification**
    
- **New-FingerPrint**
    
- **Get-MapiVirtualDirectory\***
    
- **New-MapiVirtualDirectory\***
    
- **Remove-MapiVirtualDirectory\***
    
- **Set-MapiVirtualDirectory\***
    
- **Get-OMEConfiguration**
    
- **Set-OMEConfiguration**
    
- **Get-SmimeConfig**
    
- **Set-SmimeConfig**
    
- **Get-IntraOrganizationConfiguration**
    
- **Get-IntraOrganizationConnector**
    
- **New-IntraOrganizationConnector**
    
- **Remove-IntraOrganizationConnector**
    
- **Set-IntraOrganizationConnector**
    
- **Get-HistoricalSearch**
    
- **Start-HistoricalSearch**
    
- **Stop-HistoricalSearch**
    
- **New-SearchDocumentFormat**
    
- **Remove-SearchDocumentFormat**
    
### <a name="updated-cmdlets"></a>更新されたコマンドレット

次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) で更新されました。
  
- **Get-AuditLogSearch**
    
- **Get-QuarantineMessage**
    
- **New-InboundConnector**
    
- **New-MailboxDatabase**
    
- **New-PublicFolderMoveRequest**
    
- **New-TransportRule**
    
- **Set-FrontendTransportService**
    
- **Set-InboundConnector**
    
- **Set-Mailbox**
    
- **Set-MailboxTransportService**
    
- **Set-MoveRequest**
    
- **Set-OrganizationConfig**
    
- **Set-OwaMailboxPolicy**
    
- **Set-OwaVirtualDirectory**
    
- **Set-TransportConfig**
    
- **Set-TransportRule**
    
- **Set-TransportServer**
    
- **Set-TransportService**
    
- **Test-MRSHealth**
    
- **Test-OAuthConnectivity**
    
### <a name="removed-cmdlets"></a>削除されたコマンドレット

次のコマンドレットは、ビルド 15.00.0847.032 (Exchange 2013 SP1) から削除されました。
  
- **Get-AvailabilityReportOutage**
    
- **New-AvailabilityReportOutage**
    
- **Remove-AvailabilityReportOutage**
    
- **Set-AvailabilityReportOutage**
    
## <a name="new-and-updated-cmdlets-in-exchange-2013"></a>Exchange 2013 の新規コマンドレットと更新されたコマンドレット

### <a name="new-cmdlets"></a>新規コマンドレット
<a name="bk_new"> </a>

次のコマンドレットが Exchange 2013 で導入されました。
  
- **Get-ActiveSyncDeviceAutoblockThreshold**
    
- **Set-ActiveSyncDeviceAutoblockThreshold**
    
- **Disable-App**
    
- **Enable-App**
    
- **Get-App**
    
- **New-App**
    
- **Remove-App**
    
- **Set-App**
    
- **Get-AuthConfig**
    
- **Set-AuthConfig**
    
- **Get-AuthServer**
    
- **New-AuthServer**
    
- **Remove-AuthServer**
    
- **Set-AuthServer**
    
- **New-AvailabilityConfig**
    
- **Remove-AvailabilityConfig**
    
- **Get-CalendarDiagnosticAnalysis**
    
- **Get-ClassificationRuleCollection**
    
- **New-ClassificationRuleCollection**
    
- **Remove-ClassificationRuleCollection**
    
- **Set-ClassificationRuleCollection**
    
- **Get-ConnectSubscription**
    
- **New-ConnectSubscription**
    
- **Remove-ConnectSubscription**
    
- **Set-ConnectSubscription**
    
- **Get-DataClassification**
    
- **Get-DataClassificationConfig**
    
- **Get-DlpPolicy**
    
- **New-DlpPolicy**
    
- **Remove-DlpPolicy**
    
- **Set-DlpPolicy**
    
- **Export-DlpPolicyCollection**
    
- **Import-DlpPolicyCollection**
    
- **Get-DlpPolicyTemplate**
    
- **Import-DlpPolicyTemplate**
    
- **Remove-DlpPolicyTemplate**
    
- **Get-ExchangeServerAccessLicense**
    
- **Get-ExchangeServerAccessLicenseUser**
    
- **Get-FfoMigrationReport**
    
- **Get-FrontendTransportService**
    
- **Set-FrontendTransportService**
    
- **Add-GlobalMonitoringOverride**
    
- **Get-GlobalMonitoringOverride**
    
- **Remove-GlobalMonitoringOverride**
    
- **Get-GroupActivityReport**
    
- **Get-HealthReport**
    
- **Get-HostedConnectionFilterPolicy**
    
- **New-HostedConnectionFilterPolicy**
    
- **Remove-HostedConnectionFilterPolicy**
    
- **Set-HostedConnectionFilterPolicy**
    
- **Get-HostedContentFilterPolicy**
    
- **New-HostedContentFilterPolicy**
    
- **Remove-HostedContentFilterPolicy**
    
- **Set-HostedContentFilterPolicy**
    
- **Get-HostedOutboundSpamFilterPolicy**
    
- **Set-HostedOutboundSpamFilterPolicy**
    
- **Remove-HybridConfiguration**
    
- **Get-HybridMailflow**
    
- **Set-HybridMailflow**
    
- **Get-HybridMailflowDatacenterIPs**
    
- **Get-InboundConnector**
    
- **New-InboundConnector**
    
- **Remove-InboundConnector**
    
- **Set-InboundConnector**
    
- **Get-MailboxActivityReport**
    
- **Disable-MailboxQuarantine**
    
- **Enable-MailboxQuarantine**
    
- **Get-MailboxTransportService**
    
- **Set-MailboxTransportService**
    
- **Get-MailDetailDlpPolicyReport**
    
- **Get-MailDetailMalwareReport**
    
- **Get-MailDetailReport**
    
- **Get-MailDetailSpamReport**
    
- **Get-MailDetailTransportRuleReport**
    
- **Get-MailFilterListReport**
    
- **Get-MailTrafficPolicyReport**
    
- **Get-MailTrafficReport**
    
- **Get-MailTrafficSummaryReport**
    
- **Get-MailTrafficTopReport**
    
- **Get-MalwareFilteringServer**
    
- **Set-MalwareFilteringServer**
    
- **Get-MalwareFilterPolicy**
    
- **New-MalwareFilterPolicy**
    
- **Remove-MalwareFilterPolicy**
    
- **Set-MalwareFilterPolicy**
    
- **Get-MalwareFilterRecoveryItem**
    
- **Remove-MalwareFilterRecoveryItem**
    
- **Resume-MalwareFilterRecoveryItem**
    
- **Send-MapiSubmitSystemProbe**
    
- **Redirect-Message**
    
- **Get-MessageTrace**
    
- **Get-MessageTraceDetail**
    
- **Complete-MigrationBatch**
    
- **Remove-MigrationBatch**
    
- **Get-MigrationConfig**
    
- **Set-MigrationConfig**
    
- **Get-MigrationEndpoint**
    
- **New-MigrationEndpoint**
    
- **Remove-MigrationEndpoint**
    
- **Set-MigrationEndpoint**
    
- **Get-MigrationStatistics**
    
- **Get-MigrationUser**
    
- **Remove-MigrationUser**
    
- **Get-MigrationUserStatistics**
    
- **Clear-MobileDevice**
    
- **Get-MobileDevice**
    
- **Remove-MobileDevice**
    
- **Get-MobileDeviceMailboxPolicy**
    
- **New-MobileDeviceMailboxPolicy**
    
- **Remove-MobileDeviceMailboxPolicy**
    
- **Set-MobileDeviceMailboxPolicy**
    
- **Get-MobileDeviceStatistics**
    
- **Get-MonitoringItemHelp**
    
- **Get-MonitoringItemIdentity**
    
- **Invoke-MonitoringProbe**
    
- **Get-Notification**
    
- **Set-Notification**
    
- **Test-OAuthConnectivity**
    
- **Get-OnPremisesOrganization**
    
- **New-OnPremisesOrganization**
    
- **Remove-OnPremisesOrganization**
    
- **Set-OnPremisesOrganization**
    
- **Enable-OrganizationCustomization**
    
- **Get-OutboundConnector**
    
- **New-OutboundConnector**
    
- **Remove-OutboundConnector**
    
- **Set-OutboundConnector**
    
- **Get-PartnerApplication**
    
- **New-PartnerApplication**
    
- **Remove-PartnerApplication**
    
- **Set-PartnerApplication**
    
- **Get-PendingFederatedDomain**
    
- **Set-PendingFederatedDomain**
    
- **Get-PolicyTipConfig**
    
- **New-PolicyTipConfig**
    
- **Remove-PolicyTipConfig**
    
- **Set-PolicyTipConfig**
    
- **Dump-ProvisioningCache**
    
- **Reset-ProvisioningCache**
    
- **Update-PublicFolderMailbox**
    
- **Get-PublicFolderMailboxDiagnostics**
    
- **Get-PublicFolderMigrationRequest**
    
- **New-PublicFolderMigrationRequest**
    
- **Remove-PublicFolderMigrationRequest**
    
- **Resume-PublicFolderMigrationRequest**
    
- **Set-PublicFolderMigrationRequest**
    
- **Suspend-PublicFolderMigrationRequest**
    
- **Get-PublicFolderMigrationRequestStatistics**
    
- **Get-QuarantineMessage**
    
- **Release-QuarantineMessage**
    
- **Get-QueueDigest**
    
- **Get-ResourcePolicy**
    
- **New-ResourcePolicy**
    
- **Remove-ResourcePolicy**
    
- **Set-ResourcePolicy**
    
- **Add-ResubmitRequest**
    
- **Get-ResubmitRequest**
    
- **Remove-ResubmitRequest**
    
- **Set-ResubmitRequest**
    
- **Get-ServerComponentState**
    
- **Set-ServerComponentState**
    
- **Get-ServerHealth**
    
- **Set-ServerMonitor**
    
- **Add-ServerMonitoringOverride**
    
- **Get-ServerMonitoringOverride**
    
- **Get-SiteMailbox**
    
- **New-SiteMailbox**
    
- **Set-SiteMailbox**
    
- **Test-SiteMailbox**
    
- **Update-SiteMailbox**
    
- **Get-SiteMailboxDiagnostics**
    
- **Get-SiteMailboxProvisioningPolicy**
    
- **New-SiteMailboxProvisioningPolicy**
    
- **Remove-SiteMailboxProvisioningPolicy**
    
- **Set-SiteMailboxProvisioningPolicy**
    
- **Undo-SoftDeletedMailbox**
    
- **Get-StaleMailboxDetailReport**
    
- **Get-StaleMailboxReport**
    
- **Update-StoreMailboxState**
    
- **New-SyncMailPublicFolder**
    
- **Get-TransportService**
    
- **Set-TransportService**
    
- **Disable-UMCallAnsweringRule**
    
- **Enable-UMCallAnsweringRule**
    
- **Get-UMCallAnsweringRule**
    
- **New-UMCallAnsweringRule**
    
- **Remove-UMCallAnsweringRule**
    
- **Set-UMCallAnsweringRule**
    
- **Get-UMCallRouterSettings**
    
- **Set-UMCallRouterSettings**
    
- **Disable-UMService**
    
- **Enable-UMService**
    
- **Get-UMService**
    
- **Set-UMService**
    
- **Get-UserPhoto**
    
- **Remove-UserPhoto**
    
- **Set-UserPhoto**
    
- **Get-WorkloadManagementPolicy**
    
- **New-WorkloadManagementPolicy**
    
- **Remove-WorkloadManagementPolicy**
    
- **Get-WorkloadPolicy**
    
- **New-WorkloadPolicy**
    
- **Remove-WorkloadPolicy**
    
- **Set-WorkloadPolicy**
    
### <a name="modified-cmdlets"></a>変更されたコマンドレット
<a name="bk_update"> </a>

Exchange 2013 では、次のコマンドレットの入力または出力の種類が変更されました。
  
- **Clear-ActiveSyncDevice**
    
- **Remove-ActiveSyncDevice**
    
- **Get-ActiveSyncMailboxPolicy**
    
- **New-ActiveSyncMailboxPolicy**
    
- **New-ActiveSyncVirtualDirectory**
    
- **New-AutodiscoverVirtualDirectory**
    
- **Set-AvailabilityConfig**
    
- **Enable-ExchangeCertificate**
    
- **Export-ExchangeCertificate**
    
- **Import-ExchangeCertificate**
    
- **Remove-ExchangeCertificate**
    
- **Get-FailedContentIndexDocuments**
    
- **Get-FederationInformation**
    
- **New-HybridConfiguration**
    
- **Set-HybridConfiguration**
    
- **New-Mailbox**
    
- **Resume-MailboxDatabaseCopy**
    
- **Set-MailboxDatabaseCopy**
    
- **Suspend-MailboxDatabaseCopy**
    
- **Update-MailboxDatabaseCopy**
    
- **Get-MailboxExportRequest**
    
- **Set-MailboxExportRequest**
    
- **Add-MailboxFolderPermission**
    
- **Remove-MailboxFolderPermission**
    
- **Set-MailboxFolderPermission**
    
- **Get-MailboxImportRequest**
    
- **Set-MailboxImportRequest**
    
- **Get-MailboxRestoreRequest**
    
- **Set-MailboxRestoreRequest**
    
- **Get-MailboxSearch**
    
- **Remove-MailboxSearch**
    
- **Set-MailboxSearch**
    
- **Start-MailboxSearch**
    
- **Stop-MailboxSearch**
    
- **Disable-MailPublicFolder**
    
- **Get-MailPublicFolder**
    
- **Set-MailPublicFolder**
    
- **Get-MigrationBatch**
    
- **New-MigrationBatch**
    
- **Set-MigrationBatch**
    
- **Test-MigrationServerAvailability**
    
- **Get-MoveRequest**
    
- **New-OfflineAddressBook**
    
- **Get-OrganizationConfig**
    
- **Set-OrganizationConfig**
    
- **Test-OutlookConnectivity**
    
- **Test-OutlookWebServices**
    
- **Get-OwaMailboxPolicy**
    
- **New-OwaVirtualDirectory**
    
- **New-PowerShellVirtualDirectory**
    
- **Get-PublicFolder**
    
- **New-PublicFolder**
    
- **Set-PublicFolder**
    
- **Add-PublicFolderClientPermission**
    
- **Get-PublicFolderClientPermission**
    
- **Remove-PublicFolderClientPermission**
    
- **Get-PublicFolderItemStatistics**
    
- **Get-PublicFolderStatistics**
    
- **Get-Recipient**
    
- **Set-ResourceConfig**
    
- **Test-WebServicesConnectivity**
    
- **New-WebServicesVirtualDirectory**
    
### <a name="removed-cmdlets"></a>削除されたコマンドレット
<a name="bk_removed"> </a>

次のコマンドレットが Exchange 2013 から削除されました。
  
- **Update-FileDistributionService**
    
- **Restore-Mailbox**
    
- **Clean-MailboxDatabase**
    
- **完全移行**
    
- **Get-MigrationStatus**
    
- **Update-PublicFolder**
    
- **Add-PublicFolderAdministrativePermission**
    
- **Get-PublicFolderAdministrativePermission**
    
- **Remove-PublicFolderAdministrativePermission**
    
- **New-PublicFolderDatabase**
    
- **Remove-PublicFolderDatabase**
    
- **Set-PublicFolderDatabase**
    
- **New-PublicFolderDatabaseRepairRequest**
    
- **Update-PublicFolderHierarchy**
    
- **Resume-PublicFolderReplication**
    
- **Suspend-PublicFolderReplication**
    
- **Start-RetentionAutoTagLearning**
    
- **Test-SystemHealth**
    
- **Disable-UMServer**
    
- **Enable-UMServer**
    
- **Get-UMServer**
    
- **Set-UMServer**
    
## <a name="see-also"></a>関連項目

- [Exchange 管理シェル コマンドレットの入力と出力の種類](exchange-management-shell-cmdlet-input-and-output-types.md)    
- [管理シェルを使用してメール ユーザーのリストをExchangeする](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)    
- [Exchange 2013 cmdlets](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx)
    

