---
title: GetOrganizationRelationshipSettingsRequestMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: ec9ad6a0-1a3c-405b-a6ea-b8dd4323c22a
description: GetOrganizationRelationshipSettingRequestMessage 要素は、Get組織の設定操作 (SOAP) 操作要求を表します。 GetOrganizationRelationshipSettingRequestMessage 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: a004bde20fc3445482f70fad6e7e524f5c9285df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456501"
---
# <a name="getorganizationrelationshipsettingsrequestmessage-soap"></a><span data-ttu-id="9c223-105">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c223-105">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span></span>

<span data-ttu-id="9c223-106">**GetOrganizationRelationshipSettingRequestMessage**要素は、 [Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作要求を表します。</span><span class="sxs-lookup"><span data-stu-id="9c223-106">The **GetOrganizationRelationshipSettingRequestMessage** element represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation request.</span></span> <span data-ttu-id="9c223-107">**GetOrganizationRelationshipSettingRequestMessage**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="9c223-107">The **GetOrganizationRelationshipSettingRequestMessage** element is for internal use only.</span></span> <span data-ttu-id="9c223-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="9c223-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingRequestMessage>
   <Request/>
</GetOrganizationRelationshipSettingRequestMessage>
```

 <span data-ttu-id="9c223-109">**Get組織の Relationshipsettingsrequest**</span><span class="sxs-lookup"><span data-stu-id="9c223-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c223-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9c223-110">Attributes and elements</span></span>

<span data-ttu-id="9c223-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c223-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c223-112">属性</span><span class="sxs-lookup"><span data-stu-id="9c223-112">Attributes</span></span>

<span data-ttu-id="9c223-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9c223-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c223-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9c223-114">Child elements</span></span>

|<span data-ttu-id="9c223-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="9c223-115">**Element**</span></span>|<span data-ttu-id="9c223-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c223-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c223-117">Request (Get組織関係) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c223-117">Request (GetOrganizationRelationship) (SOAP)</span></span>](request-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="9c223-118">[Getorganizationrelationshipsettingsrequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="9c223-118">Represents a [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c223-119">親要素</span><span class="sxs-lookup"><span data-stu-id="9c223-119">Parent elements</span></span>

<span data-ttu-id="9c223-120">なし。</span><span class="sxs-lookup"><span data-stu-id="9c223-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c223-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9c223-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c223-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c223-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9c223-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c223-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9c223-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="9c223-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9c223-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c223-125">Validation File</span></span>  <br/> |<span data-ttu-id="9c223-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9c223-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c223-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9c223-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c223-128">正しい</span><span class="sxs-lookup"><span data-stu-id="9c223-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c223-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c223-129">See also</span></span>



[<span data-ttu-id="9c223-130">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c223-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

