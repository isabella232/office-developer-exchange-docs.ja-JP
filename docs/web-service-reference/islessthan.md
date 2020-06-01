---
title: IsLessThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsLessThan
api_type:
- schema
ms.assetid: 2550469b-6e5d-45a5-9ecc-090d1b409296
description: Isless from 要素は、プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目のプロパティより小さい場合に true を返す検索式を表します。
ms.openlocfilehash: d68cd3e049b95b4a6ba3e6ef841514ab59e60425
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464197"
---
# <a name="islessthan"></a><span data-ttu-id="63789-103">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="63789-103">IsLessThan</span></span>

<span data-ttu-id="63789-104">**Isless** from 要素は、プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目のプロパティより小さい場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63789-104">The **IsLessThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the second.</span></span> 
  
```xml
<IsLessThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsLessThan>
```

```xml
<IsLessThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsLessThan>
```

```xml
<IsLessThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsLessThan>
```

<span data-ttu-id="63789-105">**Isna/型**</span><span class="sxs-lookup"><span data-stu-id="63789-105">**IsLessThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63789-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63789-106">Attributes and elements</span></span>

<span data-ttu-id="63789-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63789-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63789-108">属性</span><span class="sxs-lookup"><span data-stu-id="63789-108">Attributes</span></span>

<span data-ttu-id="63789-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63789-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63789-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63789-110">Child elements</span></span>

|<span data-ttu-id="63789-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="63789-111">**Element**</span></span>|<span data-ttu-id="63789-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63789-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63789-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="63789-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="63789-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="63789-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="63789-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="63789-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="63789-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="63789-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="63789-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="63789-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="63789-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="63789-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="63789-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="63789-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="63789-120">別のプロパティと比較するときに使用するプロパティまたは定数の値を表します。</span><span class="sxs-lookup"><span data-stu-id="63789-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63789-121">親要素</span><span class="sxs-lookup"><span data-stu-id="63789-121">Parent elements</span></span>

|<span data-ttu-id="63789-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="63789-122">**Element**</span></span>|<span data-ttu-id="63789-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="63789-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63789-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="63789-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="63789-125">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="63789-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="63789-126">Not</span><span class="sxs-lookup"><span data-stu-id="63789-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="63789-127">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63789-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="63789-128">And</span><span class="sxs-lookup"><span data-stu-id="63789-128">And</span></span>](and.md) <br/> |<span data-ttu-id="63789-129">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63789-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="63789-130">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="63789-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="63789-131">Or</span><span class="sxs-lookup"><span data-stu-id="63789-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="63789-132">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63789-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="63789-133">[または](or.md)、いずれかの子が true を返した場合は true を返します。</span><span class="sxs-lookup"><span data-stu-id="63789-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="63789-134">[または、](or.md) 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="63789-134">[Or](or.md) must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63789-135">注釈</span><span class="sxs-lookup"><span data-stu-id="63789-135">Remarks</span></span>

<span data-ttu-id="63789-136">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="63789-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63789-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63789-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63789-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="63789-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63789-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63789-139">Schema Name</span></span>  <br/> |<span data-ttu-id="63789-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="63789-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="63789-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63789-141">Validation File</span></span>  <br/> |<span data-ttu-id="63789-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="63789-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63789-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63789-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="63789-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="63789-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63789-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="63789-145">See also</span></span>

- [<span data-ttu-id="63789-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="63789-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

