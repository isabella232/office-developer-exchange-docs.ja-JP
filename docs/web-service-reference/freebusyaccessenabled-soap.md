---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: FreeBusyAccessEnabled 要素は、FreeBusyAccessEnabled() フラグを表します。 FreeBusyAccessEnabled 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760599"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="7fa3f-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7fa3f-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="7fa3f-106">**FreeBusyAccessEnabled**要素は、 **FreeBusyAccessEnabled()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="7fa3f-107">**FreeBusyAccessEnabled**要素は、内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="7fa3f-108">クライアントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="7fa3f-109">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="7fa3f-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7fa3f-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7fa3f-110">Attributes and elements</span></span>

<span data-ttu-id="7fa3f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fa3f-112">属性</span><span class="sxs-lookup"><span data-stu-id="7fa3f-112">Attributes</span></span>

<span data-ttu-id="7fa3f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fa3f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7fa3f-114">Child elements</span></span>

<span data-ttu-id="7fa3f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7fa3f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7fa3f-116">Parent elements</span></span>

|<span data-ttu-id="7fa3f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7fa3f-117">**Element**</span></span>|<span data-ttu-id="7fa3f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7fa3f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fa3f-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7fa3f-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="7fa3f-120">1 つの組織の組織との関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7fa3f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7fa3f-121">Text value</span></span>

<span data-ttu-id="7fa3f-122">の**場合は true** 、 **FreeBusyAccessEnabled**要素のテキスト値は、組織内のユーザーの空き時間情報を取得するために共有を使用することを示します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="7fa3f-123">**False**の値は、共有関係を抑制するかを示します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7fa3f-124">備考</span><span class="sxs-lookup"><span data-stu-id="7fa3f-124">Remarks</span></span>

<span data-ttu-id="7fa3f-125">許可するか、サーバーから空き時間情報が表示されないようにするには、この要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="7fa3f-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7fa3f-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="7fa3f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fa3f-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="7fa3f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7fa3f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7fa3f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7fa3f-129">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="7fa3f-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7fa3f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7fa3f-130">Validation File</span></span>  <br/> |<span data-ttu-id="7fa3f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7fa3f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7fa3f-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7fa3f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7fa3f-133">True</span><span class="sxs-lookup"><span data-stu-id="7fa3f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7fa3f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7fa3f-134">See also</span></span>



[<span data-ttu-id="7fa3f-135">GetOrganizationRelationshipSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7fa3f-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

