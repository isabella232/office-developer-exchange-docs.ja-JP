---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: BodyContentAttributedValue 要素は、アイテムの本文の内容を指定します。
ms.openlocfilehash: f5b8f0a19b77ce550b1d7f1c415cc8ee4340863a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759540"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="2d9d0-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2d9d0-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="2d9d0-104">**BodyContentAttributedValue**要素は、アイテムの本文の内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="2d9d0-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="2d9d0-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d9d0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2d9d0-106">Attributes and elements</span></span>

<span data-ttu-id="2d9d0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d9d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d9d0-108">Attributes</span></span>

<span data-ttu-id="2d9d0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d9d0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2d9d0-110">Child elements</span></span>

|<span data-ttu-id="2d9d0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d9d0-111">**Element**</span></span>|<span data-ttu-id="2d9d0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d9d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d9d0-113">値 (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="2d9d0-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="2d9d0-114">**BodyContentAttributedValue**要素の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="2d9d0-115">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="2d9d0-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="2d9d0-116">1 つまたは複数の連絡先や関連するペルソナに集計される active directory の受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d9d0-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2d9d0-117">Parent elements</span></span>

|<span data-ttu-id="2d9d0-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d9d0-118">**Element**</span></span>|<span data-ttu-id="2d9d0-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d9d0-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d9d0-120">ボディ</span><span class="sxs-lookup"><span data-stu-id="2d9d0-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="2d9d0-121">**BodyContentAttributedValue**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d9d0-122">備考</span><span class="sxs-lookup"><span data-stu-id="2d9d0-122">Remarks</span></span>

<span data-ttu-id="2d9d0-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2d9d0-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d9d0-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="2d9d0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d9d0-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="2d9d0-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d9d0-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d9d0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2d9d0-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2d9d0-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="2d9d0-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d9d0-129">Validation File</span></span>  <br/> |<span data-ttu-id="2d9d0-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d9d0-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d9d0-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2d9d0-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2d9d0-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d9d0-132">See also</span></span>



- [<span data-ttu-id="2d9d0-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2d9d0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

