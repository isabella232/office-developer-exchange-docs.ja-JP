---
title: GetOrganizationRelationshipSettingsResponseMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fb087ac9-bac7-4635-a54f-3b115d9f5dc4
description: GetOrganizationRelationshipSettingsResponseMessage 要素は、GetOrganizationRelationshipSettings の操作 (SOAP) 要求に対する応答を定義します。 GetOrganizationRelationshipSettingsResponseMessage 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 40a61616acba70d870d0f2ad32de8b828ea64c63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760815"
---
# <a name="getorganizationrelationshipsettingsresponsemessage-soap"></a><span data-ttu-id="974d0-105">GetOrganizationRelationshipSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="974d0-105">GetOrganizationRelationshipSettingsResponseMessage (SOAP)</span></span>

<span data-ttu-id="974d0-106">**GetOrganizationRelationshipSettingsResponseMessage**要素は、 [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="974d0-106">The **GetOrganizationRelationshipSettingsResponseMessage** element defines a response to a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span> <span data-ttu-id="974d0-107">**GetOrganizationRelationshipSettingsResponseMessage**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="974d0-107">The **GetOrganizationRelationshipSettingsResponseMessage** element is for internal use only.</span></span> <span data-ttu-id="974d0-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="974d0-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponseMessage>
   <Response/>
</GetOrganizationRelationshipSettingsResponseMessage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="974d0-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="974d0-109">Attributes and elements</span></span>

<span data-ttu-id="974d0-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="974d0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="974d0-111">属性</span><span class="sxs-lookup"><span data-stu-id="974d0-111">Attributes</span></span>

<span data-ttu-id="974d0-112">なし。</span><span class="sxs-lookup"><span data-stu-id="974d0-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="974d0-113">子要素</span><span class="sxs-lookup"><span data-stu-id="974d0-113">Child elements</span></span>

|<span data-ttu-id="974d0-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="974d0-114">**Element**</span></span>|<span data-ttu-id="974d0-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="974d0-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="974d0-116">応答 (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="974d0-116">Response (GetOrganizationRelationship) (SOAP)</span></span>](response-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="974d0-117">[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答の情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="974d0-117">Contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="974d0-118">親要素</span><span class="sxs-lookup"><span data-stu-id="974d0-118">Parent elements</span></span>

<span data-ttu-id="974d0-119">なし。</span><span class="sxs-lookup"><span data-stu-id="974d0-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="974d0-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="974d0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="974d0-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="974d0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="974d0-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="974d0-122">Schema Name</span></span>  <br/> |<span data-ttu-id="974d0-123">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="974d0-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="974d0-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="974d0-124">Validation File</span></span>  <br/> |<span data-ttu-id="974d0-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="974d0-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="974d0-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="974d0-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="974d0-127">True</span><span class="sxs-lookup"><span data-stu-id="974d0-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="974d0-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="974d0-128">See also</span></span>



[<span data-ttu-id="974d0-129">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="974d0-129">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

