---
title: Exchange で EWS とともに検索フィルターを使用する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: EWS マネージ API または Exchange の EWS によって検索ファイルを使用する方法を確認します。
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455836"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="81e26-103">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="81e26-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="81e26-104">EWS マネージ API または Exchange の EWS によって検索ファイルを使用する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="81e26-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="81e26-p101">検索フィルターは、EWS Managed API または EWS アプリケーションで検索条件を記述するための主要なツールです。[クエリ文字列](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)ではなく、検索フィルターを使用して以下を実行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="81e26-p101">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application. We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="81e26-107">特定のプロパティまたはプロパティのセットを検索します。</span><span class="sxs-lookup"><span data-stu-id="81e26-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="81e26-108">複数の検索条件を使用して検索します。</span><span class="sxs-lookup"><span data-stu-id="81e26-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="81e26-109">検索フィルターは、次のいずれかを実行する場合、唯一のオプションです。</span><span class="sxs-lookup"><span data-stu-id="81e26-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="81e26-110">カスタム プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="81e26-110">Searching custom properties.</span></span>  
- <span data-ttu-id="81e26-111">大文字小文字を区別して文字列の検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="81e26-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="81e26-112">プレフィックスまたは完全に一致する文字列の検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="81e26-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="81e26-113">ビットマスクの検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="81e26-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="81e26-114">値に関係なく特定のプロパティ セットを持つアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="81e26-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="81e26-115">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="81e26-115">Searching for folders.</span></span>
- <span data-ttu-id="81e26-116">検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="81e26-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="81e26-117">必要な検索フィルターの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="81e26-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="81e26-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-118"><a name="bk_SelectFilter"> </a></span></span>

<span data-ttu-id="81e26-119">検索フィルターを作成する前に、まず必要なフィルターの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="81e26-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="81e26-120">フィルターの種類は、EWS マネージ API では [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) クラスの子クラスとして、EWS では [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) 要素の子要素として実装されます。</span><span class="sxs-lookup"><span data-stu-id="81e26-120">The filter types are implemented as descendant classes of the [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="81e26-121">**表 1. 検索フィルターの種類**</span><span class="sxs-lookup"><span data-stu-id="81e26-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="81e26-122">**フィルターの種類**</span><span class="sxs-lookup"><span data-stu-id="81e26-122">**Filter type**</span></span>|<span data-ttu-id="81e26-123">**EWS マネージ API のクラス**</span><span class="sxs-lookup"><span data-stu-id="81e26-123">**EWS Managed API class**</span></span>|<span data-ttu-id="81e26-124">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="81e26-124">**EWS element**</span></span>|<span data-ttu-id="81e26-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="81e26-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="81e26-126">包含フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="81e26-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="81e26-127">ContainsSubstring</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-128">Contains</span><span class="sxs-lookup"><span data-stu-id="81e26-128">Contains</span></span>](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-p103">文字列比較に使用するのに最適なフィルターの種類です。大文字小文字の区別、空白を無視するかどうかを制御でき、包含モードを設定できます。</span><span class="sxs-lookup"><span data-stu-id="81e26-p103">The best filter type to use for string comparisons. It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="81e26-131">ビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="81e26-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="81e26-132">ExcludesBitmask</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-133">Excludes</span><span class="sxs-lookup"><span data-stu-id="81e26-133">Excludes</span></span>](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-134">整数のプロパティをビットマスクとして検索し、指定されたビットマスクに対応するビットが設定されていない結果のみを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="81e26-135">存在フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="81e26-136">Exists</span><span class="sxs-lookup"><span data-stu-id="81e26-136">Exists</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-137">Exists</span><span class="sxs-lookup"><span data-stu-id="81e26-137">Exists</span></span>](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-138">値に関係なく指定したプロパティを持つすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="81e26-139">等値フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="81e26-140">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-140">IsEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="81e26-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-141">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-142">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-142">IsEqualTo</span></span>](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="81e26-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-143">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-144">指定された定数値または別のプロパティの値のいずれかを持つ、指定されたプロパティの値を比較し、**IsEqualTo** フィルターの場合は同じ値を持つすべてのアイテムを返し、**IsNotEqualTo** フィルターの場合は非等値を返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="81e26-145">関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="81e26-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="81e26-146">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="81e26-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-147">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="81e26-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="81e26-148">IsLessThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="81e26-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-149">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="81e26-150">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="81e26-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-151">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="81e26-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="81e26-152">IsLessThan</span></span>](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="81e26-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="81e26-153">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-154">指定された定数値または別のプロパティのいずれかに該当する関係において、指定したプロパティの値を持つすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="81e26-155">たとえば、**IsGreaterThan** フィルターは指定されたプロパティの指定された値よりも大きい値を持つすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="81e26-156">否定フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="81e26-157">Not</span><span class="sxs-lookup"><span data-stu-id="81e26-157">Not</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-158">Not</span><span class="sxs-lookup"><span data-stu-id="81e26-158">Not</span></span>](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-159">他のフィルターの結果を否定します。</span><span class="sxs-lookup"><span data-stu-id="81e26-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="81e26-160">複合フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="81e26-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="81e26-161">SearchFilterCollection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="81e26-162">And</span><span class="sxs-lookup"><span data-stu-id="81e26-162">And</span></span>](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="81e26-163">Or</span><span class="sxs-lookup"><span data-stu-id="81e26-163">Or</span></span>](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="81e26-164">複数のフィルターを組み合わせて複雑な検索条件を指定できます。</span><span class="sxs-lookup"><span data-stu-id="81e26-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="81e26-165">包含フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-165">Contains filter</span></span>

<span data-ttu-id="81e26-p105">包含フィルターは、文字列のプロパティを検索するための最適な選択肢です。包含フィルターを使用すると、包含モードと比較モードを設定することによって、大文字小文字の区別や空白の処理方法など、文字列の一致のさまざまな面を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-p105">A contains filter is the best choice for searching string properties. With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-168">EWS マネージ API での包含フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="81e26-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-169"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="81e26-170">EWS マネージ API を使用している場合、[ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) クラスの [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) プロパティを使用して包含モードを設定し、**ContainsSubstring** クラスの [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) プロパティを使用して比較モードを設定します。</span><span class="sxs-lookup"><span data-stu-id="81e26-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="81e26-171">次の例では、"meeting notes" (会議メモ) という部分文字列を、アイテムの件名フィールドで検索する検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="81e26-172">この例では大文字と小文字は無視されますが、空白は無視されません。</span><span class="sxs-lookup"><span data-stu-id="81e26-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="81e26-173">EWS での包含フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-173">Contains filter in EWS</span></span>
<span data-ttu-id="81e26-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-174"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="81e26-175">EWS では、[Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) 要素の **ContainmentMode** 属性を使用して包含モードを設定し、**Contains** 要素の **ContainmentComparison** 属性を使用して比較モードを設定します。</span><span class="sxs-lookup"><span data-stu-id="81e26-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="81e26-176">次の例では、"meeting notes" (会議メモ) という部分文字列を、アイテムの件名フィールドで検索するための検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="81e26-177">この例では大文字と小文字は無視されますが、空白は無視されません。</span><span class="sxs-lookup"><span data-stu-id="81e26-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="81e26-178">ビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-178">Bitmask filter</span></span>

<span data-ttu-id="81e26-179">ビットマスク フィルターを使用すると、整数のプロパティをビットマスクとして検索し、指定されたプロパティの値に特定のビットが設定されていない結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-180">EWS マネージ API でのビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-181">次の例では、EWS マネージ API を使用して、(この記事の「[例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)」セクションで定義された) **ItemIndex** カスタム プロパティの値を持ち、2 番目のビット (バイナリの 10) が設定されていないすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="81e26-182">EWS でのビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="81e26-183">次の例では、EWS を使用して、(この記事の「[例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)」セクションで定義された) **ItemIndex** カスタム プロパティの値を持ち、2 番目のビット (バイナリの 10) が設定されていないすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="81e26-184">存在フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-184">Exists filter</span></span>

<span data-ttu-id="81e26-185">存在フィルターを使用すると、値に関係なく特定のプロパティが設定されているアイテムを検索できます。</span><span class="sxs-lookup"><span data-stu-id="81e26-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-186">EWS マネージ API での存在フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-187">次の例は、**ItemIndex** カスタム プロパティが設定されているすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="81e26-188">EWS での存在フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-188">Exists filter in EWS</span></span>

<span data-ttu-id="81e26-189">次の例は、**ItemIndex** カスタム プロパティが設定されているすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="81e26-190">等値フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-190">Equality filter</span></span>

<span data-ttu-id="81e26-p108">等値フィルターでは、特定の値に等しいか、特定の値に等しくない、指定されたプロパティの値を持つすべてのアイテムを検索できます。比較する値は、定数値、またはアイテムごとの別のプロパティの値のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="81e26-p108">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value. The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-193">EWS Managed API での等値フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-194">次の例は、EWS Managed API を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="81e26-195">次の例は、アイテムのサイズに等しくない **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="81e26-196">EWS での等値フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-196">Equality filter in EWS</span></span>

<span data-ttu-id="81e26-197">次の例は、EWS を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="81e26-198">次の例は、アイテムのサイズに等しくない **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="81e26-199">関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-199">Relational testing filter</span></span>

<span data-ttu-id="81e26-200">関係テスト フィルターでは、指定された値より大きい (\>)、指定された値以上である (\>=)、指定された値より小さい (\<)、または指定された値以下である (\<=) 指定したプロパティの値を持つすべてのアイテムを検索できます。</span><span class="sxs-lookup"><span data-stu-id="81e26-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="81e26-201">比較する値は、定数値、またはアイテムごとの別のプロパティの値のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="81e26-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-202">EWS マネージ API での関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-203">次の例では、EWS Managed API を使用して、定数値 3 に対して指定された関係である **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="81e26-204">EWS での関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="81e26-205">次の例では、EWS を使用して、定数値 3 よりも大きい **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="81e26-206">次の例では、定数値 3 以上の **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="81e26-207">次の例では、定数値 3 よりも小さい **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="81e26-208">次の例では、定数値 3 以下の **ItemIndex** プロパティの値を持つすべてのアイテムを返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="81e26-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="81e26-209">否定フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-209">Negating filter</span></span>

<span data-ttu-id="81e26-p110">否定フィルターでは、別のフィルターを否定し、反対の検索結果を得ることができます。他のフィルターは特定の条件に一致する結果を返すのに対し、否定フィルターは、適用されるフィルターで指定した条件に一致しない結果を返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-p110">A negating filter enables you to negate another filter and get the opposite search results. While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-212">EWS Managed API での否定フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-213">次の例は、EWS Managed API を使用して、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="81e26-214">EWS での否定フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-214">Negating filter in EWS</span></span>

<span data-ttu-id="81e26-215">次の例は、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="81e26-216">複合フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-216">Compound filter</span></span>

<span data-ttu-id="81e26-217">複合フィルターでは、複数のフィルターを組み合わせてより複雑な検索条件を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="81e26-218">論理演算子 AND または OR を使用して、条件を組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="81e26-219">この方法で、「件名に ’meeting notes’ (会議メモ) が含まれている Sadie Daniels からすべてのメール」のような検索を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="81e26-220">EWS マネージ API での複合フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="81e26-221">次の例では、EWS Managed API を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="81e26-222">EWS での複合フィルター</span><span class="sxs-lookup"><span data-stu-id="81e26-222">Compound filter in EWS</span></span>

<span data-ttu-id="81e26-223">次の例では、EWS を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="81e26-224">例: 検索フィルターと EWS マネージ API を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="81e26-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="81e26-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-225"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="81e26-226">次の EWS マネージ API メソッドは検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="81e26-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="81e26-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="81e26-227">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="81e26-228">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="81e26-228">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="81e26-229">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="81e26-229">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="81e26-230">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="81e26-230">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="81e26-231">次の例では **ExchangeService.FindItems** メソッドを使用しますが、同じルールと概念がすべてのメソッドに適用されます。</span><span class="sxs-lookup"><span data-stu-id="81e26-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="81e26-232">この例では、**SearchWithFilter** というメソッドが定義されています。</span><span class="sxs-lookup"><span data-stu-id="81e26-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="81e26-233">パラメーターとして、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、[WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクト、および [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) オブジェクトを取ります。</span><span class="sxs-lookup"><span data-stu-id="81e26-233">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="81e26-234">この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="81e26-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="81e26-235">**SearchFilter** クラスは、さまざまな検索フィルターすべての基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="81e26-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="81e26-p113">この記事の例で示すあらゆる検索フィルターに、この関数を使用できます。この例では、複合フィルターを使用して、件名に "meeting notes" (会議メモ) がある Sadie Daniels からの受信トレイのすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="81e26-p113">You can use this function with any of the search filters shown in the examples in this article. This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="81e26-238">例: 検索フィルターと EWS を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="81e26-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="81e26-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-239"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="81e26-240">次の EWS の操作は検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="81e26-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="81e26-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="81e26-241">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="81e26-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="81e26-242">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="81e26-243">次の例では **FindItem** 操作を使用しますが、両方の操作で同じルールと概念が適用されます。</span><span class="sxs-lookup"><span data-stu-id="81e26-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="81e26-244">検索フィルターは、SOAP 要求の [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) 要素に含まれます。</span><span class="sxs-lookup"><span data-stu-id="81e26-244">Search filters are contained in the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="81e26-245">この例では、前述の EWS マネージ API の例で示している検索に相当する SOAP 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="81e26-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="81e26-246">次の例は、検索結果を含むサーバーからの応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="81e26-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="81e26-247">次の手順</span><span class="sxs-lookup"><span data-stu-id="81e26-247">Next steps</span></span>
<span data-ttu-id="81e26-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="81e26-248"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="81e26-249">これで、基本的な検索での検索フィルターの使用に慣れ、より高度な検索テクニックに進むことができます。</span><span class="sxs-lookup"><span data-stu-id="81e26-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="81e26-250">Exchange で EWS を使用して、グループ化された検索を実行する</span><span class="sxs-lookup"><span data-stu-id="81e26-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="81e26-251">Exchange で EWS を使用してページング検索を実行する</span><span class="sxs-lookup"><span data-stu-id="81e26-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="81e26-252">関連項目</span><span class="sxs-lookup"><span data-stu-id="81e26-252">See also</span></span>

- [<span data-ttu-id="81e26-253">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="81e26-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="81e26-254">Exchange で EWS を使用して AQS 検索を実行する</span><span class="sxs-lookup"><span data-stu-id="81e26-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="81e26-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="81e26-255">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="81e26-256">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="81e26-256">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="81e26-257">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="81e26-257">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="81e26-258">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="81e26-258">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="81e26-259">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="81e26-259">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="81e26-260">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="81e26-260">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

