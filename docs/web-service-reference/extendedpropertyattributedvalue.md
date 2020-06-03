---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: ExtendedPropertyAttributedValue 要素は、ペルソナの拡張プロパティを指定します。
ms.openlocfilehash: 5c2ad5918d7ac666d5e26af6597b2c4c3dde6202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460128"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="89720-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="89720-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="89720-104">**ExtendedPropertyAttributedValue**要素は、ペルソナの拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="89720-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="89720-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="89720-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89720-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="89720-106">Attributes and elements</span></span>

<span data-ttu-id="89720-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89720-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89720-108">属性</span><span class="sxs-lookup"><span data-stu-id="89720-108">Attributes</span></span>

<span data-ttu-id="89720-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89720-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89720-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89720-110">Child elements</span></span>

|<span data-ttu-id="89720-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="89720-111">**Element**</span></span>|<span data-ttu-id="89720-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="89720-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89720-113">Value (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="89720-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="89720-114">ペルソナの拡張プロパティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="89720-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="89720-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="89720-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="89720-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="89720-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89720-117">親要素</span><span class="sxs-lookup"><span data-stu-id="89720-117">Parent elements</span></span>

|<span data-ttu-id="89720-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="89720-118">**Element**</span></span>|<span data-ttu-id="89720-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="89720-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89720-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="89720-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="89720-121">統合連絡先ストアの操作に使用される拡張プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="89720-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89720-122">注釈</span><span class="sxs-lookup"><span data-stu-id="89720-122">Remarks</span></span>

<span data-ttu-id="89720-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="89720-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89720-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="89720-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89720-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="89720-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89720-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="89720-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89720-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89720-127">Schema Name</span></span>  <br/> |<span data-ttu-id="89720-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="89720-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="89720-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89720-129">Validation File</span></span>  <br/> |<span data-ttu-id="89720-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="89720-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="89720-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="89720-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="89720-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="89720-132">See also</span></span>



- [<span data-ttu-id="89720-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="89720-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

