---
title: Request (Get組織関係) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 85dc155c-fad0-4756-b9a8-dedf5040a7c6
description: Request 要素は、GetOrganizationRelationshipSettingsRequest (SOAP) 要求を表します。 Request 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 90ccd3579c91c916ea645e6a3b466c9de4706421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459561"
---
# <a name="request-getorganizationrelationship-soap"></a><span data-ttu-id="b125e-105">Request (Get組織関係) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b125e-105">Request (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="b125e-106">**Request**要素は、 [Getorganizationrelationshipsettingsrequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="b125e-106">The **Request** element represents a [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) request.</span></span> <span data-ttu-id="b125e-107">**Request**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="b125e-107">The **Request** element is for internal use only.</span></span> <span data-ttu-id="b125e-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="b125e-108">This element is not used by clients.</span></span> 
  
```XML
<Request>
   <Domains/>
</Request>
```

 <span data-ttu-id="b125e-109">**Get組織の Relationshipsettingsrequest**</span><span class="sxs-lookup"><span data-stu-id="b125e-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b125e-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b125e-110">Attributes and elements</span></span>

<span data-ttu-id="b125e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b125e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b125e-112">属性</span><span class="sxs-lookup"><span data-stu-id="b125e-112">Attributes</span></span>

<span data-ttu-id="b125e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b125e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b125e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b125e-114">Child elements</span></span>

|<span data-ttu-id="b125e-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="b125e-115">**Element**</span></span>|<span data-ttu-id="b125e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b125e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b125e-117">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b125e-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="b125e-118">自動検出が実行され、クエリで使用されるドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="b125e-118">Represents the domains for which Autodiscover is to be run and that are to be used in a query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b125e-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b125e-119">Parent elements</span></span>

|<span data-ttu-id="b125e-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="b125e-120">**Element**</span></span>|<span data-ttu-id="b125e-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b125e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b125e-122">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b125e-122">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span></span>](getorganizationrelationshipsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="b125e-123">[Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作要求を表します。</span><span class="sxs-lookup"><span data-stu-id="b125e-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b125e-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b125e-124">Text value</span></span>

<span data-ttu-id="b125e-125">なし。</span><span class="sxs-lookup"><span data-stu-id="b125e-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b125e-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b125e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b125e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b125e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b125e-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b125e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b125e-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="b125e-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b125e-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b125e-130">Validation File</span></span>  <br/> |<span data-ttu-id="b125e-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b125e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b125e-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b125e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b125e-133">正しい</span><span class="sxs-lookup"><span data-stu-id="b125e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b125e-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b125e-134">See also</span></span>



[<span data-ttu-id="b125e-135">Get組織の Relationshipsettingsrequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b125e-135">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md)


[<span data-ttu-id="b125e-136">自動検出の使用</span><span class="sxs-lookup"><span data-stu-id="b125e-136">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

