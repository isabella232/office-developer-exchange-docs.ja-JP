---
title: 応答 (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: 応答要素には、GetOrganizationRelationshipSettings (SOAP) の操作の応答の情報が含まれています。 応答は内部使用のみです。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 97bef9ab9f0b860e62646703c35d539b7922a65a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833174"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="50fbf-105">応答 (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="50fbf-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="50fbf-106">**応答**要素には、 [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="50fbf-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="50fbf-107">**応答**は内部使用のみです。</span><span class="sxs-lookup"><span data-stu-id="50fbf-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="50fbf-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="50fbf-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="50fbf-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="50fbf-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50fbf-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="50fbf-110">Attributes and elements</span></span>

<span data-ttu-id="50fbf-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50fbf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50fbf-112">属性</span><span class="sxs-lookup"><span data-stu-id="50fbf-112">Attributes</span></span>

<span data-ttu-id="50fbf-113">なし。</span><span class="sxs-lookup"><span data-stu-id="50fbf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50fbf-114">子要素</span><span class="sxs-lookup"><span data-stu-id="50fbf-114">Child elements</span></span>

|<span data-ttu-id="50fbf-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="50fbf-115">**Element**</span></span>|<span data-ttu-id="50fbf-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="50fbf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50fbf-117">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="50fbf-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="50fbf-118">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="50fbf-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="50fbf-119">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="50fbf-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="50fbf-120">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="50fbf-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="50fbf-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="50fbf-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="50fbf-122">クエリに一致する組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="50fbf-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50fbf-123">親要素</span><span class="sxs-lookup"><span data-stu-id="50fbf-123">Parent elements</span></span>

<span data-ttu-id="50fbf-124">なし。</span><span class="sxs-lookup"><span data-stu-id="50fbf-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="50fbf-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="50fbf-125">Text value</span></span>

<span data-ttu-id="50fbf-126">なし。</span><span class="sxs-lookup"><span data-stu-id="50fbf-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50fbf-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="50fbf-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50fbf-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="50fbf-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="50fbf-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="50fbf-129">Schema Name</span></span>  <br/> |<span data-ttu-id="50fbf-130">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="50fbf-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="50fbf-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="50fbf-131">Validation File</span></span>  <br/> |<span data-ttu-id="50fbf-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="50fbf-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50fbf-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="50fbf-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="50fbf-134">True</span><span class="sxs-lookup"><span data-stu-id="50fbf-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50fbf-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="50fbf-135">See also</span></span>



[<span data-ttu-id="50fbf-136">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="50fbf-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

