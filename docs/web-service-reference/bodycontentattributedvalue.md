---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: BodyContentAttributedValue 要素は、アイテムの本文のコンテンツを指定します。
ms.openlocfilehash: 3550d9307e9bd652afc217f72610379a0a5b2f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527398"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="b3b37-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b3b37-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="b3b37-104">**BodyContentAttributedValue**要素は、アイテムの本文のコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="b3b37-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="b3b37-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="b3b37-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3b37-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b3b37-106">Attributes and elements</span></span>

<span data-ttu-id="b3b37-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b3b37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3b37-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3b37-108">Attributes</span></span>

<span data-ttu-id="b3b37-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b3b37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3b37-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b3b37-110">Child elements</span></span>

|<span data-ttu-id="b3b37-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b3b37-111">**Element**</span></span>|<span data-ttu-id="b3b37-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3b37-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b37-113">Value (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="b3b37-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="b3b37-114">**BodyContentAttributedValue**要素の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3b37-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="b3b37-115">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="b3b37-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="b3b37-116">関連付けられたペルソナに集約される1つ以上の連絡先または active directory 受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3b37-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3b37-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b3b37-117">Parent elements</span></span>

|<span data-ttu-id="b3b37-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b3b37-118">**Element**</span></span>|<span data-ttu-id="b3b37-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b3b37-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b37-120">本文</span><span class="sxs-lookup"><span data-stu-id="b3b37-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="b3b37-121">**BodyContentAttributedValue**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3b37-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b3b37-122">注釈</span><span class="sxs-lookup"><span data-stu-id="b3b37-122">Remarks</span></span>

<span data-ttu-id="b3b37-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b3b37-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b3b37-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b3b37-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3b37-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b3b37-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3b37-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b3b37-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3b37-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b3b37-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b3b37-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="b3b37-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="b3b37-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b3b37-129">Validation File</span></span>  <br/> |<span data-ttu-id="b3b37-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b3b37-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3b37-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b3b37-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b3b37-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="b3b37-132">See also</span></span>



- [<span data-ttu-id="b3b37-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b3b37-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

