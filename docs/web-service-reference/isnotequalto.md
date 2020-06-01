---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: IsNotEqualTo 要素は、プロパティを定数値または別のプロパティと比較し、値が同じでない場合は true を返す検索式を表します。
ms.openlocfilehash: 8c40fd1ce8c7c1f14b70f4fccfd3a24e4c99f1b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464190"
---
# <a name="isnotequalto"></a><span data-ttu-id="fe6ef-103">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="fe6ef-103">IsNotEqualTo</span></span>

<span data-ttu-id="fe6ef-104">**IsNotEqualTo**要素は、プロパティを定数値または別のプロパティと比較し、値が同じでない場合は**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <IndexedFieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

<span data-ttu-id="fe6ef-105">**IsNotEqualToType**</span><span class="sxs-lookup"><span data-stu-id="fe6ef-105">**IsNotEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fe6ef-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fe6ef-106">Attributes and elements</span></span>

<span data-ttu-id="fe6ef-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe6ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe6ef-108">Attributes</span></span>

<span data-ttu-id="fe6ef-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe6ef-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fe6ef-110">Child elements</span></span>

|<span data-ttu-id="fe6ef-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="fe6ef-111">**Element**</span></span>|<span data-ttu-id="fe6ef-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe6ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe6ef-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="fe6ef-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="fe6ef-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fe6ef-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="fe6ef-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fe6ef-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="fe6ef-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="fe6ef-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="fe6ef-120">別のプロパティと比較するときに使用するプロパティまたは定数の値を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fe6ef-121">親要素</span><span class="sxs-lookup"><span data-stu-id="fe6ef-121">Parent elements</span></span>

|<span data-ttu-id="fe6ef-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="fe6ef-122">**Element**</span></span>|<span data-ttu-id="fe6ef-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="fe6ef-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe6ef-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="fe6ef-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="fe6ef-125">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-126">Not</span><span class="sxs-lookup"><span data-stu-id="fe6ef-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="fe6ef-127">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-128">And</span><span class="sxs-lookup"><span data-stu-id="fe6ef-128">And</span></span>](and.md) <br/> |<span data-ttu-id="fe6ef-129">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="fe6ef-130">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="fe6ef-131">Or</span><span class="sxs-lookup"><span data-stu-id="fe6ef-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="fe6ef-132">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="fe6ef-133">[または](or.md)、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="fe6ef-134">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fe6ef-135">注釈</span><span class="sxs-lookup"><span data-stu-id="fe6ef-135">Remarks</span></span>

<span data-ttu-id="fe6ef-136">文字列比較を実行するには、大文字と小文字を区別するためのオプションを提供するので、 [Contains](contains.md)要素の使用を検討してください。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="fe6ef-137">[Not](not.md)要素を Contains 要素と組み合わせ[て](contains.md)使用し、結果を否定します。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="fe6ef-138">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fe6ef-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe6ef-139">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fe6ef-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe6ef-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="fe6ef-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fe6ef-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fe6ef-141">Schema Name</span></span>  <br/> |<span data-ttu-id="fe6ef-142">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fe6ef-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="fe6ef-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fe6ef-143">Validation File</span></span>  <br/> |<span data-ttu-id="fe6ef-144">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fe6ef-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fe6ef-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fe6ef-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe6ef-146">正しくない</span><span class="sxs-lookup"><span data-stu-id="fe6ef-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe6ef-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="fe6ef-147">See also</span></span>

- [<span data-ttu-id="fe6ef-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fe6ef-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

