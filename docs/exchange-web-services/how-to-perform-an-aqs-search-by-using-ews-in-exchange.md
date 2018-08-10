---
title: Exchange で EWS を使用して AQS 検索を実行する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: EWS マネージ API または EWS アプリケーションで、クエリ文字列および AQS を使用して検索する方法を確認します。
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759055"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="eb65c-103">Exchange で EWS を使用して AQS 検索を実行する</span><span class="sxs-lookup"><span data-stu-id="eb65c-103">How to: Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="eb65c-104">EWS マネージ API または EWS アプリケーションで、クエリ文字列および AQS を使用して検索する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="eb65c-105">クエリ文字列は、検索条件を表現する[検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)に代わる方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="eb65c-106">クエリ文字列を使用する最大の利点は、検索するプロパティを 1 つも指定する必要がないということです。</span><span class="sxs-lookup"><span data-stu-id="eb65c-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="eb65c-107">値を指定するだけで、アイテム上の一般的に使用されるすべてのフィールドに検索が適用されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="eb65c-108">単純な値の代わりに高度な検索テクニック (AQS) を使用して検索を絞り込むこともできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="eb65c-109">ただし、クエリ文字列には、ツールボックスに追加する前に注意すべき次の制限があります。</span><span class="sxs-lookup"><span data-stu-id="eb65c-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="eb65c-110">**特定のプロパティを検索する機能に制限がある。**</span><span class="sxs-lookup"><span data-stu-id="eb65c-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="eb65c-111">クエリ文字列で単純な値を検索すると、検索はすべてのインデックス付きプロパティに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="eb65c-112">特定のプロパティに検索を絞り込むことはできますが、AQS 文字列で使用できるプロパティは限定されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="eb65c-113">検索するプロパティが AQS で使用可能なプロパティのいずれでもない場合は、検索フィルターを使用することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="eb65c-114">**カスタム プロパティは検索されない。**</span><span class="sxs-lookup"><span data-stu-id="eb65c-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="eb65c-115">クエリ文字列の検索はインデックスに対して実行されますが、カスタム プロパティはそのインデックスに含まれません。</span><span class="sxs-lookup"><span data-stu-id="eb65c-115">Custom properties aren't searched. Query string searches are performed against an index, and custom properties are not included in that index. If you need to search custom properties, use a search filter instead.</span></span> <span data-ttu-id="eb65c-116">カスタム プロパティを検索する必要がある場合は、代わりに検索フィルターを使用してください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="eb65c-117">**文字列検索の制御が限定されている。**</span><span class="sxs-lookup"><span data-stu-id="eb65c-117">**Limited control for string searches.**</span></span> <span data-ttu-id="eb65c-118">クエリ文字列の検索は常に、大文字と小文字の違いを無視し、部分文字列の検索になります。</span><span class="sxs-lookup"><span data-stu-id="eb65c-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="eb65c-119">大文字と小文字を区別する場合、プレフィックスの検索、完全一致の検索を実行する場合は、検索フィルターを使用してください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-119">Limited control for string searches. Query string searches always ignore case, and are always substring searches. If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="eb65c-120">**フォルダーまたは検索フォルダーでは使用できない。**</span><span class="sxs-lookup"><span data-stu-id="eb65c-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="eb65c-121">フォルダーを検索するための EWS 操作では、クエリ文字列の使用がサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb65c-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="eb65c-122">さらに、検索フォルダーは、クエリ文字列をサポートしません。</span><span class="sxs-lookup"><span data-stu-id="eb65c-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="eb65c-123">どちらの場合も、検索フィルターが唯一のオプションになります。</span><span class="sxs-lookup"><span data-stu-id="eb65c-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="eb65c-124">クエリ文字列の作成</span><span class="sxs-lookup"><span data-stu-id="eb65c-124">Creating a query string</span></span>
<span data-ttu-id="eb65c-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="eb65c-125"></span></span>

<span data-ttu-id="eb65c-p106">EWS マネージ API および EWS のクエリ文字列は、AQS 構文の一部であると解釈されます。AQS 文字列は、値またはキーワード/値のペアのいずれかで構成され、コロン (:) で区切られます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-p106">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax. AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="eb65c-p107">キーワードを使用せずに値を指定した場合、すべてのインデックス付きプロパティでその値が検索されます。キーワードが値とペアになっている場合、キーワードは対応する値を検索するプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-p107">When a value is specified without a keyword, all indexed properties are searched for the value. If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="eb65c-130">**表 1. サポートされている AQS キーワード**</span><span class="sxs-lookup"><span data-stu-id="eb65c-130">**Table 1.  Supported AQS keywords**</span></span>

|<span data-ttu-id="eb65c-131">**キーワード**</span><span class="sxs-lookup"><span data-stu-id="eb65c-131">**Keyword**</span></span>|<span data-ttu-id="eb65c-132">**値の型**</span><span class="sxs-lookup"><span data-stu-id="eb65c-132">**Value type**</span></span>|<span data-ttu-id="eb65c-133">**例**</span><span class="sxs-lookup"><span data-stu-id="eb65c-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="eb65c-134">subject</span><span class="sxs-lookup"><span data-stu-id="eb65c-134">subject</span></span>  <br/> |<span data-ttu-id="eb65c-135">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-135">String</span></span>  <br/> |<span data-ttu-id="eb65c-136">subject:project</span><span class="sxs-lookup"><span data-stu-id="eb65c-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="eb65c-137">body</span><span class="sxs-lookup"><span data-stu-id="eb65c-137">body</span></span>  <br/> |<span data-ttu-id="eb65c-138">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-138">String</span></span>  <br/> |<span data-ttu-id="eb65c-139">body:sales figures</span><span class="sxs-lookup"><span data-stu-id="eb65c-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="eb65c-140">attachment</span><span class="sxs-lookup"><span data-stu-id="eb65c-140">attachment</span></span>  <br/> |<span data-ttu-id="eb65c-141">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-141">String</span></span>  <br/> |<span data-ttu-id="eb65c-142">attachment:report</span><span class="sxs-lookup"><span data-stu-id="eb65c-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="eb65c-143">to</span><span class="sxs-lookup"><span data-stu-id="eb65c-143">to</span></span>  <br/> |<span data-ttu-id="eb65c-144">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-144">String</span></span>  <br/> |<span data-ttu-id="eb65c-145">to:"Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="eb65c-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="eb65c-146">from</span><span class="sxs-lookup"><span data-stu-id="eb65c-146">from</span></span>  <br/> |<span data-ttu-id="eb65c-147">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-147">String</span></span>  <br/> |<span data-ttu-id="eb65c-148">from:hope</span><span class="sxs-lookup"><span data-stu-id="eb65c-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="eb65c-149">cc</span><span class="sxs-lookup"><span data-stu-id="eb65c-149">cc</span></span>  <br/> |<span data-ttu-id="eb65c-150">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-150">String</span></span>  <br/> |<span data-ttu-id="eb65c-151">cc:"Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="eb65c-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="eb65c-152">bcc</span><span class="sxs-lookup"><span data-stu-id="eb65c-152">bcc</span></span>  <br/> |<span data-ttu-id="eb65c-153">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-153">String</span></span>  <br/> |<span data-ttu-id="eb65c-154">bcc:mack</span><span class="sxs-lookup"><span data-stu-id="eb65c-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="eb65c-155">participants</span><span class="sxs-lookup"><span data-stu-id="eb65c-155">participants</span></span>  <br/> |<span data-ttu-id="eb65c-156">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-156">String</span></span>  <br/> |<span data-ttu-id="eb65c-157">participants:sadie</span><span class="sxs-lookup"><span data-stu-id="eb65c-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="eb65c-158">category</span><span class="sxs-lookup"><span data-stu-id="eb65c-158">category</span></span>  <br/> |<span data-ttu-id="eb65c-159">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-159">String</span></span>  <br/> |<span data-ttu-id="eb65c-160">category:project</span><span class="sxs-lookup"><span data-stu-id="eb65c-160">category:project</span></span>  <br/> |
|<span data-ttu-id="eb65c-161">importance</span><span class="sxs-lookup"><span data-stu-id="eb65c-161">importance</span></span>  <br/> |<span data-ttu-id="eb65c-162">文字列</span><span class="sxs-lookup"><span data-stu-id="eb65c-162">String</span></span>  <br/> |<span data-ttu-id="eb65c-163">importance:high</span><span class="sxs-lookup"><span data-stu-id="eb65c-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="eb65c-164">kind</span><span class="sxs-lookup"><span data-stu-id="eb65c-164">kind</span></span>  <br/> |<span data-ttu-id="eb65c-165">アイテムの種類</span><span class="sxs-lookup"><span data-stu-id="eb65c-165">Item type</span></span>  <br/> |<span data-ttu-id="eb65c-166">kind:meetings</span><span class="sxs-lookup"><span data-stu-id="eb65c-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="eb65c-167">sent</span><span class="sxs-lookup"><span data-stu-id="eb65c-167">sent</span></span>  <br/> |<span data-ttu-id="eb65c-168">日付</span><span class="sxs-lookup"><span data-stu-id="eb65c-168">Date</span></span>  <br/> |<span data-ttu-id="eb65c-169">sent:12/10/2013</span><span class="sxs-lookup"><span data-stu-id="eb65c-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="eb65c-170">received</span><span class="sxs-lookup"><span data-stu-id="eb65c-170">received</span></span>  <br/> |<span data-ttu-id="eb65c-171">日付</span><span class="sxs-lookup"><span data-stu-id="eb65c-171">Date</span></span>  <br/> |<span data-ttu-id="eb65c-172">received:yesterday</span><span class="sxs-lookup"><span data-stu-id="eb65c-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="eb65c-173">hasattachment</span><span class="sxs-lookup"><span data-stu-id="eb65c-173">hasattachment</span></span>  <br/> |<span data-ttu-id="eb65c-174">ブール型</span><span class="sxs-lookup"><span data-stu-id="eb65c-174">Boolean</span></span>  <br/> |<span data-ttu-id="eb65c-175">Has attachment:true</span><span class="sxs-lookup"><span data-stu-id="eb65c-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="eb65c-176">isflagged</span><span class="sxs-lookup"><span data-stu-id="eb65c-176">isflagged</span></span>  <br/> |<span data-ttu-id="eb65c-177">ブール型</span><span class="sxs-lookup"><span data-stu-id="eb65c-177">Boolean</span></span>  <br/> |<span data-ttu-id="eb65c-178">isflagged:true</span><span class="sxs-lookup"><span data-stu-id="eb65c-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="eb65c-179">isread</span><span class="sxs-lookup"><span data-stu-id="eb65c-179">isread</span></span>  <br/> |<span data-ttu-id="eb65c-180">ブール型</span><span class="sxs-lookup"><span data-stu-id="eb65c-180">Boolean</span></span>  <br/> |<span data-ttu-id="eb65c-181">isread:false</span><span class="sxs-lookup"><span data-stu-id="eb65c-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="eb65c-182">size</span><span class="sxs-lookup"><span data-stu-id="eb65c-182">size</span></span>  <br/> |<span data-ttu-id="eb65c-183">数値</span><span class="sxs-lookup"><span data-stu-id="eb65c-183">Number</span></span>  <br/> |<span data-ttu-id="eb65c-184">size:\>5000</span><span class="sxs-lookup"><span data-stu-id="eb65c-184">size:>5000</span></span>  <br/> |
   
<span data-ttu-id="eb65c-185">別の値の型がどのように動作するかを見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="eb65c-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="eb65c-186">文字列値型の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-186">Using a string value type</span></span>

<span data-ttu-id="eb65c-187">文字列値型は既定で、大文字と小文字を区別しないプレフィックス部分文字列として検索されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-187">String value types are by default searched as prefix substring searches that are not case-sensitive. That means that searching for subject:project would match any of the following subjects:</span></span> <span data-ttu-id="eb65c-188">つまり、subject:project を検索すると、次の項目のいずれかと一致します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-188">String value types are by default searched as prefix substring searches that are not case-sensitive. That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="eb65c-189">Project meeting notes</span><span class="sxs-lookup"><span data-stu-id="eb65c-189">Project meeting notes</span></span>
    
- <span data-ttu-id="eb65c-190">Do you have the project plans?</span><span class="sxs-lookup"><span data-stu-id="eb65c-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="eb65c-191">December sales projections</span><span class="sxs-lookup"><span data-stu-id="eb65c-191">December sales projections</span></span>
    
<span data-ttu-id="eb65c-192">文字列を引用符で囲むことによってプレフィックスと一致させるのではなく、完全に一致する単語を要求するように検索を変更できます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks. Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches. Note that the value is still not case-sensitive.</span></span> <span data-ttu-id="eb65c-193">subject:"project" を検索すると、候補一覧から「December sales projections」値が削除されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="eb65c-194">この場合でも、値は大文字と小文字が区別されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="eb65c-195">クエリ文字列に複数の単語を使用する場合、両方の単語が検索対象フィールドにあるものが一致します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields. For example, searching for subject:project plan would match any of the following subjects:</span></span> <span data-ttu-id="eb65c-196">たとえば、subject:project plan を検索すると、次の項目のいずれかと一致します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="eb65c-197">Project plan</span><span class="sxs-lookup"><span data-stu-id="eb65c-197">Project plan</span></span>
    
- <span data-ttu-id="eb65c-198">Do you have the project plans?</span><span class="sxs-lookup"><span data-stu-id="eb65c-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="eb65c-199">Please send me the plan for our project</span><span class="sxs-lookup"><span data-stu-id="eb65c-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="eb65c-200">Planning project milestones</span><span class="sxs-lookup"><span data-stu-id="eb65c-200">Planning project milestones</span></span>
    
<span data-ttu-id="eb65c-201">複数の単語を引用符で囲むと、それらは 1 つの句として扱われます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-201">If you enclose multiple words in quotation marks, they are treated as a single phrase. Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> <span data-ttu-id="eb65c-202">subject:"project plan" を検索すると、先ほどのリストの「Project plan」という件名だけが一致します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-202">If you enclose multiple words in quotation marks, they are treated as a single phrase. Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="eb65c-203">アイテムの種類の値の型の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-203">Using an item type value type</span></span>

<span data-ttu-id="eb65c-204">**kind** キーワードで次のアイテムの種類の値を使用して、検索結果をメールや会議出席依頼などの特定の種類のアイテムのみに制限することができます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="eb65c-205">連絡先</span><span class="sxs-lookup"><span data-stu-id="eb65c-205">contacts</span></span>    
- <span data-ttu-id="eb65c-206">docs</span><span class="sxs-lookup"><span data-stu-id="eb65c-206">docs</span></span>    
- <span data-ttu-id="eb65c-207">email</span><span class="sxs-lookup"><span data-stu-id="eb65c-207">email</span></span>    
- <span data-ttu-id="eb65c-208">faxes</span><span class="sxs-lookup"><span data-stu-id="eb65c-208">faxes</span></span>    
- <span data-ttu-id="eb65c-209">im (インスタント メッセージに相当)</span><span class="sxs-lookup"><span data-stu-id="eb65c-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="eb65c-210">journals</span><span class="sxs-lookup"><span data-stu-id="eb65c-210">journals</span></span>    
- <span data-ttu-id="eb65c-211">meetings (予定や会議出席依頼に相当)</span><span class="sxs-lookup"><span data-stu-id="eb65c-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="eb65c-212">notes</span><span class="sxs-lookup"><span data-stu-id="eb65c-212">notes</span></span>    
- <span data-ttu-id="eb65c-213">posts</span><span class="sxs-lookup"><span data-stu-id="eb65c-213">posts</span></span>    
- <span data-ttu-id="eb65c-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="eb65c-214">rssfeeds</span></span>    
- <span data-ttu-id="eb65c-215">tasks</span><span class="sxs-lookup"><span data-stu-id="eb65c-215">tasks</span></span>    
- <span data-ttu-id="eb65c-216">voicemail</span><span class="sxs-lookup"><span data-stu-id="eb65c-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="eb65c-217">日付値型の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-217">Using a date value type</span></span>

<span data-ttu-id="eb65c-218">日付値型はいくつかの異なる方法で検索できます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="eb65c-219">最も単純なのは特定の日付を検索することです。</span><span class="sxs-lookup"><span data-stu-id="eb65c-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="eb65c-220">received:12/11/2013 で検索すると、2013 年 12 月 11 日に受信したすべてのアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="eb65c-221">ただし、指定の仕方を簡単な形式にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-221">However, you can also be less specific.</span></span> <span data-ttu-id="eb65c-222">received:12/11 で検索すると、現在の年の 12 月 11 日に受信したすべてのアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="eb65c-223">別のオプションとして、月の名前を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-223">Another option is to use the month names.</span></span> <span data-ttu-id="eb65c-224">received:December 11, 2013 または December 11 で検索すると、received:12/11/2013 および received:12/11 と同じ結果を取得できます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-224">Another option is to use the month names. You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively. You can also search with received:December to get all items received in the month of December, in the current year.</span></span> <span data-ttu-id="eb65c-225">received:December で検索し、現在の年の 12 月に受信したすべてのアイテムを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="eb65c-226">週の曜日の名前を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-226">Using the names of the days of the week is also an option. Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> <span data-ttu-id="eb65c-227">received:Tuesday で検索すると、現在の週の火曜日に受信したすべてのアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-227">Using the names of the days of the week is also an option. Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="eb65c-p115">日付値型は、現在の時刻を基準にした検索のキーワードのセットもサポートします。サポートされているキーワードは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="eb65c-p115">Date value types also support a set of keywords for searches relative to the current time. The following keywords are supported:</span></span>
  
- <span data-ttu-id="eb65c-230">今日</span><span class="sxs-lookup"><span data-stu-id="eb65c-230">today</span></span>  
- <span data-ttu-id="eb65c-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="eb65c-231">tomorrow</span></span>
- <span data-ttu-id="eb65c-232">yesterday</span><span class="sxs-lookup"><span data-stu-id="eb65c-232">yesterday</span></span>
- <span data-ttu-id="eb65c-233">this week</span><span class="sxs-lookup"><span data-stu-id="eb65c-233">this week</span></span>    
- <span data-ttu-id="eb65c-234">last week</span><span class="sxs-lookup"><span data-stu-id="eb65c-234">last week</span></span>    
- <span data-ttu-id="eb65c-235">next month</span><span class="sxs-lookup"><span data-stu-id="eb65c-235">next month</span></span>    
- <span data-ttu-id="eb65c-236">past month</span><span class="sxs-lookup"><span data-stu-id="eb65c-236">past month</span></span>    
- <span data-ttu-id="eb65c-237">coming year</span><span class="sxs-lookup"><span data-stu-id="eb65c-237">coming year</span></span>
    
<span data-ttu-id="eb65c-238">日付値型は、greater than または less than のような関係演算子で比較したり、範囲演算子 **..** を使用して範囲として指定したりすることもできます。たとえば、received:\>11/30/2013, sent:\>=yesterday、received:12/1/2013..today はすべて、有効なクエリ文字列です。</span><span class="sxs-lookup"><span data-stu-id="eb65c-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator ... For example, received:>11/30/2013, sent:>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="eb65c-239">ブール値型の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-239">Using a Boolean value type</span></span>

<span data-ttu-id="eb65c-240">ブール値型は "true" または "false" にできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="eb65c-241">値は大文字と小文字を区別しないので、isread:false と isread:FALSE で生成される結果は同じです。</span><span class="sxs-lookup"><span data-stu-id="eb65c-241">Boolean value types can be "true" or "false". The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="eb65c-242">数値型の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-242">Using a number value type</span></span>

<span data-ttu-id="eb65c-243">数値型は、完全一致として検索できますが、greater than または less than のような関係演算子を使用して検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="eb65c-244">たとえば、size:10000 では、正確に 10000 バイトのサイズを持つアイテムのみが返されますが、size:\>=10000 では 10000 バイト以上のサイズを持つアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="eb65c-245">範囲演算子 (**..**) を使用して範囲を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="eb65c-246">たとえば、size:7000..8000 ではサイズが 7000 と 8000 の間のアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="eb65c-247">論理演算子の使用</span><span class="sxs-lookup"><span data-stu-id="eb65c-247">Using logical operators</span></span>

<span data-ttu-id="eb65c-248">クエリ文字列は、次の論理演算子をサポートします。</span><span class="sxs-lookup"><span data-stu-id="eb65c-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="eb65c-249">**表 2. サポートされる論理演算子**</span><span class="sxs-lookup"><span data-stu-id="eb65c-249">**Table 2.  Supported logical operators**</span></span>

|<span data-ttu-id="eb65c-250">**演算子**</span><span class="sxs-lookup"><span data-stu-id="eb65c-250">**Operator**</span></span>|<span data-ttu-id="eb65c-251">**例**</span><span class="sxs-lookup"><span data-stu-id="eb65c-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eb65c-252">AND</span><span class="sxs-lookup"><span data-stu-id="eb65c-252">AND</span></span>  <br/> |<span data-ttu-id="eb65c-253">project AND from:"Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="eb65c-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="eb65c-254">subject:(project AND plan)</span><span class="sxs-lookup"><span data-stu-id="eb65c-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="eb65c-255">OR</span><span class="sxs-lookup"><span data-stu-id="eb65c-255">OR</span></span>  <br/> |<span data-ttu-id="eb65c-256">subject:meeting OR from:"Hope Gross"</span><span class="sxs-lookup"><span data-stu-id="eb65c-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="eb65c-257">from:("Sadie Daniels" OR "Hope Gross")</span><span class="sxs-lookup"><span data-stu-id="eb65c-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="eb65c-258">NOT</span><span class="sxs-lookup"><span data-stu-id="eb65c-258">NOT</span></span>  <br/> |<span data-ttu-id="eb65c-259">NOT from:"Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="eb65c-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="eb65c-260">received:NOT today</span><span class="sxs-lookup"><span data-stu-id="eb65c-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="eb65c-261">これらの演算子を使用して、複数の条件を結合したり、1 つのキーワード/値のペア内で複数の値を結合したりできることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="eb65c-262">ただし、1 つのキーワード/値ペアで複数の値を結合する場合は、かっこを使用して複数の値を囲む必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb65c-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="eb65c-263">その理由を理解するために、from:"Sadie Daniels" OR "Hope Gross" で検索してみてください。</span><span class="sxs-lookup"><span data-stu-id="eb65c-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="eb65c-264">この検索は、実際には次の条件として解釈されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="eb65c-265">アイテムが Sadie Daniels からのもの、または</span><span class="sxs-lookup"><span data-stu-id="eb65c-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="eb65c-266">アイテムのインデックス付きプロパティのいずれかに「Hope Gross」という語句がある。</span><span class="sxs-lookup"><span data-stu-id="eb65c-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="eb65c-267">対照的に、from:("Sadie Daniels" OR "Hope Gross") は次のように解釈されます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="eb65c-268">アイテムが Sadie Daniels からのもの、または</span><span class="sxs-lookup"><span data-stu-id="eb65c-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="eb65c-269">アイテムが Hope Gross からのもの</span><span class="sxs-lookup"><span data-stu-id="eb65c-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="eb65c-270">複数の条件が指定されているものの論理演算子は含まれていない場合の既定の演算子は AND です。</span><span class="sxs-lookup"><span data-stu-id="eb65c-270">The default operator when multiple criteria are specified but no logical operator is included is AND. For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span> <span data-ttu-id="eb65c-271">たとえば、has attachment:true subject:project は has:attachment:true AND subject:project と同じです。</span><span class="sxs-lookup"><span data-stu-id="eb65c-271">The default operator when multiple criteria are specified but no logical operator is included is AND. For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="eb65c-272">例: クエリ文字列と EWS マネージ API を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="eb65c-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="eb65c-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="eb65c-273"></span></span>

<span data-ttu-id="eb65c-274">この例では、**SearchWithQueryString** というメソッドが定義されています。</span><span class="sxs-lookup"><span data-stu-id="eb65c-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="eb65c-275">パラメーターとして、[ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、[WellKnownFolderName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクト、クエリ文字列を表す **string** オブジェクトを取ります。</span><span class="sxs-lookup"><span data-stu-id="eb65c-275">It takes an [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="eb65c-276">この例では、**ExchangeService** オブジェクトは [Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="eb65c-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

<span data-ttu-id="eb65c-277">このメソッドを使用して、この例のように、件名に「project plan」という語句が含まれるすべてのアイテムを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="eb65c-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="eb65c-278">例: クエリ文字列と EWS を使用してアイテムを検索する</span><span class="sxs-lookup"><span data-stu-id="eb65c-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="eb65c-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="eb65c-279"></span></span>

<span data-ttu-id="eb65c-280">この例では、SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要求で、件名に「project plan」という語句が含まれる受信トレイ内のすべてのアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="eb65c-280">In this example, a SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="eb65c-281">次の例は、検索結果を含むサーバーからの応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="eb65c-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="eb65c-282">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb65c-282">See also</span></span>

- [<span data-ttu-id="eb65c-283">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="eb65c-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="eb65c-284">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="eb65c-284">How to: Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="eb65c-285">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="eb65c-285">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="eb65c-286">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="eb65c-286">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

