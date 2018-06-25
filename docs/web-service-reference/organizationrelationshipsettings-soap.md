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
# <a name="organizationrelationshipsettings-soap"></a><span data-ttu-id="a4747-105">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-105">OrganizationRelationshipSettings (SOAP)</span></span>

<span data-ttu-id="a4747-106">**OrganizationRelationshipSettings**要素は、単一の組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-106">The **OrganizationRelationshipSettings** element represents a list of organization relationships for a single organization.</span></span> <span data-ttu-id="a4747-107">**OrganizationRelationshipSettings**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="a4747-107">The **OrganizationRelationshipSettings** element is for internal use only.</span></span> <span data-ttu-id="a4747-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="a4747-108">This element is not used by clients.</span></span> 
  
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

 <span data-ttu-id="a4747-109">**OrganizationRelationshipSettings**</span><span class="sxs-lookup"><span data-stu-id="a4747-109">**OrganizationRelationshipSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4747-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4747-110">Attributes and elements</span></span>

<span data-ttu-id="a4747-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4747-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4747-112">属性</span><span class="sxs-lookup"><span data-stu-id="a4747-112">Attributes</span></span>

<span data-ttu-id="a4747-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a4747-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4747-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a4747-114">Child elements</span></span>

|<span data-ttu-id="a4747-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4747-115">**Element**</span></span>|<span data-ttu-id="a4747-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4747-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4747-117">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-117">DeliveryReportEnabled (SOAP)</span></span>](deliveryreportenabled-soap.md) <br/> |<span data-ttu-id="a4747-118">[DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-118">Represents the [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="a4747-119">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-119">DomainNames (SOAP)</span></span>](domainnames-soap.md) <br/> |<span data-ttu-id="a4747-120">ドメイン名のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-120">Represents the domain names collection.</span></span>  <br/> |
|[<span data-ttu-id="a4747-121">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-121">FreeBusyAccessEnabled (SOAP)</span></span>](freebusyaccessenabled-soap.md) <br/> |<span data-ttu-id="a4747-122">[FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-122">Represents the [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="a4747-123">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-123">FreeBusyAccessLevel (SOAP)</span></span>](freebusyaccesslevel-soap.md) <br/> |<span data-ttu-id="a4747-124">[FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-124">Represents the [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="a4747-125">MailTipsAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-125">MailTipsAccessEnabled (SOAP)</span></span>](mailtipsaccessenabled-soap.md) <br/> |<span data-ttu-id="a4747-126">[MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-126">Represents the [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="a4747-127">MailTipsAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-127">MailTipsAccessLevel (SOAP)</span></span>](mailtipsaccesslevel-soap.md) <br/> |<span data-ttu-id="a4747-128">[MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-128">Represents the [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="a4747-129">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-129">MailboxMoveEnabled (SOAP)</span></span>](mailboxmoveenabled-soap.md) <br/> |<span data-ttu-id="a4747-130">[MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx)フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-130">Represents the [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="a4747-131">名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-131">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="a4747-132">組織の関係の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-132">Represents the name of the organization relationship.</span></span>  <br/> |
|[<span data-ttu-id="a4747-133">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-133">TargetApplicationUri (SOAP)</span></span>](targetapplicationuri-soap.md) <br/> |<span data-ttu-id="a4747-134">ターゲット アプリケーションの URI を定義します。</span><span class="sxs-lookup"><span data-stu-id="a4747-134">Defines the target application URI.</span></span>  <br/> |
|[<span data-ttu-id="a4747-135">TargetAutodiscoverEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-135">TargetAutodiscoverEpr (SOAP)</span></span>](targetautodiscoverepr-soap.md) <br/> |<span data-ttu-id="a4747-136">[TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-136">Represents the [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="a4747-137">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-137">TargetSharingEpr (SOAP)</span></span>](targetsharingepr-soap.md) <br/> |<span data-ttu-id="a4747-138">[TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx)プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-138">Represents the [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4747-139">親要素</span><span class="sxs-lookup"><span data-stu-id="a4747-139">Parent elements</span></span>

|<span data-ttu-id="a4747-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4747-140">**Element**</span></span>|<span data-ttu-id="a4747-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4747-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4747-142">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a4747-142">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="a4747-143">クエリに一致する組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="a4747-143">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4747-144">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4747-144">Text value</span></span>

<span data-ttu-id="a4747-145">なし。</span><span class="sxs-lookup"><span data-stu-id="a4747-145">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4747-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4747-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4747-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4747-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a4747-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4747-148">Schema Name</span></span>  <br/> |<span data-ttu-id="a4747-149">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="a4747-149">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a4747-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4747-150">Validation File</span></span>  <br/> |<span data-ttu-id="a4747-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4747-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4747-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4747-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4747-153">True</span><span class="sxs-lookup"><span data-stu-id="a4747-153">True</span></span>  <br/> |
   

