---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: FreeBusyAccessEnabled 要素は、FreeBusyAccessEnabled () フラグを表します。 FreeBusyAccessEnabled 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461297"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="b9a99-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9a99-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="b9a99-106">**FreeBusyAccessEnabled**要素は、 **FreeBusyAccessEnabled ()** フラグを表します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="b9a99-107">**FreeBusyAccessEnabled**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="b9a99-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="b9a99-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="b9a99-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="b9a99-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b9a99-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9a99-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b9a99-110">Attributes and elements</span></span>

<span data-ttu-id="b9a99-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9a99-112">属性</span><span class="sxs-lookup"><span data-stu-id="b9a99-112">Attributes</span></span>

<span data-ttu-id="b9a99-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a99-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9a99-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b9a99-114">Child elements</span></span>

<span data-ttu-id="b9a99-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b9a99-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9a99-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b9a99-116">Parent elements</span></span>

|<span data-ttu-id="b9a99-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b9a99-117">**Element**</span></span>|<span data-ttu-id="b9a99-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b9a99-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a99-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9a99-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="b9a99-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9a99-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b9a99-121">Text value</span></span>

<span data-ttu-id="b9a99-122">**FreeBusyAccessEnabled**要素のテキスト値が**true**の場合は、共有関係を使用して、組織内のユーザーから空き時間情報を取得する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="b9a99-123">値が**false**の場合は、共有リレーションシップを抑制する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b9a99-124">注釈</span><span class="sxs-lookup"><span data-stu-id="b9a99-124">Remarks</span></span>

<span data-ttu-id="b9a99-125">この要素を使用して、サーバーからの空き時間情報を許可または抑制します。</span><span class="sxs-lookup"><span data-stu-id="b9a99-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b9a99-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b9a99-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9a99-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9a99-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b9a99-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b9a99-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9a99-129">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="b9a99-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b9a99-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b9a99-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9a99-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b9a99-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9a99-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b9a99-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9a99-133">正しい</span><span class="sxs-lookup"><span data-stu-id="b9a99-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9a99-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9a99-134">See also</span></span>



[<span data-ttu-id="b9a99-135">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9a99-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

