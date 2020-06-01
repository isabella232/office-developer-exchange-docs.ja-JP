---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: 並べ替え要素は、FindItem または FindConversation 会話要求でアイテムを並べ替える方法を定義します。
ms.openlocfilehash: b520bb3ca6daadc777e7235b2b7420a12e425048
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468370"
---
# <a name="sortorder"></a><span data-ttu-id="a072d-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="a072d-103">SortOrder</span></span>

<span data-ttu-id="a072d-104">並べ替え**要素は**、 **FindItem**または**findconversation 会話**要求でアイテムを並べ替える方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="a072d-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="a072d-105">**NonEmptyArrayOfFieldOrdersType**</span><span class="sxs-lookup"><span data-stu-id="a072d-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a072d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a072d-106">Attributes and elements</span></span>

<span data-ttu-id="a072d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a072d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a072d-108">属性</span><span class="sxs-lookup"><span data-stu-id="a072d-108">Attributes</span></span>

<span data-ttu-id="a072d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a072d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a072d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a072d-110">Child elements</span></span>

|<span data-ttu-id="a072d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="a072d-111">**Element**</span></span>|<span data-ttu-id="a072d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a072d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a072d-113">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="a072d-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="a072d-114">結果を並べ替えるための1つのフィールドを表し、並べ替えの方向を示します。</span><span class="sxs-lookup"><span data-stu-id="a072d-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="a072d-115">これらの要素の1つ以上を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a072d-115">One or more of these elements may be included.</span></span> <span data-ttu-id="a072d-116">[Fieldorder](fieldorder.md)要素は、並べ替えに指定された順序で適用されます。</span><span class="sxs-lookup"><span data-stu-id="a072d-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a072d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="a072d-117">Parent elements</span></span>

|<span data-ttu-id="a072d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="a072d-118">**Element**</span></span>|<span data-ttu-id="a072d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="a072d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a072d-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="a072d-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="a072d-121">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="a072d-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="a072d-122">この要素の XPath 式を次に示します。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="a072d-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="a072d-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="a072d-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="a072d-124">メールボックス内のスレッドを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="a072d-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a072d-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a072d-125">Text value</span></span>

<span data-ttu-id="a072d-126">なし。</span><span class="sxs-lookup"><span data-stu-id="a072d-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a072d-127">注釈</span><span class="sxs-lookup"><span data-stu-id="a072d-127">Remarks</span></span>

<span data-ttu-id="a072d-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a072d-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a072d-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a072d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a072d-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="a072d-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a072d-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a072d-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a072d-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a072d-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a072d-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a072d-133">Validation File</span></span>  <br/> |<span data-ttu-id="a072d-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a072d-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a072d-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a072d-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a072d-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="a072d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a072d-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="a072d-137">See also</span></span>



[<span data-ttu-id="a072d-138">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="a072d-138">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="a072d-139">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="a072d-139">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="a072d-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a072d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

