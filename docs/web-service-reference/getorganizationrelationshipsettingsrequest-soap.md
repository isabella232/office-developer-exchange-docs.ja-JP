---
title: Get組織の Relationshipsettingsrequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: GetOrganizationRelationshipSettingsRequest 要素は、Get組織の設定操作 (SOAP) 操作の呼び出しのパラメーターを表します。 Get組織の設定要求要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 053bbb8cbe2ccdcf6d544ab1fc92bb81765997e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452735"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="aa421-105">Get組織の Relationshipsettingsrequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa421-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="aa421-106">**Getorganizationrelationshipsettingsrequest**要素は、 [Get組織の設定操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)操作の呼び出しのパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="aa421-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="aa421-107">**Get組織**の設定要求要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="aa421-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="aa421-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="aa421-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="aa421-109">**Get組織の Relationshipsettingsrequest**</span><span class="sxs-lookup"><span data-stu-id="aa421-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa421-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aa421-110">Attributes and elements</span></span>

<span data-ttu-id="aa421-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa421-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa421-112">属性</span><span class="sxs-lookup"><span data-stu-id="aa421-112">Attributes</span></span>

<span data-ttu-id="aa421-113">なし。</span><span class="sxs-lookup"><span data-stu-id="aa421-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa421-114">子要素</span><span class="sxs-lookup"><span data-stu-id="aa421-114">Child elements</span></span>

|<span data-ttu-id="aa421-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="aa421-115">**Element**</span></span>|<span data-ttu-id="aa421-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa421-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa421-117">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa421-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="aa421-118">ドメイン識別子のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="aa421-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="aa421-119">親要素</span><span class="sxs-lookup"><span data-stu-id="aa421-119">Parent elements</span></span>

<span data-ttu-id="aa421-120">なし。</span><span class="sxs-lookup"><span data-stu-id="aa421-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa421-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aa421-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa421-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa421-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="aa421-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa421-123">Schema Name</span></span>  <br/> |<span data-ttu-id="aa421-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="aa421-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="aa421-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa421-125">Validation File</span></span>  <br/> |<span data-ttu-id="aa421-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aa421-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa421-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa421-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa421-128">正しい</span><span class="sxs-lookup"><span data-stu-id="aa421-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa421-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa421-129">See also</span></span>



[<span data-ttu-id="aa421-130">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa421-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

