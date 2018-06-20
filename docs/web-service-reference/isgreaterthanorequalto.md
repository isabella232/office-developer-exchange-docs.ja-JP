---
title: IsGreaterThanOrEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThanOrEqualTo
api_type:
- schema
ms.assetid: 373cc954-314d-40e2-be03-cc08aefc0d5b
description: IsGreaterThanOrEqualTo 要素は、定数値または別のプロパティと 2 つ目と同じかよりも大きい場合は、最初のプロパティに true を返しますのいずれかのプロパティを比較する検索式を表します。
ms.openlocfilehash: 81df79d15e6c5c8d301e69a822d038588ce42325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832030"
---
# <a name="isgreaterthanorequalto"></a><span data-ttu-id="afa53-103">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="afa53-103">IsGreaterThanOrEqualTo</span></span>

<span data-ttu-id="afa53-104">**IsGreaterThanOrEqualTo**要素は、最初のプロパティには、もう 1 つ以上の場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-104">The **IsGreaterThanOrEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the second.</span></span> 
  
```xml
<IsGreaterThanOrEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThanOrEqualTo>
```

 <span data-ttu-id="afa53-105">**IsGreaterThanOrEqualToType**</span><span class="sxs-lookup"><span data-stu-id="afa53-105">**IsGreaterThanOrEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afa53-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="afa53-106">Attributes and elements</span></span>

<span data-ttu-id="afa53-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afa53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afa53-108">属性</span><span class="sxs-lookup"><span data-stu-id="afa53-108">Attributes</span></span>

<span data-ttu-id="afa53-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afa53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afa53-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afa53-110">Child elements</span></span>

|<span data-ttu-id="afa53-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="afa53-111">**Element**</span></span>|<span data-ttu-id="afa53-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="afa53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afa53-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="afa53-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="afa53-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="afa53-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="afa53-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="afa53-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="afa53-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="afa53-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="afa53-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="afa53-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="afa53-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="afa53-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="afa53-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="afa53-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="afa53-120">プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="afa53-121">親要素</span><span class="sxs-lookup"><span data-stu-id="afa53-121">Parent elements</span></span>

|<span data-ttu-id="afa53-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="afa53-122">**Element**</span></span>|<span data-ttu-id="afa53-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="afa53-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afa53-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="afa53-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="afa53-125">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="afa53-126">Not</span><span class="sxs-lookup"><span data-stu-id="afa53-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="afa53-127">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-127">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="afa53-128">And</span><span class="sxs-lookup"><span data-stu-id="afa53-128">And</span></span>](and.md) <br/> |<span data-ttu-id="afa53-129">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="afa53-130">**すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="afa53-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="afa53-131">Or</span><span class="sxs-lookup"><span data-stu-id="afa53-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="afa53-132">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="afa53-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="afa53-133">[または](or.md)その子のいずれかの場合は true を返す場合は true。 戻ります。</span><span class="sxs-lookup"><span data-stu-id="afa53-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="afa53-134">[または](or.md)2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="afa53-134">[Or](or.md) must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afa53-135">備考</span><span class="sxs-lookup"><span data-stu-id="afa53-135">Remarks</span></span>

<span data-ttu-id="afa53-136">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="afa53-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afa53-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="afa53-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afa53-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="afa53-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afa53-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afa53-139">Schema Name</span></span>  <br/> |<span data-ttu-id="afa53-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="afa53-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="afa53-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afa53-141">Validation File</span></span>  <br/> |<span data-ttu-id="afa53-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afa53-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afa53-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afa53-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="afa53-144">False</span><span class="sxs-lookup"><span data-stu-id="afa53-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afa53-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="afa53-145">See also</span></span>



- [<span data-ttu-id="afa53-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="afa53-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

