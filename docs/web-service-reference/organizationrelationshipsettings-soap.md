---
title: OrganizationRelationshipSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: OrganizationRelationshipSettings 要素は、単一の組織の組織との関係のリストを表します。 OrganizationRelationshipSettings 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: ed6cc0ef1891cd92c02a8e088e913886048623ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832660"
---
# <a name="organizationrelationshipsettings-soap"></a>OrganizationRelationshipSettings (SOAP)

**OrganizationRelationshipSettings**要素は、単一の組織の組織との関係のリストを表します。 **OrganizationRelationshipSettings**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 **OrganizationRelationshipSettings**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DeliveryReportEnabled (SOAP)](deliveryreportenabled-soap.md) <br/> |[DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx)フラグを表します。  <br/> |
|[DomainNames (SOAP)](domainnames-soap.md) <br/> |ドメイン名のコレクションを表します。  <br/> |
|[FreeBusyAccessEnabled (SOAP)](freebusyaccessenabled-soap.md) <br/> |[FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx)フラグを表します。  <br/> |
|[FreeBusyAccessLevel (SOAP)](freebusyaccesslevel-soap.md) <br/> |[FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx)プロパティを表します。  <br/> |
|[MailTipsAccessEnabled (SOAP)](mailtipsaccessenabled-soap.md) <br/> |[MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx)フラグを表します。  <br/> |
|[MailTipsAccessLevel (SOAP)](mailtipsaccesslevel-soap.md) <br/> |[MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx)プロパティを表します。  <br/> |
|[MailboxMoveEnabled (SOAP)](mailboxmoveenabled-soap.md) <br/> |[MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx)フラグを表します。  <br/> |
|[名 (SOAP)](name-soap.md) <br/> |組織の関係の名前を表します。  <br/> |
|[TargetApplicationUri (SOAP)](targetapplicationuri-soap.md) <br/> |ターゲット アプリケーションの URI を定義します。  <br/> |
|[TargetAutodiscoverEpr (SOAP)](targetautodiscoverepr-soap.md) <br/> |[TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx)プロパティを表します。  <br/> |
|[TargetSharingEpr (SOAP)](targetsharingepr-soap.md) <br/> |[TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx)プロパティを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |クエリに一致する組織との関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   

