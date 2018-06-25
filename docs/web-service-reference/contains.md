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
description: 含まれる要素は、指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759700"
---
# <a name="contains"></a><span data-ttu-id="c06d3-103">内容</span><span class="sxs-lookup"><span data-stu-id="c06d3-103">Contains</span></span>

<span data-ttu-id="c06d3-104">**含まれる**要素は、指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 <span data-ttu-id="c06d3-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="c06d3-105">**ContainsExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c06d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c06d3-106">Attributes and elements</span></span>

<span data-ttu-id="c06d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c06d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="c06d3-108">Attributes</span></span>

|<span data-ttu-id="c06d3-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c06d3-109">**Attribute**</span></span>|<span data-ttu-id="c06d3-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c06d3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c06d3-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="c06d3-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="c06d3-112">検索の範囲を識別します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="c06d3-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="c06d3-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="c06d3-114">検索には、ケースとのスペースが無視されるかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="c06d3-115">ContainmentMode 属性の値</span><span class="sxs-lookup"><span data-stu-id="c06d3-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="c06d3-116">**値**</span><span class="sxs-lookup"><span data-stu-id="c06d3-116">**Value**</span></span>|<span data-ttu-id="c06d3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c06d3-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c06d3-118">プリフィックス</span><span class="sxs-lookup"><span data-stu-id="c06d3-118">FullString</span></span>  <br/> |<span data-ttu-id="c06d3-119">比較では、完全な文字列と定数との間です。</span><span class="sxs-lookup"><span data-stu-id="c06d3-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="c06d3-120">プロパティの値と指定された定数は正確に同じです。</span><span class="sxs-lookup"><span data-stu-id="c06d3-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="c06d3-121">プレフィックス</span><span class="sxs-lookup"><span data-stu-id="c06d3-121">Prefixed</span></span>  <br/> |<span data-ttu-id="c06d3-122">比較は文字列のプレフィックスと定数との間です。</span><span class="sxs-lookup"><span data-stu-id="c06d3-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="c06d3-123">部分文字列</span><span class="sxs-lookup"><span data-stu-id="c06d3-123">Substring</span></span>  <br/> |<span data-ttu-id="c06d3-124">比較は、文字列の部分文字列と定数との間です。</span><span class="sxs-lookup"><span data-stu-id="c06d3-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="c06d3-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="c06d3-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="c06d3-126">比較は文字列内の各単語のプレフィックスと定数との間です。</span><span class="sxs-lookup"><span data-stu-id="c06d3-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="c06d3-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="c06d3-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="c06d3-128">比較は、文字列の完全一致のフレーズと定数との間です。</span><span class="sxs-lookup"><span data-stu-id="c06d3-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="c06d3-129">ContainmentComparison 属性の値</span><span class="sxs-lookup"><span data-stu-id="c06d3-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="c06d3-130">**値**</span><span class="sxs-lookup"><span data-stu-id="c06d3-130">**Value**</span></span>|<span data-ttu-id="c06d3-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="c06d3-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c06d3-132">Exact</span><span class="sxs-lookup"><span data-stu-id="c06d3-132">Exact</span></span>  <br/> |<span data-ttu-id="c06d3-133">比較は正確である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c06d3-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="c06d3-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="c06d3-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="c06d3-135">比較は、大文字と小文字を無視します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="c06d3-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="c06d3-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="c06d3-137">比較では、空白でない文字を無視します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="c06d3-138">広く</span><span class="sxs-lookup"><span data-stu-id="c06d3-138">Loose</span></span>  <br/> |<span data-ttu-id="c06d3-139">削除します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="c06d3-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="c06d3-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="c06d3-141">比較は、大文字と非空白文字を無視します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="c06d3-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="c06d3-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="c06d3-143">削除します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="c06d3-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="c06d3-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="c06d3-145">削除します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="c06d3-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="c06d3-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="c06d3-147">削除します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c06d3-148">子要素</span><span class="sxs-lookup"><span data-stu-id="c06d3-148">Child elements</span></span>

|<span data-ttu-id="c06d3-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="c06d3-149">**Element**</span></span>|<span data-ttu-id="c06d3-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="c06d3-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c06d3-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c06d3-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c06d3-152">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c06d3-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c06d3-154">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c06d3-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c06d3-156">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-157">定数</span><span class="sxs-lookup"><span data-stu-id="c06d3-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="c06d3-158">制限における定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c06d3-159">親要素</span><span class="sxs-lookup"><span data-stu-id="c06d3-159">Parent elements</span></span>

|<span data-ttu-id="c06d3-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="c06d3-160">**Element**</span></span>|<span data-ttu-id="c06d3-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="c06d3-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c06d3-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="c06d3-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c06d3-163">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-164">Not</span><span class="sxs-lookup"><span data-stu-id="c06d3-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="c06d3-165">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-166">And</span><span class="sxs-lookup"><span data-stu-id="c06d3-166">And</span></span>](and.md) <br/> |<span data-ttu-id="c06d3-167">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="c06d3-168">**すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="c06d3-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="c06d3-169">Or</span><span class="sxs-lookup"><span data-stu-id="c06d3-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="c06d3-170">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="c06d3-171">その子のいずれかの**場合は true**を返す場合、要素[または](or.md)要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c06d3-172">備考</span><span class="sxs-lookup"><span data-stu-id="c06d3-172">Remarks</span></span>

<span data-ttu-id="c06d3-173">属性を使用すると、要素を照合する方法を決定します。</span><span class="sxs-lookup"><span data-stu-id="c06d3-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="c06d3-174">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c06d3-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c06d3-175">要素情報</span><span class="sxs-lookup"><span data-stu-id="c06d3-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c06d3-176">名前空間</span><span class="sxs-lookup"><span data-stu-id="c06d3-176">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c06d3-177">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c06d3-177">Schema Name</span></span>  <br/> |<span data-ttu-id="c06d3-178">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c06d3-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="c06d3-179">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c06d3-179">Validation File</span></span>  <br/> |<span data-ttu-id="c06d3-180">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c06d3-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c06d3-181">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c06d3-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="c06d3-182">False</span><span class="sxs-lookup"><span data-stu-id="c06d3-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c06d3-183">関連項目</span><span class="sxs-lookup"><span data-stu-id="c06d3-183">See also</span></span>



- [<span data-ttu-id="c06d3-184">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c06d3-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

