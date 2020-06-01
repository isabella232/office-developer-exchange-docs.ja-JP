---
title: FreeBusyAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a287b9c3-7fb6-4f2f-a8dc-15d4bc32394c
description: FreeBusyAccessLevel 要素は、FreeBusyAccessLevel プロパティを表します。 FreeBusyAccessLevel 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 7ff0c6c72f924a2f1f8eee0dd152d19f6a8745e9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460051"
---
# <a name="freebusyaccesslevel-soap"></a><span data-ttu-id="a2fa3-105">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2fa3-105">FreeBusyAccessLevel (SOAP)</span></span>

<span data-ttu-id="a2fa3-106">**FreeBusyAccessLevel**要素は、 **FreeBusyAccessLevel**プロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-106">The **FreeBusyAccessLevel** element represents the **FreeBusyAccessLevel** property.</span></span> <span data-ttu-id="a2fa3-107">**FreeBusyAccessLevel**要素は、内部使用のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-107">The **FreeBusyAccessLevel** element is for internal use only.</span></span> <span data-ttu-id="a2fa3-108">この要素はクライアントによって使用されません。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessLevel/>
```

 <span data-ttu-id="a2fa3-109">**string**</span><span class="sxs-lookup"><span data-stu-id="a2fa3-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2fa3-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a2fa3-110">Attributes and elements</span></span>

<span data-ttu-id="a2fa3-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2fa3-112">属性</span><span class="sxs-lookup"><span data-stu-id="a2fa3-112">Attributes</span></span>

<span data-ttu-id="a2fa3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2fa3-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a2fa3-114">Child elements</span></span>

<span data-ttu-id="a2fa3-115">なし。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2fa3-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a2fa3-116">Parent elements</span></span>

|<span data-ttu-id="a2fa3-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="a2fa3-117">**Element**</span></span>|<span data-ttu-id="a2fa3-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2fa3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fa3-119">組織のリレーションシップ設定 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2fa3-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="a2fa3-120">1つの組織の組織上の関係のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2fa3-121">注釈</span><span class="sxs-lookup"><span data-stu-id="a2fa3-121">Remarks</span></span>

<span data-ttu-id="a2fa3-122">この要素は、応答で返される空き時間情報の最大量を指定し、外部共有されている空き時間情報データのレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="a2fa3-122">This element specifies the maximum amount of free/busy detail that will be returned in the response and indicates the level of free/busy data that is externally shared.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a2fa3-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a2fa3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2fa3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2fa3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a2fa3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a2fa3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a2fa3-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="a2fa3-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a2fa3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a2fa3-127">Validation File</span></span>  <br/> |<span data-ttu-id="a2fa3-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a2fa3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2fa3-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a2fa3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2fa3-130">正しい</span><span class="sxs-lookup"><span data-stu-id="a2fa3-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2fa3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2fa3-131">See also</span></span>



[<span data-ttu-id="a2fa3-132">Get組織の Relationshipsettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a2fa3-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

