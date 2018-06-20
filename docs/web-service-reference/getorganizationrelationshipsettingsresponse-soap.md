---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: GetOrganizationRelationshipSettingsResponse 要素には、GetOrganizationRelationshipSettings (SOAP) の操作の応答が含まれています。 GetOrganizationRelationshipSettingsResponse 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760808"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="9ff9f-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ff9f-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="9ff9f-106">**GetOrganizationRelationshipSettingsResponse**要素には、 [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="9ff9f-107">**GetOrganizationRelationshipSettingsResponse**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="9ff9f-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="9ff9f-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="9ff9f-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ff9f-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ff9f-110">Attributes and elements</span></span>

<span data-ttu-id="9ff9f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ff9f-112">属性</span><span class="sxs-lookup"><span data-stu-id="9ff9f-112">Attributes</span></span>

<span data-ttu-id="9ff9f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ff9f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9ff9f-114">Child elements</span></span>

|<span data-ttu-id="9ff9f-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ff9f-115">**Element**</span></span>|<span data-ttu-id="9ff9f-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ff9f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ff9f-117">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ff9f-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="9ff9f-118">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="9ff9f-119">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ff9f-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="9ff9f-120">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="9ff9f-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ff9f-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="9ff9f-122">クエリに一致する組織との関係のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ff9f-123">親要素</span><span class="sxs-lookup"><span data-stu-id="9ff9f-123">Parent elements</span></span>

<span data-ttu-id="9ff9f-124">なし。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9ff9f-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9ff9f-125">Text value</span></span>

<span data-ttu-id="9ff9f-126">なし。</span><span class="sxs-lookup"><span data-stu-id="9ff9f-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ff9f-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ff9f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ff9f-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ff9f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9ff9f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ff9f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9ff9f-130">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="9ff9f-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9ff9f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ff9f-131">Validation File</span></span>  <br/> |<span data-ttu-id="9ff9f-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9ff9f-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ff9f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ff9f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ff9f-134">True</span><span class="sxs-lookup"><span data-stu-id="9ff9f-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ff9f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ff9f-135">See also</span></span>



[<span data-ttu-id="9ff9f-136">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9ff9f-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

