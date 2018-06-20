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
ms.openlocfilehash: 92e4ec7f192ccb36ea68d7862e66cb7b3349819a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760411"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="23b53-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="23b53-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="23b53-104">**ExtendedPropertyAttributedValue**要素は、ペルソナの拡張プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="23b53-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="23b53-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="23b53-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23b53-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="23b53-106">Attributes and elements</span></span>

<span data-ttu-id="23b53-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23b53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23b53-108">属性</span><span class="sxs-lookup"><span data-stu-id="23b53-108">Attributes</span></span>

<span data-ttu-id="23b53-109">なし。</span><span class="sxs-lookup"><span data-stu-id="23b53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23b53-110">子要素</span><span class="sxs-lookup"><span data-stu-id="23b53-110">Child elements</span></span>

|<span data-ttu-id="23b53-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="23b53-111">**Element**</span></span>|<span data-ttu-id="23b53-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="23b53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23b53-113">値 (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="23b53-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="23b53-114">ペルソナの拡張プロパティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="23b53-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="23b53-115">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="23b53-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="23b53-116">帰属、関連付けられている**値**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="23b53-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23b53-117">親要素</span><span class="sxs-lookup"><span data-stu-id="23b53-117">Parent elements</span></span>

|<span data-ttu-id="23b53-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="23b53-118">**Element**</span></span>|<span data-ttu-id="23b53-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="23b53-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23b53-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="23b53-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="23b53-121">統合連絡先ストアの操作に使用される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="23b53-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23b53-122">備考</span><span class="sxs-lookup"><span data-stu-id="23b53-122">Remarks</span></span>

<span data-ttu-id="23b53-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="23b53-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23b53-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="23b53-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23b53-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="23b53-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23b53-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="23b53-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23b53-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23b53-127">Schema Name</span></span>  <br/> |<span data-ttu-id="23b53-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="23b53-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="23b53-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23b53-129">Validation File</span></span>  <br/> |<span data-ttu-id="23b53-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="23b53-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="23b53-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="23b53-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="23b53-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="23b53-132">See also</span></span>



- [<span data-ttu-id="23b53-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="23b53-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

