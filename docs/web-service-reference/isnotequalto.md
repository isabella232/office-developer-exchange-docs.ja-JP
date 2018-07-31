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
description: IsNotEqualTo 要素をプロパティに定数値または別のプロパティを比較し、値が同じではない場合は true を返す検索式を表します。
ms.openlocfilehash: 75b580d97fbadbf3aa28c29159973f53768df624
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353253"
---
# <a name="isnotequalto"></a><span data-ttu-id="b67c2-103">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="b67c2-103">IsNotEqualTo</span></span>

<span data-ttu-id="b67c2-104">**IsNotEqualTo**要素は、値が同じではない場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
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

<span data-ttu-id="b67c2-105">**IsNotEqualToType**</span><span class="sxs-lookup"><span data-stu-id="b67c2-105">**IsNotEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b67c2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b67c2-106">Attributes and elements</span></span>

<span data-ttu-id="b67c2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b67c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b67c2-108">Attributes</span></span>

<span data-ttu-id="b67c2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b67c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b67c2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b67c2-110">Child elements</span></span>

|<span data-ttu-id="b67c2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b67c2-111">**Element**</span></span>|<span data-ttu-id="b67c2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b67c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b67c2-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b67c2-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b67c2-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b67c2-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b67c2-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b67c2-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b67c2-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="b67c2-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="b67c2-120">プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b67c2-121">親要素</span><span class="sxs-lookup"><span data-stu-id="b67c2-121">Parent elements</span></span>

|<span data-ttu-id="b67c2-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="b67c2-122">**Element**</span></span>|<span data-ttu-id="b67c2-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="b67c2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b67c2-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="b67c2-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="b67c2-125">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-126">Not</span><span class="sxs-lookup"><span data-stu-id="b67c2-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="b67c2-127">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-128">And</span><span class="sxs-lookup"><span data-stu-id="b67c2-128">And</span></span>](and.md) <br/> |<span data-ttu-id="b67c2-129">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="b67c2-130">**すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="b67c2-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="b67c2-131">Or</span><span class="sxs-lookup"><span data-stu-id="b67c2-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="b67c2-132">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="b67c2-133">[または](or.md) **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="b67c2-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="b67c2-134">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="b67c2-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b67c2-135">注釈</span><span class="sxs-lookup"><span data-stu-id="b67c2-135">Remarks</span></span>

<span data-ttu-id="b67c2-136">文字列比較を実行するには、検討、[含まれる](contains.md)要素を使用する大文字と小文字や空白文字などの対応するパラメーターのオプションが用意されています。</span><span class="sxs-lookup"><span data-stu-id="b67c2-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="b67c2-137">結果の符号を反転するのに[含まれる](contains.md)要素と共に、要素では[なく](not.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="b67c2-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="b67c2-138">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b67c2-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b67c2-139">要素情報</span><span class="sxs-lookup"><span data-stu-id="b67c2-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b67c2-140">名前空間</span><span class="sxs-lookup"><span data-stu-id="b67c2-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b67c2-141">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b67c2-141">Schema Name</span></span>  <br/> |<span data-ttu-id="b67c2-142">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b67c2-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="b67c2-143">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b67c2-143">Validation File</span></span>  <br/> |<span data-ttu-id="b67c2-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b67c2-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b67c2-145">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b67c2-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="b67c2-146">False</span><span class="sxs-lookup"><span data-stu-id="b67c2-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b67c2-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="b67c2-147">See also</span></span>

- [<span data-ttu-id="b67c2-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b67c2-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

