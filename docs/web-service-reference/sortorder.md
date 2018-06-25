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
description: SortOrder 要素は、FindItem または FindConversation の要求の項目の並べ替え方法を定義します。
ms.openlocfilehash: e20e5eab7972616c90079786abd78a0f7fedfebe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833519"
---
# <a name="sortorder"></a><span data-ttu-id="ba275-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="ba275-103">SortOrder</span></span>

<span data-ttu-id="ba275-104">**SortOrder**要素は、 **FindItem**または**FindConversation**の要求の項目の並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="ba275-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="ba275-105">**NonEmptyArrayOfFieldOrdersType**</span><span class="sxs-lookup"><span data-stu-id="ba275-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba275-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ba275-106">Attributes and elements</span></span>

<span data-ttu-id="ba275-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba275-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba275-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba275-108">Attributes</span></span>

<span data-ttu-id="ba275-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ba275-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba275-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ba275-110">Child elements</span></span>

|<span data-ttu-id="ba275-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ba275-111">**Element**</span></span>|<span data-ttu-id="ba275-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba275-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba275-113">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="ba275-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="ba275-114">結果の並べ替えに使用する単一のフィールドを表し、並べ替えの方向を示します。</span><span class="sxs-lookup"><span data-stu-id="ba275-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="ba275-115">これらの要素の 1 つ以上が含まれている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ba275-115">One or more of these elements may be included.</span></span> <span data-ttu-id="ba275-116">[FieldOrder](fieldorder.md)要素は、並べ替えの指定された順序で適用されます。</span><span class="sxs-lookup"><span data-stu-id="ba275-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba275-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ba275-117">Parent elements</span></span>

|<span data-ttu-id="ba275-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ba275-118">**Element**</span></span>|<span data-ttu-id="ba275-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba275-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba275-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="ba275-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ba275-121">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ba275-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="ba275-122">この要素への XPath 式は、次のようにします。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="ba275-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="ba275-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="ba275-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="ba275-124">メールボックス内の会話を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ba275-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba275-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ba275-125">Text value</span></span>

<span data-ttu-id="ba275-126">なし。</span><span class="sxs-lookup"><span data-stu-id="ba275-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba275-127">備考</span><span class="sxs-lookup"><span data-stu-id="ba275-127">Remarks</span></span>

<span data-ttu-id="ba275-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ba275-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba275-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="ba275-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba275-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="ba275-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba275-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba275-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ba275-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ba275-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba275-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba275-133">Validation File</span></span>  <br/> |<span data-ttu-id="ba275-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ba275-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba275-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ba275-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba275-136">False</span><span class="sxs-lookup"><span data-stu-id="ba275-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba275-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba275-137">See also</span></span>



<span data-ttu-id="ba275-138">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="ba275-138">[FindItem operation](finditem-operation.md)</span></span>
  
<span data-ttu-id="ba275-139">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="ba275-139">[FindConversation operation](findconversation-operation.md)</span></span>


- [<span data-ttu-id="ba275-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ba275-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

