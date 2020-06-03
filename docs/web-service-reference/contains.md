---
title: 内容
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Contains 要素は、指定したプロパティに指定の定数文字列値が含まれているかどうかを決定する検索式を表します。
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527118"
---
# <a name="contains"></a><span data-ttu-id="d1ef2-103">内容</span><span class="sxs-lookup"><span data-stu-id="d1ef2-103">Contains</span></span>

<span data-ttu-id="d1ef2-104">**Contains**要素は、指定したプロパティに指定の定数文字列値が含まれているかどうかを決定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


<span data-ttu-id="d1ef2-105">**型**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-105">**ContainsExpressionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d1ef2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d1ef2-106">Attributes and elements</span></span>

<span data-ttu-id="d1ef2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1ef2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1ef2-108">Attributes</span></span>

|<span data-ttu-id="d1ef2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-109">**Attribute**</span></span>|<span data-ttu-id="d1ef2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1ef2-111">**このモード**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="d1ef2-112">検索の境界を識別します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-113">**式の比較**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="d1ef2-114">検索でケースとスペースを無視するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="d1ef2-115">指定した要素の属性値</span><span class="sxs-lookup"><span data-stu-id="d1ef2-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="d1ef2-116">**値**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-116">**Value**</span></span>|<span data-ttu-id="d1ef2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1ef2-118">FullString</span><span class="sxs-lookup"><span data-stu-id="d1ef2-118">FullString</span></span>  <br/> |<span data-ttu-id="d1ef2-119">完全な文字列と定数の間の比較があります。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="d1ef2-120">プロパティの値と指定された定数は正確に同じです。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-121">固定長</span><span class="sxs-lookup"><span data-stu-id="d1ef2-121">Prefixed</span></span>  <br/> |<span data-ttu-id="d1ef2-122">文字列プレフィックスと定数の間に比較があります。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-123">副</span><span class="sxs-lookup"><span data-stu-id="d1ef2-123">Substring</span></span>  <br/> |<span data-ttu-id="d1ef2-124">文字列の部分文字列と定数の間の比較。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="d1ef2-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="d1ef2-126">文字列内の個々の単語のプレフィックスと定数の間の比較が比較されます。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="d1ef2-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="d1ef2-128">文字列内の完全に一致する語句と定数の間に比較があります。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="d1ef2-129">要素の比較属性値</span><span class="sxs-lookup"><span data-stu-id="d1ef2-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="d1ef2-130">**値**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-130">**Value**</span></span>|<span data-ttu-id="d1ef2-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1ef2-132">ニーズ</span><span class="sxs-lookup"><span data-stu-id="d1ef2-132">Exact</span></span>  <br/> |<span data-ttu-id="d1ef2-133">比較は厳密でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="d1ef2-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="d1ef2-135">比較では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-136">Ignorenon文字</span><span class="sxs-lookup"><span data-stu-id="d1ef2-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="d1ef2-137">比較では、スペース以外の文字は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-138">広く</span><span class="sxs-lookup"><span data-stu-id="d1ef2-138">Loose</span></span>  <br/> |<span data-ttu-id="d1ef2-139">を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-140">Ignorecaseandnon文字</span><span class="sxs-lookup"><span data-stu-id="d1ef2-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="d1ef2-141">比較では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="d1ef2-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="d1ef2-143">を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="d1ef2-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="d1ef2-145">を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="d1ef2-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="d1ef2-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="d1ef2-147">を削除します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d1ef2-148">子要素</span><span class="sxs-lookup"><span data-stu-id="d1ef2-148">Child elements</span></span>

|<span data-ttu-id="d1ef2-149">**Element**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-149">**Element**</span></span>|<span data-ttu-id="d1ef2-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1ef2-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d1ef2-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d1ef2-152">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d1ef2-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d1ef2-154">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d1ef2-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d1ef2-156">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-157">定数</span><span class="sxs-lookup"><span data-stu-id="d1ef2-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="d1ef2-158">制限で定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1ef2-159">親要素</span><span class="sxs-lookup"><span data-stu-id="d1ef2-159">Parent elements</span></span>

|<span data-ttu-id="d1ef2-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-160">**Element**</span></span>|<span data-ttu-id="d1ef2-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1ef2-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1ef2-162">制限</span><span class="sxs-lookup"><span data-stu-id="d1ef2-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="d1ef2-163">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-164">Not</span><span class="sxs-lookup"><span data-stu-id="d1ef2-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="d1ef2-165">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-166">And</span><span class="sxs-lookup"><span data-stu-id="d1ef2-166">And</span></span>](and.md) <br/> |<span data-ttu-id="d1ef2-167">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="d1ef2-168">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="d1ef2-169">Or</span><span class="sxs-lookup"><span data-stu-id="d1ef2-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="d1ef2-170">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="d1ef2-171">[または](or.md)のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1ef2-172">注釈</span><span class="sxs-lookup"><span data-stu-id="d1ef2-172">Remarks</span></span>

<span data-ttu-id="d1ef2-173">これらの属性は、要素の照合方法を決定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="d1ef2-174">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d1ef2-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1ef2-175">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d1ef2-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1ef2-176">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1ef2-176">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1ef2-177">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d1ef2-177">Schema Name</span></span>  <br/> |<span data-ttu-id="d1ef2-178">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d1ef2-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1ef2-179">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d1ef2-179">Validation File</span></span>  <br/> |<span data-ttu-id="d1ef2-180">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d1ef2-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1ef2-181">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d1ef2-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1ef2-182">正しくない</span><span class="sxs-lookup"><span data-stu-id="d1ef2-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1ef2-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1ef2-183">See also</span></span>

- [<span data-ttu-id="d1ef2-184">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d1ef2-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

