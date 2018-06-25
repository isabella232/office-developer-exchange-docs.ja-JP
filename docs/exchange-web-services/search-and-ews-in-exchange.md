---
title: Exchange の検索と EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: EWS マネージ API または EWS を使用して、Exchange でアイテムを検索する方法を確認します。
ms.openlocfilehash: da24258ba94b842fa97fff92148620344c939f05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759188"
---
# <a name="search-and-ews-in-exchange"></a><span data-ttu-id="369a8-103">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="369a8-103">Search and EWS in Exchange</span></span>

<span data-ttu-id="369a8-104">EWS マネージ API または EWS を使用して、Exchange でアイテムを検索する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="369a8-104">Find out how to search for items in Exchange by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="369a8-p101">次のような流れを経験したことはないでしょうか。数週間先延ばしにしていたあるプロジェクトをやっと開始しようとしたときに、上司から数週間前にメールで受け取った、プロジェクトに関する情報が必要になりました。受信トレイには数百またはおそらく数千ものメッセージがあります。どうしますか。その情報が見つかるまで、メールをスクロールして各件名と送信者のスキャンしますか。または、好みのメール クライアント検索機能を使用して、必要な情報に的を絞りますか。</span><span class="sxs-lookup"><span data-stu-id="369a8-p101">Does this sound familiar? You're finally starting that project you've been putting off for weeks, and you need information about the project that your manager sent you in email weeks ago. Your Inbox has hundreds or perhaps thousands of messages in it. What do you do? Do you scroll through your email scanning each subject and sender until you find it? Or do you use the search feature in your favorite email client to quickly zero in on what you need?</span></span>
  
<span data-ttu-id="369a8-p102">検索は、ほぼ間違いなくすべてのメール クライアントに備わっている機能です。しかし、検索はユーザーがただ自分のメールボックスを検索できるようにするためのものではありません。特定の期間に含まれる予定をアプリで処理する必要がありますか。特定のステータスのすべてのタスク アイテムについてレポートしたり、特定の会社名を含むすべての連絡先を別のフォルダーに移動したりする必要があるかもしれません。検索によって、これらのすべての要件を満たすことができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p102">Search is arguably a must-have feature for any email client. But search can be used for a lot more than just enabling users to search their mailbox. Does your app need to process appointments that fall within specific time windows? Maybe you need to report on all task items with a specific status, or move all contacts with a specific company name to a different folder. Search can help with all of these requirements.</span></span>
  
## <a name="search-basics"></a><span data-ttu-id="369a8-116">検索の基本</span><span class="sxs-lookup"><span data-stu-id="369a8-116">Search basics</span></span>
<span data-ttu-id="369a8-117"><a name="bk_SearchBasics"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-117"></span></span>

<span data-ttu-id="369a8-118">EWS のマネージ API と EWS は、検索を指定するための 2 つの基本的な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="369a8-118">The EWS Managed API and EWS offer two basic methods for specifying a search.</span></span> <span data-ttu-id="369a8-119">[検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)または[クエリ文字列](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-119">You can use a [search filter](how-to-use-search-filters-with-ews-in-exchange.md) or a [query string](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="369a8-120">使用する方法は、検索の背後にある意図によって異なります。</span><span class="sxs-lookup"><span data-stu-id="369a8-120">The method you use depends on the intent behind your search.</span></span>
  
<span data-ttu-id="369a8-121">**表 1 です。検索フィルターと検索クエリのシナリオ**</span><span class="sxs-lookup"><span data-stu-id="369a8-121">**Table 1. Scenarios for search filters and search queries**</span></span>

|<span data-ttu-id="369a8-122">**目的…**</span><span class="sxs-lookup"><span data-stu-id="369a8-122">**If you want to…**</span></span>|<span data-ttu-id="369a8-123">**使用する.**</span><span class="sxs-lookup"><span data-stu-id="369a8-123">**Use a…**</span></span>|<span data-ttu-id="369a8-124">**メモ**</span><span class="sxs-lookup"><span data-stu-id="369a8-124">**Notes**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="369a8-125">検索を特定のプロパティまたはプロパティのセットに限定する</span><span class="sxs-lookup"><span data-stu-id="369a8-125">Limit your search to a specific property or set of properties</span></span>  <br/> |<span data-ttu-id="369a8-126">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-126">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-p104">検索フィルターは、プロパティの検索を最も良く制御できます。クエリ文字列では、高度な検索テクニック (AQS) を使用して限定されたプロパティのセットをターゲットにすることができます。検索フィルターでは任意のプロパティをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p104">Search filters provide the best level of control over which properties are searched. Although query strings can target a limited set of properties by using Advanced Query Syntax (AQS), search filters can target any property.</span></span>  <br/> |
|<span data-ttu-id="369a8-129">複数の条件で検索を作成する</span><span class="sxs-lookup"><span data-stu-id="369a8-129">Create searches with multiple criteria</span></span>  <br/> |<span data-ttu-id="369a8-130">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-130">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-p105">検索フィルターでは、論理 AND または OR を使用して複数の検索条件を結合でき、「件名に '会議ノート' が含まれる、および送信者が 'Sadie Daniels' に等しい」のような検索が可能になります。クエリ文字列では複数の検索条件を結合することもできますが、検索はクエリ文字列でサポートされているプロパティのセットに限定されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p105">With search filters, multiple search criteria can be joined together with logical ANDs or ORs, allowing for searches like "subject contains 'Meeting Notes' AND sender equals 'Sadie Daniels'". Although query strings can also join multiple search criteria, they are limited to the set of properties supported by query strings.</span></span>  <br/> |
|<span data-ttu-id="369a8-133">カスタム プロパティの検索</span><span class="sxs-lookup"><span data-stu-id="369a8-133">Search custom properties</span></span>  <br/> |<span data-ttu-id="369a8-134">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-134">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-p106">検索フィルターは、カスタム プロパティをターゲットにすることができます。クエリ文字列は、カスタム プロパティを検索しません。</span><span class="sxs-lookup"><span data-stu-id="369a8-p106">Search filters can target custom properties. Query strings do not search custom properties.</span></span>  <br/> |
|<span data-ttu-id="369a8-137">文字列プロパティの大文字と小文字を区別する検索を実行する</span><span class="sxs-lookup"><span data-stu-id="369a8-137">Perform a case sensitive search of string properties</span></span>  <br/> |<span data-ttu-id="369a8-138">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-138">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-139">クエリ文字列では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="369a8-139">Query string searches are not case sensitive.</span></span>  <br/> |
|<span data-ttu-id="369a8-140">文字列プロパティを検索するときに含有モードを制御する</span><span class="sxs-lookup"><span data-stu-id="369a8-140">Control the containment mode when searching string properties</span></span>  <br/> |<span data-ttu-id="369a8-141">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-141">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-p107">クエリ文字列の検索は常に、部分文字列の検索になります。特定のプレフィックスを検索する場合や、完全一致が必要な場合は、検索フィルターを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="369a8-p107">Query string searches are always substring searches. If you need to search for specific prefixes, or require exact matches, a search filter is the best choice.</span></span>  <br/> |
|<span data-ttu-id="369a8-144">フォルダーを検索する</span><span class="sxs-lookup"><span data-stu-id="369a8-144">Search for folders</span></span>  <br/> |<span data-ttu-id="369a8-145">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-145">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-146">EWS では、クエリ文字列によるフォルダーの検索はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369a8-146">EWS does not support searching for folders with a query string.</span></span>  <br/> |
|<span data-ttu-id="369a8-147">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="369a8-147">Create a search folder</span></span>  <br/> |<span data-ttu-id="369a8-148">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="369a8-148">Search filter</span></span>  <br/> |<span data-ttu-id="369a8-149">EWS では、クエリ文字列による検索フォルダーの作成はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="369a8-149">EWS does not support creating search folders with a query string.</span></span>  <br/> |
|<span data-ttu-id="369a8-150">一般的に使用されるすべてのプロパティを検索する</span><span class="sxs-lookup"><span data-stu-id="369a8-150">Search across all commonly used properties</span></span>  <br/> |<span data-ttu-id="369a8-151">クエリ文字列</span><span class="sxs-lookup"><span data-stu-id="369a8-151">Query string</span></span>  <br/> |<span data-ttu-id="369a8-p108">AQS が含まれていないクエリ文字列は、一般的に使用されるすべてのプロパティを検索します。たとえば、クエリ文字列値が「Mack Chaves」である場合、Mack Chaves によって送信されたすべてのメッセージ、および本文または件名に「Mack Chaves」が含まれるすべてのメッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p108">Query strings that do not contain AQS will search across all commonly used properties. For example, a query string value of "Mack Chaves" will return all messages sent by Mack Chaves as well as any messages that have "Mack Chaves" in the body or subject.</span></span>  <br/> |
|<span data-ttu-id="369a8-154">単純なユーザー入力に基づいた検索を作成する</span><span class="sxs-lookup"><span data-stu-id="369a8-154">Construct a search based on simple user input</span></span>  <br/> |<span data-ttu-id="369a8-155">クエリ文字列</span><span class="sxs-lookup"><span data-stu-id="369a8-155">Query string</span></span>  <br/> |<span data-ttu-id="369a8-p109">クエリ文字列は、エンド ユーザーが単純な文字列を入力してクイック検索を実行するための最適な選択肢です。クエリ文字列の検索には、一般的に使用されるすべてのプロパティが含まれるため、ユーザーの検索語句を含むすべてのアイテムが結果に含まれます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p109">A query string is a great choice for allowing an end user to do a quick search by typing in a simple string. Because a query string search includes all commonly used properties, the results will contain any items that contain the user's search terms.</span></span>  <br/> |
   
### <a name="using-a-search-filter"></a><span data-ttu-id="369a8-158">検索フィルターの使用</span><span class="sxs-lookup"><span data-stu-id="369a8-158">Using a search filter</span></span>

<span data-ttu-id="369a8-p110">検索フィルターでは、さまざまな検索オプションを使用し、検索の実行方法を最高度に制御できます。検索フィルターを使用して、基本的な等値検索と比較検索を実行できますが、さらに、文字列プロパティの内容を検索したりビットマスクの比較を実行することも可能です。</span><span class="sxs-lookup"><span data-stu-id="369a8-p110">Search filters give you a wide range of search options and the greatest degree of control over how the search is performed. You can use search filters to perform basic equality and comparison searches, but you can also search within the contents of string properties or do bitmask comparisons.</span></span>
  
<span data-ttu-id="369a8-161">たとえば、EWS のマネージ API で[SearchFilter.ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx)クラスを使用して、アイテムの件名の内容を検索できます。</span><span class="sxs-lookup"><span data-stu-id="369a8-161">For example, you can search the contents of the subject of items by using the [SearchFilter.ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class in the EWS Managed API.</span></span> <span data-ttu-id="369a8-162">この例では、大文字と小文字を無視して、部分文字列「会議メモ」の件名を検索する検索フィルターが作成されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-162">In this example, a search filter is created to search the subject for the substring "meeting notes", ignoring case.</span></span> 
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

<span data-ttu-id="369a8-163">カスタム プロパティに対して検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="369a8-163">You can also search against custom properties.</span></span> <span data-ttu-id="369a8-164">この例では、3 より大きい値は**ItemIndex**のユーザー設定のプロパティが検索されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-164">In this example, the custom property **ItemIndex** is searched for values greater than 3.</span></span> 
  
```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer); 
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

<span data-ttu-id="369a8-165">複雑な検索を作成するのには複数の検索フィルターを組み合わせることもできます。</span><span class="sxs-lookup"><span data-stu-id="369a8-165">You can also combine multiple search filters to create more complex searches.</span></span> <span data-ttu-id="369a8-166">たとえば、 [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx)クラスを使用して論理 AND で前の 2 つのフィルターを組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-166">For example, you can combine the previous two filters with a logical AND by using the [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) class.</span></span> 
  
```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a><span data-ttu-id="369a8-167">クエリ文字列の使用</span><span class="sxs-lookup"><span data-stu-id="369a8-167">Using a query string</span></span>

<span data-ttu-id="369a8-168">クエリ文字列を検索する別の方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="369a8-168">Query strings provide a different approach to search.</span></span> <span data-ttu-id="369a8-169">検索されるフィールドとクエリ文字列の検索を使用する場合に、検索を実行する方法があります。</span><span class="sxs-lookup"><span data-stu-id="369a8-169">You have less control over the fields that are searched and how the search is performed when you use a query string search.</span></span> <span data-ttu-id="369a8-170">ありませんが悪いことである!</span><span class="sxs-lookup"><span data-stu-id="369a8-170">Not that that's a bad thing!</span></span> <span data-ttu-id="369a8-171">場合によっては、幅の広いネットワークでは、ためのいわばキャストすることがあります。</span><span class="sxs-lookup"><span data-stu-id="369a8-171">In some cases, you might want to cast a wider net, so to speak.</span></span>
  
<span data-ttu-id="369a8-172">たとえば、「会議ノート」の[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/jj223808%28v=exchg.80%29.aspx) EWS 管理 API メソッドを使用して検索できます。</span><span class="sxs-lookup"><span data-stu-id="369a8-172">For example, you can search for "meeting notes" by using the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/jj223808%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> 
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

<span data-ttu-id="369a8-173">**SearchFilter.ContainsSubstring**検索の例を前の結果には、この検索の結果を比較すると、この検索によりより多くの結果が含まれます。</span><span class="sxs-lookup"><span data-stu-id="369a8-173">If you compare the results of this search to the results of the **SearchFilter.ContainsSubstring** search example earlier, this search will contain more results.</span></span> <span data-ttu-id="369a8-174">検索フィルター検索はこの検索は、件名、本文、およびその他のフィールドに「会議ノート」の項目を返すときに、件名に「会議ノート」を持っているアイテムのみを返します。</span><span class="sxs-lookup"><span data-stu-id="369a8-174">The search filter search will return only items that have "meeting notes" in the subject, while this search will return items that have "meeting notes" in the subject, body, and other fields.</span></span> 
  
<span data-ttu-id="369a8-p116">クエリ文字列を調整して、検索フィルターの結果に近くなる、絞り込み方法を見てみましょう。AQS を使用すると、検索を件名に制限することができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p116">Let's take a look at how you can refine the query string to get closer to the results you see from the search filter. Using AQS, you can limit your search to the subject.</span></span>
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

<span data-ttu-id="369a8-p117">これでかなり近くなりますが、結果はまだ同じではありません。複数の文字が含まれるクエリ文字列を使用すると、それらの単語が指定した順序どおりでない場合や、それらの単語が隣接していない場合でも、一致となります。クエリ文字列「subject:meeting notes」を使用すると、「meeting notes」、「notes from the meeting」が一致となります。さらに絞り込むには、検索用語を二重引用符で囲み、その語句だけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p117">This is closer, but the results are still not quite the same. When you use a query string with multiple words, you will get matches even if the words are not in the order you specify, or even if they're not adjacent to each other. With the query string "subject:meeting notes", you will get matches for "meeting notes", "notes from the meeting", and so on. To further refine, you can wrap the search terms in double quotes to indicate that you want that phrase only.</span></span>
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a><span data-ttu-id="369a8-181">検索結果で特定のプロパティを要求する</span><span class="sxs-lookup"><span data-stu-id="369a8-181">Requesting specific properties in search results</span></span>
<span data-ttu-id="369a8-182"><a name="bk_RequestSpecific"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-182"></span></span>

<span data-ttu-id="369a8-183">既定では、検索結果に検索条件に一致する項目のすべてのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="369a8-183">By default, search results will contain all properties on the items that match the search.</span></span> <span data-ttu-id="369a8-184">いくつかの場合がありますたいが、ほとんどの場合アプリケーションだけで必要なプロパティの個別のセットです。</span><span class="sxs-lookup"><span data-stu-id="369a8-184">In some cases this might be what you want, but in most cases your application only requires a discrete set of properties.</span></span> <span data-ttu-id="369a8-185">この例では、アプリケーションのプロパティだけに返されるプロパティのセットを制限する必要があります必要があります。</span><span class="sxs-lookup"><span data-stu-id="369a8-185">In this case, you should limit the set of properties that are returned to only the properties your application needs.</span></span> <span data-ttu-id="369a8-186">、件名に返されるプロパティを制限するのには次の例では、 [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx)クラスが使用される日付と時刻を受信すると、およびアイテムの ID です。</span><span class="sxs-lookup"><span data-stu-id="369a8-186">In the following example, the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class is used to limit the returned properties to the subject, date/time received, and ID of the items.</span></span> 
  
```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes 
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a><span data-ttu-id="369a8-187">検索の深さの制御</span><span class="sxs-lookup"><span data-stu-id="369a8-187">Controlling search depth</span></span>
<span data-ttu-id="369a8-188"><a name="bk_SearchDepth"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-188"></span></span>

<span data-ttu-id="369a8-189">ビュー上で走査の設定をすることによって、検索の範囲と深さを制御します。 </span><span class="sxs-lookup"><span data-stu-id="369a8-189">Setting the traversal on the view controls the depth and scope of the search.</span></span> 
  
<span data-ttu-id="369a8-190">**表 2 になります。検査値の検索**</span><span class="sxs-lookup"><span data-stu-id="369a8-190">**Table 2. Search traversal values**</span></span>

|<span data-ttu-id="369a8-191">**検査値**</span><span class="sxs-lookup"><span data-stu-id="369a8-191">**Traversal value**</span></span>|<span data-ttu-id="369a8-192">**適用されます。**</span><span class="sxs-lookup"><span data-stu-id="369a8-192">**Applies to**</span></span>|<span data-ttu-id="369a8-193">**説明**</span><span class="sxs-lookup"><span data-stu-id="369a8-193">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="369a8-194">浅い</span><span class="sxs-lookup"><span data-stu-id="369a8-194">Shallow</span></span>  <br/> |<span data-ttu-id="369a8-195">アイテムとフォルダー</span><span class="sxs-lookup"><span data-stu-id="369a8-195">Items and Folders</span></span>  <br/> |<span data-ttu-id="369a8-196">浅い検索は、検索対象フォルダーの直接の子に制限されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-196">Shallow searches are limited to direct children of the folder being searched.</span></span>  <br/> |
|<span data-ttu-id="369a8-197">深い</span><span class="sxs-lookup"><span data-stu-id="369a8-197">Deep</span></span>  <br/> |<span data-ttu-id="369a8-198">アイテム (検索フォルダーのみ) とフォルダー</span><span class="sxs-lookup"><span data-stu-id="369a8-198">Items (only with search folders) and Folders</span></span>  <br/> |<span data-ttu-id="369a8-199">深い検索は、検索対象のフォルダーとサブフォルダーを再帰的に検索します。</span><span class="sxs-lookup"><span data-stu-id="369a8-199">Deep searches recursively search the folder being searched and subfolders.</span></span>  <br/> |
|<span data-ttu-id="369a8-200">関連</span><span class="sxs-lookup"><span data-stu-id="369a8-200">Associated</span></span>  <br/> |<span data-ttu-id="369a8-201">アイテム</span><span class="sxs-lookup"><span data-stu-id="369a8-201">Items</span></span>  <br/> |<span data-ttu-id="369a8-p119">関連検索には、検索対象のフォルダーの関連アイテムだけが含まれます。関連アイテムは、フォルダー内にある非表示のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="369a8-p119">Associated searches only include associated items from the folder being searched. Associated items are hidden items within the folder.</span></span>  <br/> |
|<span data-ttu-id="369a8-204">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="369a8-204">SoftDeleted</span></span>  <br/> |<span data-ttu-id="369a8-205">アイテムとフォルダー</span><span class="sxs-lookup"><span data-stu-id="369a8-205">Items and Folders</span></span>  <br/> |<span data-ttu-id="369a8-206">この走査型の使用は推奨されていません。</span><span class="sxs-lookup"><span data-stu-id="369a8-206">This traversal type is deprecated.</span></span> <span data-ttu-id="369a8-207">SoftDeleted の検索に含まれる項目にはのみが含まれます、ごみ箱をあさる。</span><span class="sxs-lookup"><span data-stu-id="369a8-207">SoftDeleted searches only include items that are in the dumpster.</span></span> <span data-ttu-id="369a8-208">ごみ箱をあさる、Office 365 の一部のバージョンの Exchange が Exchange 2010 で始まると、Exchange Online では、[回復可能なアイテム] フォルダー](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx)を Exchange Online に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="369a8-208">The dumpster has been replaced by the [Recoverable Items Folder](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx) in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2010.</span></span>  <br/> |
   
## <a name="managing-search-results"></a><span data-ttu-id="369a8-209">検索結果の管理</span><span class="sxs-lookup"><span data-stu-id="369a8-209">Managing search results</span></span>
<span data-ttu-id="369a8-210"><a name="bk_ManageSearchResults"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-210"></span></span>

<span data-ttu-id="369a8-p121">EWS マネージ API および EWS では、検索結果が返される方法を変更することもできます。ビューを使用することによって、結果に含めるプロパティを指定し、結果を並べ替え、結果をページングして応答ごとに取得する結果を設定した数だけにできます。特定のフィールド値で結果をグループ化したり、走査の種類を指定して検索の深さを制御したりすることもできます。最後に、検索フォルダーを使用して、新しいアイテムが到着したときに動的に更新される永続的な検索を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p121">The EWS Managed API and EWS also allow you to change how your search results are returned. You can use views to specify which properties are included in the results, sort results, and page your results to only get back a set number of results per response. You can also group results by specific field values and control the depth of a search by specifying a traversal type. Finally, you can use search folders to create persistent searches that are updated dynamically as new items arrive.</span></span>
  
### <a name="sorting"></a><span data-ttu-id="369a8-215">並べ替え</span><span class="sxs-lookup"><span data-stu-id="369a8-215">Sorting</span></span>

<span data-ttu-id="369a8-p122">並べ替えられた結果を返すようにサーバーを設定できます。これによって、より簡単にアイテムを順番に表示または処理することができます。この例では、結果は、受信した日時に基づいて最新のアイテムが最初になるように並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p122">You can get the server to return sorted results, which can make it easier to display or process items in order. In this example, the results will be sorted by the date/time received, with the newest items being first.</span></span>
  
```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a><span data-ttu-id="369a8-218">ページング</span><span class="sxs-lookup"><span data-stu-id="369a8-218">Paging</span></span>

<span data-ttu-id="369a8-219">EWS のマネージ API または EWS を使用して、検索要求を送信すると、返されるアイテムの最大数を制御する、ビューのサイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="369a8-219">When you send a search request by using the EWS Managed API or EWS, you specify a view size, which controls the maximum number of items returned.</span></span> <span data-ttu-id="369a8-220">ただし、サーバー上の検索条件に一致するアイテムの数は、ビューのサイズを超える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="369a8-220">However, the number of items on the server that match your search might be larger than the view size.</span></span> <span data-ttu-id="369a8-221">この例では、サーバーでは、他のアイテムがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="369a8-221">In this case, the server indicates that more items are available.</span></span> <span data-ttu-id="369a8-222">[検索を繰り返すにページングを使用](how-to-perform-paged-searches-by-using-ews-in-exchange.md)することができ、次の結果セットを取得します。</span><span class="sxs-lookup"><span data-stu-id="369a8-222">You can [use paging to repeat your search](how-to-perform-paged-searches-by-using-ews-in-exchange.md) and get the next set of results.</span></span> 
  
<span data-ttu-id="369a8-223">たとえば、表示サイズが 10 の検索要求を送信できます。</span><span class="sxs-lookup"><span data-stu-id="369a8-223">For example, you can send a search request with a view size of 10.</span></span> <span data-ttu-id="369a8-224">、検索条件に一致するサーバー上の 15 の項目がある可能性がありますが、のみが表示されます戻ると共に、最初の 10 ( [FindItemsResults\<TItem\>。MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx)プロパティは、EWS のマネージ API を使用している場合)、サーバー上でより多くの結果があること。</span><span class="sxs-lookup"><span data-stu-id="369a8-224">There might be 15 items on the server that match your search, but you will only get back the first 10, along with an indicator (the [FindItemsResults\<TItem\>.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) property if you're using the EWS Managed API) that there are more results on the server.</span></span> <span data-ttu-id="369a8-225">検索条件に一致する次の 10 項目を要求する 10 のオフセットと同じ検索を送信できます。</span><span class="sxs-lookup"><span data-stu-id="369a8-225">You can then send the same search with an offset of 10 to ask for the next 10 items that match your search.</span></span> <span data-ttu-id="369a8-226">残りの 5 つの項目が返されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-226">The server will return the remaining five items.</span></span> 
  
<span data-ttu-id="369a8-227">**図 1 です。ページ単位の検索の例**</span><span class="sxs-lookup"><span data-stu-id="369a8-227">**Figure 1. Paged search example**</span></span>

![図は、ページ検索を示しています。初期要求は 10 アイテムに送信されます。2 番目の要求は次の 10 アイテムに送信されます。](media/Ex15_Search_PagedSearch.png)
  
### <a name="grouping"></a><span data-ttu-id="369a8-231">グループ化</span><span class="sxs-lookup"><span data-stu-id="369a8-231">Grouping</span></span>

 <span data-ttu-id="369a8-p126"> Exchange では、特定のフィールドで検索結果をグループ化できます。これにより、検索結果を管理可能なセットに分割することができます。たとえば、「meeting notes」を検索した結果を、送信者別にグループ化できます。次の図に示されているように、返されたアイテムは複数のグループに分けられます。条件に一致するアイテムで同じ送信者からのものはすべて 1 つのグループに、条件に一致するアイテムで別の送信者からのものはすべて別のグループに、というように分けられます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p126">Exchange enables you to group search results by a specific field. This can help break up search results into more manageable sets. For example, you can search for "meeting notes" and group the results by sender. As shown in the following figure, the items returned will be separated into groups, with all the items that match the criteria from the same sender in one group, all the matching items from another sender in another group, and so on.</span></span> 
  
<span data-ttu-id="369a8-236">**図 2 になります。送信者によってグループ化された検索結果**</span><span class="sxs-lookup"><span data-stu-id="369a8-236">**Figure 2. Search results grouped by sender**</span></span>

![図は、送信者別にグループ化された検索結果を示しています。](media/Ex15_Search_GroupedResults.png)
  
## <a name="search-folders"></a><span data-ttu-id="369a8-238">検索フォルダー</span><span class="sxs-lookup"><span data-stu-id="369a8-238">Search folders</span></span>
<span data-ttu-id="369a8-239"><a name="bk_SearchFolders"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-239"></span></span>

<span data-ttu-id="369a8-p127">通常の検索では、検索が実行されると、結果は処理用にアプリケーションに返され、検索は存在しなくなります。検索フォルダーは、検索を永続的なものにする方法を提供します。これは、検索を複数回実行することがわかっている場合の優れたオプションです。同じ検索を繰り返し実行してサーバーで毎回最初から検索を評価するのではなく、検索フォルダーでは検索を常にオンにします。これにより、アイテムが検索範囲に追加されたり、検索範囲から削除されたりしたときに、サーバーは既存の結果セットを更新できます。検索フォルダーは、アイテムが含まれるフォルダーとして表示されるという意味で、通常のフォルダーと同じように動作します。違いは、フォルダーに含まれるアイテムだけが、フォルダーに関連付けられている検索条件に一致するということです。検索フォルダーが作成されると、アプリケーションは、フォルダーの内容を確認するだけで検索の最新結果を取得できます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p127">With a regular search, the search is executed, the results are returned to your application for processing, and the search ceases to exist. Search folders provide a way to make a search persistent. This is a great option for searches that you know you will want to execute multiple times. Rather than executing the same search repeatedly, causing the server to evaluate the search from scratch each time, a search folder makes a search always on, allowing the server to update the existing result set as items are added to or removed from the search scope. Search folders act like regular folders, in that they appear as folders that have items in them. The difference is that the only items contained in the folder are those that match the search criteria that are associated with the folder. After a search folder is created, your application can get up-to-date results of the search just by checking the contents of the folder.</span></span>
  
<span data-ttu-id="369a8-p128">検索フィルターの作成方法をすでに習得していれば、検索フォルダーを作成するのは簡単です。次の例では、件名に「meeting notes」が含まれるすべてのメールを表示する検索フォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="369a8-p128">Creating a search folder is simple when you've mastered creating search filters. In the following example, a search folder is created to show all email with a subject that contains "meeting notes".</span></span>
  
```cs
static void CreateSearchFolder(ExchangeService service)
{
    SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
        "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "Meeting Notes";
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    searchFolder.SearchParameters.SearchFilter = subjectFilter;
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="in-this-section"></a><span data-ttu-id="369a8-249">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="369a8-249">In this section</span></span>
<span data-ttu-id="369a8-250"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="369a8-250"></span></span>

- [<span data-ttu-id="369a8-251">EWS を使って Exchange 検索フィルターを使用します。</span><span class="sxs-lookup"><span data-stu-id="369a8-251">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)
    
- [<span data-ttu-id="369a8-252">EWS を使用して Exchange、AQS 検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="369a8-252">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="369a8-253">Exchange EWS を使用してページ検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="369a8-253">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="369a8-254">EWS を使用して Exchange によってグループ化された検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="369a8-254">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="369a8-255">EWS を使用して Exchange で検索フォルダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="369a8-255">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="369a8-256">関連項目</span><span class="sxs-lookup"><span data-stu-id="369a8-256">See also</span></span>


- [<span data-ttu-id="369a8-257">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="369a8-257">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- <span data-ttu-id="369a8-258">[回復可能な項目] フォルダー](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx)</span><span class="sxs-lookup"><span data-stu-id="369a8-258">[Recoverable Items Folder](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx)</span></span>
    
- [<span data-ttu-id="369a8-259">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="369a8-259">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="369a8-260">EWS に影響するスロットルのポリシー パラメーターの操作を検索します。</span><span class="sxs-lookup"><span data-stu-id="369a8-260">Throttling policy parameters that affect EWS search operations</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingSearch)
    

