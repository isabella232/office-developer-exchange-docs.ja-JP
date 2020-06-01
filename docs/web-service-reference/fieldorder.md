---
title: FieldOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldOrder
api_type:
- schema
ms.assetid: b9364842-bbe2-4221-afef-bf5022bc89ec
description: FieldOrder 要素は、結果を並べ替えるための1つのフィールドを表し、並べ替えの方向を示します。
ms.openlocfilehash: 19dee7175d541dd99b53e004ea8ccd785b619184
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461262"
---
# <a name="fieldorder"></a><span data-ttu-id="2cfb6-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="2cfb6-103">FieldOrder</span></span>

<span data-ttu-id="2cfb6-104">**Fieldorder**要素は、結果を並べ替えるための1つのフィールドを表し、並べ替えの方向を示します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <ExtendedFieldURI/> 
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <IndexedFieldURI/>
</FieldOrder>
```

<span data-ttu-id="2cfb6-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-105">**FieldOrderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2cfb6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2cfb6-106">Attributes and elements</span></span>

<span data-ttu-id="2cfb6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cfb6-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cfb6-108">Attributes</span></span>

|<span data-ttu-id="2cfb6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-109">**Attribute**</span></span>|<span data-ttu-id="2cfb6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2cfb6-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-111">**Order**</span></span> <br/> | <span data-ttu-id="2cfb6-112">並べ替え順序の方向を表します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="2cfb6-113">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="2cfb6-114">-昇順</span><span class="sxs-lookup"><span data-stu-id="2cfb6-114">-  Ascending</span></span>  <br/><span data-ttu-id="2cfb6-115">-降順</span><span class="sxs-lookup"><span data-stu-id="2cfb6-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2cfb6-116">子要素</span><span class="sxs-lookup"><span data-stu-id="2cfb6-116">Child elements</span></span>

|<span data-ttu-id="2cfb6-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-117">**Element**</span></span>|<span data-ttu-id="2cfb6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cfb6-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2cfb6-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="2cfb6-120">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="2cfb6-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2cfb6-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="2cfb6-122">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="2cfb6-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="2cfb6-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="2cfb6-124">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cfb6-125">親要素</span><span class="sxs-lookup"><span data-stu-id="2cfb6-125">Parent elements</span></span>

|<span data-ttu-id="2cfb6-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-126">**Element**</span></span>|<span data-ttu-id="2cfb6-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cfb6-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cfb6-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="2cfb6-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="2cfb6-129">FindItem 要求でのアイテムの並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="2cfb6-130">この要素の XPath 式を次に示します。`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="2cfb6-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2cfb6-131">注釈</span><span class="sxs-lookup"><span data-stu-id="2cfb6-131">Remarks</span></span>

<span data-ttu-id="2cfb6-132">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cfb6-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2cfb6-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cfb6-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="2cfb6-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cfb6-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2cfb6-135">Schema Name</span></span>  <br/> |<span data-ttu-id="2cfb6-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2cfb6-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cfb6-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2cfb6-137">Validation File</span></span>  <br/> |<span data-ttu-id="2cfb6-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2cfb6-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cfb6-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2cfb6-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cfb6-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="2cfb6-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cfb6-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cfb6-141">See also</span></span>

- [<span data-ttu-id="2cfb6-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2cfb6-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

