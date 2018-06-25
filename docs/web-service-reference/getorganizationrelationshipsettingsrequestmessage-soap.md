---
title: GetOrganizationRelationshipSettingsRequestMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: ec9ad6a0-1a3c-405b-a6ea-b8dd4323c22a
description: GetOrganizationRelationshipSettingRequestMessage 要素は、GetOrganizationRelationshipSettings 操作 (SOAP) 操作要求を表します。 GetOrganizationRelationshipSettingRequestMessage 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 357f6c75ff81fdf6b31bab15f4662d0f17fbbec0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760809"
---
# <a name="getorganizationrelationshipsettingsrequestmessage-soap"></a><span data-ttu-id="46676-105">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="46676-105">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span></span>

<span data-ttu-id="46676-106">**GetOrganizationRelationshipSettingRequestMessage**要素は、 [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作要求を表します。</span><span class="sxs-lookup"><span data-stu-id="46676-106">The **GetOrganizationRelationshipSettingRequestMessage** element represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation request.</span></span> <span data-ttu-id="46676-107">**GetOrganizationRelationshipSettingRequestMessage**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="46676-107">The **GetOrganizationRelationshipSettingRequestMessage** element is for internal use only.</span></span> <span data-ttu-id="46676-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="46676-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingRequestMessage>
   <Request/>
</GetOrganizationRelationshipSettingRequestMessage>
```

 <span data-ttu-id="46676-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="46676-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46676-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="46676-110">Attributes and elements</span></span>

<span data-ttu-id="46676-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="46676-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46676-112">属性</span><span class="sxs-lookup"><span data-stu-id="46676-112">Attributes</span></span>

<span data-ttu-id="46676-113">なし。</span><span class="sxs-lookup"><span data-stu-id="46676-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46676-114">子要素</span><span class="sxs-lookup"><span data-stu-id="46676-114">Child elements</span></span>

|<span data-ttu-id="46676-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="46676-115">**Element**</span></span>|<span data-ttu-id="46676-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="46676-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46676-117">要求 (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="46676-117">Request (GetOrganizationRelationship) (SOAP)</span></span>](request-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="46676-118">[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="46676-118">Represents a [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46676-119">親要素</span><span class="sxs-lookup"><span data-stu-id="46676-119">Parent elements</span></span>

<span data-ttu-id="46676-120">なし。</span><span class="sxs-lookup"><span data-stu-id="46676-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46676-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="46676-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46676-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="46676-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="46676-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="46676-123">Schema Name</span></span>  <br/> |<span data-ttu-id="46676-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="46676-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="46676-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="46676-125">Validation File</span></span>  <br/> |<span data-ttu-id="46676-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="46676-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46676-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="46676-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="46676-128">True</span><span class="sxs-lookup"><span data-stu-id="46676-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46676-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="46676-129">See also</span></span>



[<span data-ttu-id="46676-130">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="46676-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

