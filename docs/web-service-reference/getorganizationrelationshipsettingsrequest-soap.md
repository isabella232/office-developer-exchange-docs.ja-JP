---
title: GetOrganizationRelationshipSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: GetOrganizationRelationshipSettingsRequest 要素は、GetOrganizationRelationshipSettings の操作 (SOAP) 操作の呼び出しのパラメーターを表します。 GetOrganizationRelationshipSettingsRequest 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 451506d53212ddca416f5b797624688f511988d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760805"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="df493-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="df493-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="df493-106">**GetOrganizationRelationshipSettingsRequest**要素は、 [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作の呼び出しのパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="df493-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="df493-107">**GetOrganizationRelationshipSettingsRequest**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="df493-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="df493-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="df493-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="df493-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="df493-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df493-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="df493-110">Attributes and elements</span></span>

<span data-ttu-id="df493-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df493-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df493-112">属性</span><span class="sxs-lookup"><span data-stu-id="df493-112">Attributes</span></span>

<span data-ttu-id="df493-113">なし。</span><span class="sxs-lookup"><span data-stu-id="df493-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df493-114">子要素</span><span class="sxs-lookup"><span data-stu-id="df493-114">Child elements</span></span>

|<span data-ttu-id="df493-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="df493-115">**Element**</span></span>|<span data-ttu-id="df493-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="df493-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df493-117">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="df493-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="df493-118">ドメイン識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="df493-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="df493-119">親要素</span><span class="sxs-lookup"><span data-stu-id="df493-119">Parent elements</span></span>

<span data-ttu-id="df493-120">なし。</span><span class="sxs-lookup"><span data-stu-id="df493-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df493-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="df493-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df493-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="df493-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="df493-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df493-123">Schema Name</span></span>  <br/> |<span data-ttu-id="df493-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="df493-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="df493-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df493-125">Validation File</span></span>  <br/> |<span data-ttu-id="df493-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="df493-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="df493-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="df493-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="df493-128">True</span><span class="sxs-lookup"><span data-stu-id="df493-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df493-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="df493-129">See also</span></span>



[<span data-ttu-id="df493-130">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="df493-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

