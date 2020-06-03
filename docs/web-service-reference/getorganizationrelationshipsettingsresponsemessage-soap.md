---
title: GetOrganizationRelationshipSettingsResponseMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: fb087ac9-bac7-4635-a54f-3b115d9f5dc4
description: GetOrganizationRelationshipSettingsResponseMessage 要素は、Get組織の設定操作 (SOAP) 要求に対する応答を定義します。 GetOrganizationRelationshipSettingsResponseMessage 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 806f062824e7e8d937f54cd3d38000aba42acf1e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466172"
---
# <a name="getorganizationrelationshipsettingsresponsemessage-soap"></a><span data-ttu-id="92085-105">GetOrganizationRelationshipSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92085-105">GetOrganizationRelationshipSettingsResponseMessage (SOAP)</span></span>

<span data-ttu-id="92085-106">**GetOrganizationRelationshipSettingsResponseMessage**要素は、 [Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="92085-106">The **GetOrganizationRelationshipSettingsResponseMessage** element defines a response to a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span> <span data-ttu-id="92085-107">**GetOrganizationRelationshipSettingsResponseMessage**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="92085-107">The **GetOrganizationRelationshipSettingsResponseMessage** element is for internal use only.</span></span> <span data-ttu-id="92085-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="92085-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponseMessage>
   <Response/>
</GetOrganizationRelationshipSettingsResponseMessage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="92085-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92085-109">Attributes and elements</span></span>

<span data-ttu-id="92085-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92085-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92085-111">属性</span><span class="sxs-lookup"><span data-stu-id="92085-111">Attributes</span></span>

<span data-ttu-id="92085-112">なし。</span><span class="sxs-lookup"><span data-stu-id="92085-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92085-113">子要素</span><span class="sxs-lookup"><span data-stu-id="92085-113">Child elements</span></span>

|<span data-ttu-id="92085-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="92085-114">**Element**</span></span>|<span data-ttu-id="92085-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="92085-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92085-116">Response (Get組織関係) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92085-116">Response (GetOrganizationRelationship) (SOAP)</span></span>](response-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="92085-117">[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)応答情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92085-117">Contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92085-118">親要素</span><span class="sxs-lookup"><span data-stu-id="92085-118">Parent elements</span></span>

<span data-ttu-id="92085-119">なし。</span><span class="sxs-lookup"><span data-stu-id="92085-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92085-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="92085-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92085-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="92085-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="92085-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92085-122">Schema Name</span></span>  <br/> |<span data-ttu-id="92085-123">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="92085-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="92085-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92085-124">Validation File</span></span>  <br/> |<span data-ttu-id="92085-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="92085-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92085-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="92085-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="92085-127">正しい</span><span class="sxs-lookup"><span data-stu-id="92085-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92085-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="92085-128">See also</span></span>



[<span data-ttu-id="92085-129">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="92085-129">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

