---
title: 組織のリレーションシップ設定 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: 組織の組織上の関係のリストを表す。 この要素は、組織内でのみ使用できます。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 383b3635e1435c6597ccf793a7990c411c02d36d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462459"
---
# <a name="organizationrelationshipsettings-soap"></a><span data-ttu-id="1f045-105">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-105">OrganizationRelationshipSettings (SOAP)</span></span>

<span data-ttu-id="1f045-106">組織**の**組織上の関係のリストを表す。</span><span class="sxs-lookup"><span data-stu-id="1f045-106">The **OrganizationRelationshipSettings** element represents a list of organization relationships for a single organization.</span></span> <span data-ttu-id="1f045-107">この要素は、**組織**内でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1f045-107">The **OrganizationRelationshipSettings** element is for internal use only.</span></span> <span data-ttu-id="1f045-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="1f045-108">This element is not used by clients.</span></span> 
  
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

 <span data-ttu-id="1f045-109">**組織のリレーションシップ設定**</span><span class="sxs-lookup"><span data-stu-id="1f045-109">**OrganizationRelationshipSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f045-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f045-110">Attributes and elements</span></span>

<span data-ttu-id="1f045-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f045-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f045-112">属性</span><span class="sxs-lookup"><span data-stu-id="1f045-112">Attributes</span></span>

<span data-ttu-id="1f045-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1f045-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f045-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1f045-114">Child elements</span></span>

|<span data-ttu-id="1f045-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="1f045-115">**Element**</span></span>|<span data-ttu-id="1f045-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f045-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f045-117">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-117">DeliveryReportEnabled (SOAP)</span></span>](deliveryreportenabled-soap.md) <br/> |<span data-ttu-id="1f045-118">[Deliveryreportenabled ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-118">Represents the [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="1f045-119">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-119">DomainNames (SOAP)</span></span>](domainnames-soap.md) <br/> |<span data-ttu-id="1f045-120">ドメイン名のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-120">Represents the domain names collection.</span></span>  <br/> |
|[<span data-ttu-id="1f045-121">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-121">FreeBusyAccessEnabled (SOAP)</span></span>](freebusyaccessenabled-soap.md) <br/> |<span data-ttu-id="1f045-122">[FreeBusyAccessEnabled ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-122">Represents the [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="1f045-123">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-123">FreeBusyAccessLevel (SOAP)</span></span>](freebusyaccesslevel-soap.md) <br/> |<span data-ttu-id="1f045-124">[FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-124">Represents the [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="1f045-125">Mailヒント Accessenabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-125">MailTipsAccessEnabled (SOAP)</span></span>](mailtipsaccessenabled-soap.md) <br/> |<span data-ttu-id="1f045-126">[Mailヒント Accessenabled ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-126">Represents the [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="1f045-127">Mailヒント Accesslevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-127">MailTipsAccessLevel (SOAP)</span></span>](mailtipsaccesslevel-soap.md) <br/> |<span data-ttu-id="1f045-128">[Mailヒント Accesslevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-128">Represents the [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="1f045-129">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-129">MailboxMoveEnabled (SOAP)</span></span>](mailboxmoveenabled-soap.md) <br/> |<span data-ttu-id="1f045-130">[MailboxMoveEnabled ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-130">Represents the [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="1f045-131">Name (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-131">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="1f045-132">組織上の関係の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-132">Represents the name of the organization relationship.</span></span>  <br/> |
|[<span data-ttu-id="1f045-133">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-133">TargetApplicationUri (SOAP)</span></span>](targetapplicationuri-soap.md) <br/> |<span data-ttu-id="1f045-134">ターゲットアプリケーション URI を定義します。</span><span class="sxs-lookup"><span data-stu-id="1f045-134">Defines the target application URI.</span></span>  <br/> |
|[<span data-ttu-id="1f045-135">TargetAutodiscoverEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-135">TargetAutodiscoverEpr (SOAP)</span></span>](targetautodiscoverepr-soap.md) <br/> |<span data-ttu-id="1f045-136">[TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-136">Represents the [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="1f045-137">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-137">TargetSharingEpr (SOAP)</span></span>](targetsharingepr-soap.md) <br/> |<span data-ttu-id="1f045-138">[Targetsharingepr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-138">Represents the [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f045-139">親要素</span><span class="sxs-lookup"><span data-stu-id="1f045-139">Parent elements</span></span>

|<span data-ttu-id="1f045-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f045-140">**Element**</span></span>|<span data-ttu-id="1f045-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f045-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f045-142">組織/リレーションシップ設定コレクション (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f045-142">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="1f045-143">クエリに一致する組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="1f045-143">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f045-144">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1f045-144">Text value</span></span>

<span data-ttu-id="1f045-145">なし。</span><span class="sxs-lookup"><span data-stu-id="1f045-145">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f045-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f045-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f045-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f045-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1f045-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f045-148">Schema Name</span></span>  <br/> |<span data-ttu-id="1f045-149">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f045-149">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1f045-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f045-150">Validation File</span></span>  <br/> |<span data-ttu-id="1f045-151">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1f045-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f045-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f045-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f045-153">はい</span><span class="sxs-lookup"><span data-stu-id="1f045-153">True</span></span>  <br/> |
   

