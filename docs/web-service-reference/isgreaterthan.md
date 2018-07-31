---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: IsGreaterThan 要素をプロパティに定数値または別のプロパティを比較し、最初のプロパティ値が大きい場合に true を返す検索式を表します。
ms.openlocfilehash: dfa7c221bb04e59f1ae12eeb5b9f2e1f09aea3ce
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353491"
---
# <a name="isgreaterthan"></a><span data-ttu-id="b8a3a-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="b8a3a-103">IsGreaterThan</span></span>

<span data-ttu-id="b8a3a-104">**IsGreaterThan**要素は、最初のプロパティ値が大きい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

<span data-ttu-id="b8a3a-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-105">**IsGreaterThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b8a3a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b8a3a-106">Attributes and elements</span></span>

<span data-ttu-id="b8a3a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8a3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8a3a-108">Attributes</span></span>

<span data-ttu-id="b8a3a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8a3a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b8a3a-110">Child elements</span></span>

|<span data-ttu-id="b8a3a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-111">**Element**</span></span>|<span data-ttu-id="b8a3a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a3a-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b8a3a-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b8a3a-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b8a3a-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b8a3a-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b8a3a-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b8a3a-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="b8a3a-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="b8a3a-120">プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8a3a-121">親要素</span><span class="sxs-lookup"><span data-stu-id="b8a3a-121">Parent elements</span></span>

|<span data-ttu-id="b8a3a-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-122">**Element**</span></span>|<span data-ttu-id="b8a3a-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8a3a-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="b8a3a-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="b8a3a-125">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-126">Not</span><span class="sxs-lookup"><span data-stu-id="b8a3a-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="b8a3a-127">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-128">And</span><span class="sxs-lookup"><span data-stu-id="b8a3a-128">And</span></span>](and.md) <br/> |<span data-ttu-id="b8a3a-129">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="b8a3a-130">**And 内に含まれるすべての検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="b8a3a-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="b8a3a-131">Or</span><span class="sxs-lookup"><span data-stu-id="b8a3a-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="b8a3a-132">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="b8a3a-133">[または](or.md) **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8a3a-134">注釈</span><span class="sxs-lookup"><span data-stu-id="b8a3a-134">Remarks</span></span>

<span data-ttu-id="b8a3a-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b8a3a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8a3a-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="b8a3a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8a3a-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="b8a3a-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8a3a-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8a3a-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b8a3a-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8a3a-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8a3a-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8a3a-140">Validation File</span></span>  <br/> |<span data-ttu-id="b8a3a-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8a3a-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8a3a-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b8a3a-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8a3a-143">False</span><span class="sxs-lookup"><span data-stu-id="b8a3a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8a3a-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8a3a-144">See also</span></span>

- [<span data-ttu-id="b8a3a-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b8a3a-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

