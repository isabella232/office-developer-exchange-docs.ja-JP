---
title: Response (Get組織関係) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: Response 要素には、Get組織の設定操作 (SOAP) 応答の情報が含まれています。 Response 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 55f8cd549f40b780b2e7438634a851a2c3854f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467943"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="1440d-105">Response (Get組織関係) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1440d-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="1440d-106">**Response**要素には、 [Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1440d-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="1440d-107">**Response**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="1440d-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="1440d-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="1440d-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="1440d-109">**Get組織の Relationshipsettingsresponse**</span><span class="sxs-lookup"><span data-stu-id="1440d-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1440d-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1440d-110">Attributes and elements</span></span>

<span data-ttu-id="1440d-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1440d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1440d-112">属性</span><span class="sxs-lookup"><span data-stu-id="1440d-112">Attributes</span></span>

<span data-ttu-id="1440d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1440d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1440d-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1440d-114">Child elements</span></span>

|<span data-ttu-id="1440d-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="1440d-115">**Element**</span></span>|<span data-ttu-id="1440d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1440d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1440d-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1440d-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="1440d-118">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="1440d-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1440d-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1440d-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="1440d-120">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="1440d-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1440d-121">組織/リレーションシップ設定コレクション (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1440d-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="1440d-122">クエリに一致する組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="1440d-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1440d-123">親要素</span><span class="sxs-lookup"><span data-stu-id="1440d-123">Parent elements</span></span>

<span data-ttu-id="1440d-124">なし。</span><span class="sxs-lookup"><span data-stu-id="1440d-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1440d-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1440d-125">Text value</span></span>

<span data-ttu-id="1440d-126">なし。</span><span class="sxs-lookup"><span data-stu-id="1440d-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1440d-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1440d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1440d-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="1440d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1440d-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1440d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1440d-130">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="1440d-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1440d-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1440d-131">Validation File</span></span>  <br/> |<span data-ttu-id="1440d-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1440d-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1440d-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1440d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1440d-134">正しい</span><span class="sxs-lookup"><span data-stu-id="1440d-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1440d-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="1440d-135">See also</span></span>



[<span data-ttu-id="1440d-136">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1440d-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

