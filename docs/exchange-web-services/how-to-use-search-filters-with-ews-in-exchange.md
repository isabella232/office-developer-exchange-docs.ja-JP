---
title: EWS を使って Exchange 検索フィルターを使用します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: EWS Managed API または Exchange の EWS によって検索ファイルを使用する方法を確認します。
ms.openlocfilehash: 0652c36fd610c2f9dfe22b55323b368997137e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759081"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="fcb58-103">EWS を使って Exchange 検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="fcb58-104">EWS Managed API または Exchange の EWS によって検索ファイルを使用する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fcb58-105">検索フィルターは、EWS のマネージ API または EWS アプリケーションでの検索条件を記述するための主要なツールです。</span><span class="sxs-lookup"><span data-stu-id="fcb58-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="fcb58-106">次の[クエリ文字列](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)ではなく、検索フィルターを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="fcb58-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="fcb58-107">特定のプロパティまたはプロパティのセットを検索します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="fcb58-108">複数の検索条件を使用して検索します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="fcb58-109">検索フィルターは、次のいずれかを実行する場合、唯一のオプションです。</span><span class="sxs-lookup"><span data-stu-id="fcb58-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="fcb58-110">カスタム プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-110">Searching custom properties.</span></span>  
- <span data-ttu-id="fcb58-111">大文字小文字を区別して文字列の検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="fcb58-112">プレフィックスまたは完全に一致する文字列の検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="fcb58-113">ビットマスクの検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="fcb58-114">値に関係なく特定のプロパティ セットを持つアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="fcb58-115">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-115">Searching for folders.</span></span>
- <span data-ttu-id="fcb58-116">検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="fcb58-117">必要な検索フィルターの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="fcb58-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-118"></span></span>

<span data-ttu-id="fcb58-119">検索フィルターを作成する前にまず必要なフィルターの種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="fcb58-120">フィルターの種類は、EWS のマネージ API で[SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx)クラスの派生クラスおよび EWS での[制限](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx)要素の子要素として実装されています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-120">The filter types are implemented as descendant classes of the [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="fcb58-121">**表 1 です。検索フィルターの種類**</span><span class="sxs-lookup"><span data-stu-id="fcb58-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="fcb58-122">**フィルターの種類**</span><span class="sxs-lookup"><span data-stu-id="fcb58-122">**Filter type**</span></span>|<span data-ttu-id="fcb58-123">**EWS マネージ API クラス**</span><span class="sxs-lookup"><span data-stu-id="fcb58-123">**EWS Managed API class**</span></span>|<span data-ttu-id="fcb58-124">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="fcb58-124">**EWS element**</span></span>|<span data-ttu-id="fcb58-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="fcb58-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="fcb58-126">包含フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="fcb58-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="fcb58-127">ContainsSubstring</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-128">内容</span><span class="sxs-lookup"><span data-stu-id="fcb58-128">Contains</span></span>](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-p103">文字列比較に使用するのに最適なフィルターの種類です。大文字小文字の区別、空白を無視するかどうかを制御でき、包含モードを設定できます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-p103">The best filter type to use for string comparisons. It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="fcb58-131">ビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="fcb58-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="fcb58-132">ExcludesBitmask</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-133">除外</span><span class="sxs-lookup"><span data-stu-id="fcb58-133">Excludes</span></span>](http://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-134">整数のプロパティをビットマスクとして検索し、指定されたビットマスクに対応するビットが設定されていない結果のみを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="fcb58-135">存在フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="fcb58-136">存在します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-136">Exists</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-137">存在します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-137">Exists</span></span>](http://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-138">値に関係なく指定したプロパティを持つすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="fcb58-139">等値フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="fcb58-140">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-140">IsEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="fcb58-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-141">IsNotEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-142">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-142">IsEqualTo</span></span>](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="fcb58-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-143">IsNotEqualTo</span></span>](http://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-144">指定された定数値または別のプロパティの値のいずれかを指定したプロパティの値を比較し、同じ値の場合、 **IsEqualTo**フィルター) または (IsNotEqualTo、**の場合、非等値を持つすべてのアイテムを返す**フィルター) です。</span><span class="sxs-lookup"><span data-stu-id="fcb58-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="fcb58-145">関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="fcb58-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="fcb58-146">IsGreaterThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="fcb58-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-147">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="fcb58-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="fcb58-148">IsLessThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="fcb58-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-149">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="fcb58-150">IsGreaterThan</span></span>](http://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="fcb58-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-151">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="fcb58-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="fcb58-152">IsLessThan</span></span>](http://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="fcb58-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fcb58-153">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-154">指定された定数値または別のプロパティのいずれかに該当する関係で指定したプロパティの値を持つすべての項目を返します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="fcb58-155">など、 **IsGreaterThan**フィルターは、指定したプロパティで指定した値より大きい値を持っているすべての項目を返します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="fcb58-156">否定フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="fcb58-157">Not</span><span class="sxs-lookup"><span data-stu-id="fcb58-157">Not</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-158">Not</span><span class="sxs-lookup"><span data-stu-id="fcb58-158">Not</span></span>](http://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-159">他のフィルターの結果を否定します。 </span><span class="sxs-lookup"><span data-stu-id="fcb58-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="fcb58-160">複合フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="fcb58-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="fcb58-161">SearchFilterCollection</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fcb58-162">And</span><span class="sxs-lookup"><span data-stu-id="fcb58-162">And</span></span>](http://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="fcb58-163">Or</span><span class="sxs-lookup"><span data-stu-id="fcb58-163">Or</span></span>](http://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="fcb58-164">複数のフィルターを組み合わせて複雑な検索条件を指定できます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="fcb58-165">包含フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-165">Contains filter</span></span>

<span data-ttu-id="fcb58-p105">包含フィルターは、文字列のプロパティを検索するための最適な選択肢です。包含フィルターを使用すると、包含モードと比較モードを設定することによって、大文字小文字の区別や空白の処理方法など、文字列の一致のさまざまな面を制御することができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-p105">A contains filter is the best choice for searching string properties. With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-168">EWS Managed API での包含フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="fcb58-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-169"></span></span>

<span data-ttu-id="fcb58-170">EWS のマネージ API を使用している場合は、モードを設定する、包含構造、 [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx)クラスの[ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx)プロパティを使用していて、**の[ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx)プロパティを使用して比較モードを設定します。ContainsSubstring**クラス。</span><span class="sxs-lookup"><span data-stu-id="fcb58-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="fcb58-171">次の例では、「会議ノート」の部分文字列のアイテムの件名フィールドを検索する検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="fcb58-172">次の使用例は、大文字と小文字は無視されますが、空白は無視されません。</span><span class="sxs-lookup"><span data-stu-id="fcb58-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
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

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="fcb58-173">EWS での包含フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-173">Contains filter in EWS</span></span>
<span data-ttu-id="fcb58-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-174"></span></span>

<span data-ttu-id="fcb58-175">EWS でのモードを設定する、包含構造、[含まれる](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx)要素の**ContainmentMode**属性を使用して、**含まれる**要素の**ContainmentComparison**属性を使用して比較モードを設定します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="fcb58-176">次の例では、部分文字列「会議ノート」のアイテムの件名フィールドを検索する検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="fcb58-177">次の使用例は、大文字と小文字は無視されますが、空白は無視されません。</span><span class="sxs-lookup"><span data-stu-id="fcb58-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="fcb58-178">ビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-178">Bitmask filter</span></span>

<span data-ttu-id="fcb58-179">ビットマスク フィルターを使用すると、整数のプロパティをビットマスクとして検索し、指定されたプロパティの値に特定のビットが設定されていない結果を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-180">EWS Managed API でのビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-181">**ItemIndex**のカスタム プロパティの値を持つすべての項目を返す検索フィルターを作成するのには、EWS のマネージ API を使用する方法を示します、次の例 (で定義されている、[の使用例: 検索フィルターと、EWS のマネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)セクションこの資料では) の設定、2 番目のビット (2 進法では 10) を持っていません。</span><span class="sxs-lookup"><span data-stu-id="fcb58-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
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

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="fcb58-182">EWS でのビットマスク フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="fcb58-183">**ItemIndex**のカスタム プロパティの値を持つすべての項目を返す検索フィルターを作成するのには、EWS を使用する方法を示します、次の例 (で定義されている、[の使用例: 検索フィルターと、EWS のマネージ API を使用してアイテムを検索する](#bk_ExampleEWSMA)この資料の「)2 番目のビット (2 進法では 10) を設定するはありません。</span><span class="sxs-lookup"><span data-stu-id="fcb58-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="fcb58-184">存在フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-184">Exists filter</span></span>

<span data-ttu-id="fcb58-185">存在フィルターを使用すると、値に関係なく特定のプロパティが設定されているアイテムを検索できます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-186">EWS Managed API での存在フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-187">次の使用例は**ItemIndex**カスタム プロパティが設定されているすべての項目を返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="fcb58-188">EWS での存在フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-188">Exists filter in EWS</span></span>

<span data-ttu-id="fcb58-189">次の使用例は**ItemIndex**カスタム プロパティが設定されているすべての項目を返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="fcb58-190">等値フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-190">Equality filter</span></span>

<span data-ttu-id="fcb58-p108">等値フィルターでは、特定の値に等しいか、特定の値に等しくない、指定されたプロパティの値を持つすべてのアイテムを検索できます。比較する値は、定数値、またはアイテムごとの別のプロパティの値のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-p108">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value. The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-193">EWS Managed API での等値フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-194">次の例は、EWS Managed API を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="fcb58-195">次の例では、項目のサイズは**ItemIndex**プロパティの値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="fcb58-196">EWS での等値フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-196">Equality filter in EWS</span></span>

<span data-ttu-id="fcb58-197">次の例は、EWS を使用して、読み取られていないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="fcb58-198">次の例では、項目のサイズは**ItemIndex**プロパティの値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="fcb58-199">関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-199">Relational testing filter</span></span>

<span data-ttu-id="fcb58-200">リレーショナル テスト フィルターを有効にするには、指定したプロパティの値を持つすべての項目を検索することよりも大きい (\>) より大きいまたは等しい (\>=) より小さい (\<) と等しいかそれより小さい、または (\<=) 指定した値。</span><span class="sxs-lookup"><span data-stu-id="fcb58-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="fcb58-201">比較する値は、定数値または項目ごとに別のプロパティの値のいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-202">EWS Managed API での関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-203">次の例では、EWS のマネージ API を使用して、定数の値 3 を指定したリレーションシップの**ItemIndex**プロパティの値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
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

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="fcb58-204">EWS での関係テスト フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="fcb58-205">次の例では、EWS を使用して、定数値は 3 より大きい値は**ItemIndex**プロパティに値を持つすべての項目を返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="fcb58-206">次の例では、定数の値を 3 以上には**ItemIndex**プロパティに値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="fcb58-207">次の例では、定数値は 3 より小さいの**ItemIndex**プロパティの値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="fcb58-208">次の例では、定数値は 3 以下では**ItemIndex**プロパティの値を持つすべての項目を返す検索フィルターを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="fcb58-209">否定フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-209">Negating filter</span></span>

<span data-ttu-id="fcb58-p110">否定フィルターでは、別のフィルターを否定し、反対の検索結果を得ることができます。他のフィルターは特定の条件に一致する結果を返すのに対し、否定フィルターは、適用されるフィルターで指定した条件に一致しない結果を返します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-p110">A negating filter enables you to negate another filter and get the opposite search results. While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-212">EWS Managed API での否定フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-213">次の例は、EWS Managed API を使用して、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="fcb58-214">EWS での否定フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-214">Negating filter in EWS</span></span>

<span data-ttu-id="fcb58-215">次の例は、件名に部分文字列 "meeting notes" (会議メモ) を持たないすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="fcb58-216">複合フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-216">Compound filter</span></span>

<span data-ttu-id="fcb58-217">複合フィルターを使用するより複雑な検索条件を作成する複数のフィルターを組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="fcb58-218">論理演算子を使用して抽出条件を組み合わせることができ、または OR です。</span><span class="sxs-lookup"><span data-stu-id="fcb58-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="fcb58-219">これで、「件名に会議メモが含まれています Sadie Daniels からすべてのメール」のような検索を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="fcb58-220">EWS Managed API での複合フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="fcb58-221">次の例では、EWS Managed API を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="fcb58-222">EWS での複合フィルター</span><span class="sxs-lookup"><span data-stu-id="fcb58-222">Compound filter in EWS</span></span>

<span data-ttu-id="fcb58-223">次の例では、EWS を使用して、Sadie Daniels から送信され、件名に "meeting notes" (会議メモ) を含むすべてのアイテムを返す検索フィルターを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="fcb58-224">例:検索フィルターと EWS Managed API を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="fcb58-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="fcb58-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-225"></span></span>

<span data-ttu-id="fcb58-226">次の EWS Managed API メソッドは検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="fcb58-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="fcb58-227">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="fcb58-228">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="fcb58-228">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="fcb58-229">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="fcb58-229">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="fcb58-230">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="fcb58-230">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="fcb58-231">**ExchangeService.FindItems**メソッドを使用して、次の使用例ただし、同じ規則や概念は、すべてのメソッドに適用されます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="fcb58-232">この例では、 **SearchWithFilter**と呼ばれるメソッドを定義します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="fcb58-233">[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクト、 [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)オブジェクト、および[SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx)オブジェクトはパラメーターとして受け取ります。</span><span class="sxs-lookup"><span data-stu-id="fcb58-233">It takes an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="fcb58-234">次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="fcb58-235">**SearchFilter**クラスは、さまざまな検索フィルターをすべての基本クラスです。</span><span class="sxs-lookup"><span data-stu-id="fcb58-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
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

<span data-ttu-id="fcb58-p113">この記事の例で示すあらゆる検索フィルターに、この関数を使用できます。この例では、複合フィルターを使用して、件名に "meeting notes" (会議メモ) がある Sadie Daniels からの受信トレイのすべてのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-p113">You can use this function with any of the search filters shown in the examples in this article. This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="fcb58-238">例:検索フィルターと EWS を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="fcb58-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="fcb58-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-239"></span></span>

<span data-ttu-id="fcb58-240">次の EWS の操作は検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="fcb58-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="fcb58-241">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="fcb58-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="fcb58-242">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="fcb58-243">**FindItem**操作を使用して、次の使用例ただし、同じ規則や概念は、両方の操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="fcb58-244">検索フィルターは、SOAP 要求の[制限](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx)要素に含まれます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-244">Search filters are contained in the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="fcb58-245">この例では、EWS のマネージ API の例に示されている検索するのと同じである SOAP 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fcb58-246">次の例は、検索結果を含むサーバーからの応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fcb58-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="next-steps"></a><span data-ttu-id="fcb58-247">次の手順</span><span class="sxs-lookup"><span data-stu-id="fcb58-247">Next steps</span></span>
<span data-ttu-id="fcb58-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="fcb58-248"></span></span>

<span data-ttu-id="fcb58-249">これで、基本的な検索での検索フィルターの使用に慣れ、より高度な検索テクニックに進むことができます。</span><span class="sxs-lookup"><span data-stu-id="fcb58-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="fcb58-250">EWS を使用して Exchange によってグループ化された検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="fcb58-251">Exchange EWS を使用してページ検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="fcb58-252">関連項目</span><span class="sxs-lookup"><span data-stu-id="fcb58-252">See also</span></span>

- [<span data-ttu-id="fcb58-253">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="fcb58-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="fcb58-254">EWS を使用して Exchange、AQS 検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="fcb58-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="fcb58-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="fcb58-255">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="fcb58-256">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="fcb58-256">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="fcb58-257">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="fcb58-257">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="fcb58-258">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="fcb58-258">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- <span data-ttu-id="fcb58-259">
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fcb58-259">[FindFolder operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)</span></span>   
- <span data-ttu-id="fcb58-260">
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="fcb58-260">[FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)</span></span>
    

