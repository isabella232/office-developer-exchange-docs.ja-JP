---
title: IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: IsEqualTo 要素は、プロパティを定数値または別のプロパティと比較し、等しい場合は true に評価される検索式を表します。
ms.openlocfilehash: 857192443ab0520bb26ead399bc5364cc862a4fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455297"
---
# <a name="isequalto"></a><span data-ttu-id="49743-103">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="49743-103">IsEqualTo</span></span>

<span data-ttu-id="49743-104">**IsEqualTo**要素は、プロパティを定数値または別のプロパティと比較し、等しい場合は true に評価される検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="49743-104">The **IsEqualTo** element represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span> 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsEqualTo>
```

<span data-ttu-id="49743-105">**IsEqualToType**</span><span class="sxs-lookup"><span data-stu-id="49743-105">**IsEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49743-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="49743-106">Attributes and elements</span></span>

<span data-ttu-id="49743-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49743-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49743-108">属性</span><span class="sxs-lookup"><span data-stu-id="49743-108">Attributes</span></span>

<span data-ttu-id="49743-109">なし。</span><span class="sxs-lookup"><span data-stu-id="49743-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49743-110">子要素</span><span class="sxs-lookup"><span data-stu-id="49743-110">Child elements</span></span>

|<span data-ttu-id="49743-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="49743-111">**Element**</span></span>|<span data-ttu-id="49743-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="49743-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49743-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="49743-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="49743-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="49743-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="49743-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="49743-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="49743-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="49743-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="49743-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="49743-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="49743-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="49743-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="49743-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="49743-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="49743-120">別のプロパティと比較するときに使用するプロパティまたは定数の値を表します。</span><span class="sxs-lookup"><span data-stu-id="49743-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49743-121">親要素</span><span class="sxs-lookup"><span data-stu-id="49743-121">Parent elements</span></span>

|<span data-ttu-id="49743-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="49743-122">**Element**</span></span>|<span data-ttu-id="49743-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="49743-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49743-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="49743-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="49743-125">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="49743-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="49743-126">Not</span><span class="sxs-lookup"><span data-stu-id="49743-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="49743-127">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="49743-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="49743-128">And</span><span class="sxs-lookup"><span data-stu-id="49743-128">And</span></span>](and.md) <br/> |<span data-ttu-id="49743-129">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="49743-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="49743-130">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="49743-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="49743-131">Or</span><span class="sxs-lookup"><span data-stu-id="49743-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="49743-132">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="49743-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="49743-133">[または](or.md)、いずれかの子が true を返した場合は true を返します。</span><span class="sxs-lookup"><span data-stu-id="49743-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="49743-134">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="49743-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49743-135">注釈</span><span class="sxs-lookup"><span data-stu-id="49743-135">Remarks</span></span>

<span data-ttu-id="49743-136">文字列比較を実行するには、 [Contains](contains.md)要素を使用することを検討します。大文字と小文字を区別するためのオプションを提供します。</span><span class="sxs-lookup"><span data-stu-id="49743-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters, such as case and white space.</span></span> <span data-ttu-id="49743-137">[Not](not.md)要素を Contains 要素と組み合わせ[て](contains.md)使用し、結果を否定します。</span><span class="sxs-lookup"><span data-stu-id="49743-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="49743-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="49743-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49743-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="49743-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49743-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="49743-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49743-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49743-141">Schema Name</span></span>  <br/> |<span data-ttu-id="49743-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="49743-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="49743-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49743-143">Validation File</span></span>  <br/> |<span data-ttu-id="49743-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="49743-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49743-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49743-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="49743-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="49743-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49743-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="49743-147">See also</span></span>

- [<span data-ttu-id="49743-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="49743-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

