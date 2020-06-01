---
title: Exchange の検索と EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: EWS マネージ API または EWS を使用して、Exchange でアイテムを検索する方法を確認します。
ms.openlocfilehash: d35cc74ab2fa79530ac09256e315a780023d833b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463838"
---
# <a name="search-and-ews-in-exchange"></a><span data-ttu-id="1e4cf-103">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="1e4cf-103">Search and EWS in Exchange</span></span>

<span data-ttu-id="1e4cf-104">EWS マネージ API または EWS を使用して、Exchange でアイテムを検索する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-104">Find out how to search for items in Exchange by using the EWS Managed API or EWS.</span></span>

<span data-ttu-id="1e4cf-p101">次のような流れを経験したことはないでしょうか。数週間先延ばしにしていたあるプロジェクトをやっと開始しようとしたときに、上司から数週間前にメールで受け取った、プロジェクトに関する情報が必要になりました。受信トレイには数百またはおそらく数千ものメッセージがあります。どうしますか。その情報が見つかるまで、メールをスクロールして各件名と送信者のスキャンしますか。または、好みのメール クライアント検索機能を使用して、必要な情報に的を絞りますか。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p101">Does this sound familiar? You're finally starting that project you've been putting off for weeks, and you need information about the project that your manager sent you in email weeks ago. Your Inbox has hundreds or perhaps thousands of messages in it. What do you do? Do you scroll through your email scanning each subject and sender until you find it? Or do you use the search feature in your favorite email client to quickly zero in on what you need?</span></span>

<span data-ttu-id="1e4cf-p102">検索は、ほぼ間違いなくすべてのメール クライアントに備わっている機能です。しかし、検索はユーザーがただ自分のメールボックスを検索できるようにするためのものではありません。特定の期間に含まれる予定をアプリで処理する必要がありますか。特定のステータスのすべてのタスク アイテムについてレポートしたり、特定の会社名を含むすべての連絡先を別のフォルダーに移動したりする必要があるかもしれません。検索によって、これらのすべての要件を満たすことができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p102">Search is arguably a must-have feature for any email client. But search can be used for a lot more than just enabling users to search their mailbox. Does your app need to process appointments that fall within specific time windows? Maybe you need to report on all task items with a specific status, or move all contacts with a specific company name to a different folder. Search can help with all of these requirements.</span></span>

## <a name="search-basics"></a><span data-ttu-id="1e4cf-116">検索の基本</span><span class="sxs-lookup"><span data-stu-id="1e4cf-116">Search basics</span></span>
<span data-ttu-id="1e4cf-117"><a name="bk_SearchBasics"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-117"><a name="bk_SearchBasics"> </a></span></span>

<span data-ttu-id="1e4cf-p103">EWS マネージ API および EWS には、検索方法を指定するための 2 つの基本的な方法があります。[検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)または[クエリ文字列](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)を使用することができます。どちらを使用するかは、検索の目的によって異なります。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p103">The EWS Managed API and EWS offer two basic methods for specifying a search. You can use a [search filter](how-to-use-search-filters-with-ews-in-exchange.md) or a [query string](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). The method you use depends on the intent behind your search.</span></span>

<span data-ttu-id="1e4cf-121">**表 1. 検索フィルターおよび検索クエリのシナリオ**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-121">**Table 1. Scenarios for search filters and search queries**</span></span>

|<span data-ttu-id="1e4cf-122">**目的…**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-122">**If you want to…**</span></span>|<span data-ttu-id="1e4cf-123">**使う機能…**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-123">**Use a…**</span></span>|<span data-ttu-id="1e4cf-124">**注**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-124">**Notes**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1e4cf-125">検索を特定のプロパティまたはプロパティのセットに限定する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-125">Limit your search to a specific property or set of properties</span></span>  <br/> |<span data-ttu-id="1e4cf-126">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-126">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-p104">検索フィルターは、プロパティの検索を最も良く制御できます。クエリ文字列では、高度な検索テクニック (AQS) を使用して限定されたプロパティのセットをターゲットにすることができます。検索フィルターでは任意のプロパティをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p104">Search filters provide the best level of control over which properties are searched. Although query strings can target a limited set of properties by using Advanced Query Syntax (AQS), search filters can target any property.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-129">複数の条件で検索を作成する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-129">Create searches with multiple criteria</span></span>  <br/> |<span data-ttu-id="1e4cf-130">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-130">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-p105">検索フィルターでは、論理 AND または OR を使用して複数の検索条件を結合でき、「件名に '会議ノート' が含まれる、および送信者が 'Sadie Daniels' に等しい」のような検索が可能になります。クエリ文字列では複数の検索条件を結合することもできますが、検索はクエリ文字列でサポートされているプロパティのセットに限定されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p105">With search filters, multiple search criteria can be joined together with logical ANDs or ORs, allowing for searches like "subject contains 'Meeting Notes' AND sender equals 'Sadie Daniels'". Although query strings can also join multiple search criteria, they are limited to the set of properties supported by query strings.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-133">カスタム プロパティの検索</span><span class="sxs-lookup"><span data-stu-id="1e4cf-133">Search custom properties</span></span>  <br/> |<span data-ttu-id="1e4cf-134">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-134">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-p106">検索フィルターは、カスタム プロパティをターゲットにすることができます。クエリ文字列は、カスタム プロパティを検索しません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p106">Search filters can target custom properties. Query strings do not search custom properties.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-137">文字列プロパティの大文字と小文字を区別する検索を実行する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-137">Perform a case sensitive search of string properties</span></span>  <br/> |<span data-ttu-id="1e4cf-138">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-138">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-139">クエリ文字列では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-139">Query string searches are not case sensitive.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-140">文字列プロパティを検索するときに含有モードを制御する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-140">Control the containment mode when searching string properties</span></span>  <br/> |<span data-ttu-id="1e4cf-141">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-141">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-p107">クエリ文字列の検索は常に、部分文字列の検索になります。特定のプレフィックスを検索する場合や、完全一致が必要な場合は、検索フィルターを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p107">Query string searches are always substring searches. If you need to search for specific prefixes, or require exact matches, a search filter is the best choice.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-144">フォルダーを検索する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-144">Search for folders</span></span>  <br/> |<span data-ttu-id="1e4cf-145">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-145">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-146">EWS では、クエリ文字列によるフォルダーの検索はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-146">EWS does not support searching for folders with a query string.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-147">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-147">Create a search folder</span></span>  <br/> |<span data-ttu-id="1e4cf-148">検索フィルター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-148">Search filter</span></span>  <br/> |<span data-ttu-id="1e4cf-149">EWS では、クエリ文字列による検索フォルダーの作成はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-149">EWS does not support creating search folders with a query string.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-150">一般的に使用されるすべてのプロパティを検索する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-150">Search across all commonly used properties</span></span>  <br/> |<span data-ttu-id="1e4cf-151">クエリ文字列</span><span class="sxs-lookup"><span data-stu-id="1e4cf-151">Query string</span></span>  <br/> |<span data-ttu-id="1e4cf-p108">AQS が含まれていないクエリ文字列は、一般的に使用されるすべてのプロパティを検索します。たとえば、クエリ文字列値が「Mack Chaves」である場合、Mack Chaves によって送信されたすべてのメッセージ、および本文または件名に「Mack Chaves」が含まれるすべてのメッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p108">Query strings that do not contain AQS will search across all commonly used properties. For example, a query string value of "Mack Chaves" will return all messages sent by Mack Chaves as well as any messages that have "Mack Chaves" in the body or subject.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-154">単純なユーザー入力に基づいた検索を作成する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-154">Construct a search based on simple user input</span></span>  <br/> |<span data-ttu-id="1e4cf-155">クエリ文字列</span><span class="sxs-lookup"><span data-stu-id="1e4cf-155">Query string</span></span>  <br/> |<span data-ttu-id="1e4cf-p109">クエリ文字列は、エンド ユーザーが単純な文字列を入力してクイック検索を実行するための最適な選択肢です。クエリ文字列の検索には、一般的に使用されるすべてのプロパティが含まれるため、ユーザーの検索語句を含むすべてのアイテムが結果に含まれます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p109">A query string is a great choice for allowing an end user to do a quick search by typing in a simple string. Because a query string search includes all commonly used properties, the results will contain any items that contain the user's search terms.</span></span>  <br/> |

### <a name="using-a-search-filter"></a><span data-ttu-id="1e4cf-158">検索フィルターの使用</span><span class="sxs-lookup"><span data-stu-id="1e4cf-158">Using a search filter</span></span>

<span data-ttu-id="1e4cf-p110">検索フィルターでは、さまざまな検索オプションを使用し、検索の実行方法を最高度に制御できます。検索フィルターを使用して、基本的な等値検索と比較検索を実行できますが、さらに、文字列プロパティの内容を検索したりビットマスクの比較を実行することも可能です。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p110">Search filters give you a wide range of search options and the greatest degree of control over how the search is performed. You can use search filters to perform basic equality and comparison searches, but you can also search within the contents of string properties or do bitmask comparisons.</span></span>

<span data-ttu-id="1e4cf-161">たとえば、EWS マネージ API で [SearchFilter.ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) クラスを使用して、アイテムの件名の内容を検索することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-161">For example, you can search the contents of the subject of items by using the [SearchFilter.ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class in the EWS Managed API.</span></span> <span data-ttu-id="1e4cf-162">この例では、部分文字列「meeting notes」(大文字と小文字を区別しない) が含まれている件名を検索する検索フィルターが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-162">In this example, a search filter is created to search the subject for the substring "meeting notes", ignoring case.</span></span>

```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

<span data-ttu-id="1e4cf-p112">カスタム プロパティを検索対象にすることもできます。この例では、3 より大きい値が含まれてるカスタム プロパティ **ItemIndex** を検索します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p112">You can also search against custom properties. In this example, the custom property **ItemIndex** is searched for values greater than 3.</span></span>

```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer);
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

<span data-ttu-id="1e4cf-165">複数の検索フィルターを組み合わせて、より複雑な検索を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-165">You can also combine multiple search filters to create more complex searches.</span></span> <span data-ttu-id="1e4cf-166">たとえば、[SearchFilter.SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) クラスを使用して、先ほどの 2 つのフィルターを論理 AND で組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-166">For example, you can combine the previous two filters with a logical AND by using the [SearchFilter.SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) class.</span></span>

```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a><span data-ttu-id="1e4cf-167">クエリ文字列の使用</span><span class="sxs-lookup"><span data-stu-id="1e4cf-167">Using a query string</span></span>

<span data-ttu-id="1e4cf-168">クエリ文字列は、異なるアプローチで検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-168">Query strings provide a different approach to search.</span></span> <span data-ttu-id="1e4cf-169">クエリ文字列による検索は、検索するフィールドおよび検索を実行する方法をそれほど制御できません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-169">You have less control over the fields that are searched and how the search is performed when you use a query string search.</span></span> <span data-ttu-id="1e4cf-170">しかし、これは大きな問題ではありません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-170">Not that that's a bad thing!</span></span> <span data-ttu-id="1e4cf-171">いわゆる「大きな網を投げる」場合があるかもしれません。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-171">In some cases, you might want to cast a wider net, so to speak.</span></span>

<span data-ttu-id="1e4cf-172">たとえば、[ExchangeService.FindItems](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して「meeting notes」を検索することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-172">For example, you can search for "meeting notes" by using the [ExchangeService.FindItems](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx) EWS Managed API method.</span></span>

```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

<span data-ttu-id="1e4cf-p115">先ほどの **SearchFilter.ContainsSubstring** 検索例の結果と比較した場合、この検索のほうが結果が多くなります。検索フィルターによる検索では、件名に「meeting notes」が含まれるアイテムのみが返されます。しかし、この検索では、件名、本文、およびその他のフィールドに「meeting notes」が含まれるアイテムが返されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p115">If you compare the results of this search to the results of the **SearchFilter.ContainsSubstring** search example earlier, this search will contain more results. The search filter search will return only items that have "meeting notes" in the subject, while this search will return items that have "meeting notes" in the subject, body, and other fields.</span></span>

<span data-ttu-id="1e4cf-p116">クエリ文字列を調整して、検索フィルターの結果に近くなる、絞り込み方法を見てみましょう。AQS を使用すると、検索を件名に制限することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p116">Let's take a look at how you can refine the query string to get closer to the results you see from the search filter. Using AQS, you can limit your search to the subject.</span></span>

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

<span data-ttu-id="1e4cf-p117">これでかなり近くなりますが、結果はまだ同じではありません。複数の文字が含まれるクエリ文字列を使用すると、それらの単語が指定した順序どおりでない場合や、それらの単語が隣接していない場合でも、一致となります。クエリ文字列「subject:meeting notes」を使用すると、「meeting notes」、「notes from the meeting」が一致となります。さらに絞り込むには、検索用語を二重引用符で囲み、その語句だけを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p117">This is closer, but the results are still not quite the same. When you use a query string with multiple words, you will get matches even if the words are not in the order you specify, or even if they're not adjacent to each other. With the query string "subject:meeting notes", you will get matches for "meeting notes", "notes from the meeting", and so on. To further refine, you can wrap the search terms in double quotes to indicate that you want that phrase only.</span></span>

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a><span data-ttu-id="1e4cf-181">検索結果で特定のプロパティを要求する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-181">Requesting specific properties in search results</span></span>
<span data-ttu-id="1e4cf-182"><a name="bk_RequestSpecific"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-182"><a name="bk_RequestSpecific"> </a></span></span>

<span data-ttu-id="1e4cf-183">既定では、検索に一致するアイテムのすべてのプロパティが検索結果に含まれます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-183">By default, search results will contain all properties on the items that match the search.</span></span> <span data-ttu-id="1e4cf-184">これが希望どおりの結果である場合もありますが、ほとんどの場合、アプリケーションが必要とするのはプロパティの個別セットのみです。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-184">In some cases this might be what you want, but in most cases your application only requires a discrete set of properties.</span></span> <span data-ttu-id="1e4cf-185">この場合、返されるプロパティのセットを、アプリケーションが必要とするプロパティのみに制限する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-185">In this case, you should limit the set of properties that are returned to only the properties your application needs.</span></span> <span data-ttu-id="1e4cf-186">次の例では、[ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) クラスを使用して、返されるプロパティをアイテムの件名、受信日時、ID に制限します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-186">In the following example, the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class is used to limit the returned properties to the subject, date/time received, and ID of the items.</span></span>

```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a><span data-ttu-id="1e4cf-187">検索の深さの制御</span><span class="sxs-lookup"><span data-stu-id="1e4cf-187">Controlling search depth</span></span>
<span data-ttu-id="1e4cf-188"><a name="bk_SearchDepth"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-188"><a name="bk_SearchDepth"> </a></span></span>

<span data-ttu-id="1e4cf-189">ビュー上で走査の設定をすることによって、検索の範囲と深さを制御します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-189">Setting the traversal on the view controls the depth and scope of the search.</span></span>

<span data-ttu-id="1e4cf-190">**表 2. 検索走査値**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-190">**Table 2. Search traversal values**</span></span>

|<span data-ttu-id="1e4cf-191">**走査値**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-191">**Traversal value**</span></span>|<span data-ttu-id="1e4cf-192">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-192">**Applies to**</span></span>|<span data-ttu-id="1e4cf-193">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-193">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1e4cf-194">浅い</span><span class="sxs-lookup"><span data-stu-id="1e4cf-194">Shallow</span></span>  <br/> |<span data-ttu-id="1e4cf-195">アイテムとフォルダー</span><span class="sxs-lookup"><span data-stu-id="1e4cf-195">Items and Folders</span></span>  <br/> |<span data-ttu-id="1e4cf-196">浅い検索は、検索対象フォルダーの直接の子に制限されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-196">Shallow searches are limited to direct children of the folder being searched.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-197">深い</span><span class="sxs-lookup"><span data-stu-id="1e4cf-197">Deep</span></span>  <br/> |<span data-ttu-id="1e4cf-198">アイテム (検索フォルダーのみ) とフォルダー</span><span class="sxs-lookup"><span data-stu-id="1e4cf-198">Items (only with search folders) and Folders</span></span>  <br/> |<span data-ttu-id="1e4cf-199">深い検索は、検索対象のフォルダーとサブフォルダーを再帰的に検索します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-199">Deep searches recursively search the folder being searched and subfolders.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-200">関連</span><span class="sxs-lookup"><span data-stu-id="1e4cf-200">Associated</span></span>  <br/> |<span data-ttu-id="1e4cf-201">Items</span><span class="sxs-lookup"><span data-stu-id="1e4cf-201">Items</span></span>  <br/> |<span data-ttu-id="1e4cf-p119">関連検索には、検索対象のフォルダーの関連アイテムだけが含まれます。関連アイテムは、フォルダー内にある非表示のアイテムです。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p119">Associated searches only include associated items from the folder being searched. Associated items are hidden items within the folder.</span></span>  <br/> |
|<span data-ttu-id="1e4cf-204">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="1e4cf-204">SoftDeleted</span></span>  <br/> |<span data-ttu-id="1e4cf-205">アイテムとフォルダー</span><span class="sxs-lookup"><span data-stu-id="1e4cf-205">Items and Folders</span></span>  <br/> |<span data-ttu-id="1e4cf-p120">この走査の種類は廃止されました。削除済み (回復可能) の検索には、ごみ箱にあるアイテムのみが含まれます。このごみ箱は、Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2010 以降のバージョンの Exchange では、[回復可能なアイテム フォルダー](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)に置き換えられています。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p120">This traversal type is deprecated. SoftDeleted searches only include items that are in the dumpster. The dumpster has been replaced by the [Recoverable Items Folder](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder) in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2010.  </span></span><br/> |

## <a name="managing-search-results"></a><span data-ttu-id="1e4cf-209">検索結果の管理</span><span class="sxs-lookup"><span data-stu-id="1e4cf-209">Managing search results</span></span>
<span data-ttu-id="1e4cf-210"><a name="bk_ManageSearchResults"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-210"><a name="bk_ManageSearchResults"> </a></span></span>

<span data-ttu-id="1e4cf-p121">EWS マネージ API および EWS では、検索結果が返される方法を変更することもできます。ビューを使用することによって、結果に含めるプロパティを指定し、結果を並べ替え、結果をページングして応答ごとに取得する結果を設定した数だけにできます。特定のフィールド値で結果をグループ化したり、走査の種類を指定して検索の深さを制御したりすることもできます。最後に、検索フォルダーを使用して、新しいアイテムが到着したときに動的に更新される永続的な検索を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p121">The EWS Managed API and EWS also allow you to change how your search results are returned. You can use views to specify which properties are included in the results, sort results, and page your results to only get back a set number of results per response. You can also group results by specific field values and control the depth of a search by specifying a traversal type. Finally, you can use search folders to create persistent searches that are updated dynamically as new items arrive.</span></span>

### <a name="sorting"></a><span data-ttu-id="1e4cf-215">並べ替え</span><span class="sxs-lookup"><span data-stu-id="1e4cf-215">Sorting</span></span>

<span data-ttu-id="1e4cf-p122">並べ替えられた結果を返すようにサーバーを設定できます。これによって、より簡単にアイテムを順番に表示または処理することができます。この例では、結果は、受信した日時に基づいて最新のアイテムが最初になるように並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p122">You can get the server to return sorted results, which can make it easier to display or process items in order. In this example, the results will be sorted by the date/time received, with the newest items being first.</span></span>

```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a><span data-ttu-id="1e4cf-218">ページング</span><span class="sxs-lookup"><span data-stu-id="1e4cf-218">Paging</span></span>

<span data-ttu-id="1e4cf-p123">EWS マネージ API または EWS を使用して検索要求を送信するときに、ビューのサイズを指定します。これにより、返されるアイテムの最大数が制御されます。ただし、検索に一致するサーバー上のアイテム数は、ビューのサイズを超える可能性があります。この場合、サーバーは利用できるアイテムがさらに多く存在することを示します。[ページングを使用して検索を繰り返し](how-to-perform-paged-searches-by-using-ews-in-exchange.md)、次の結果セットを取得できます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p123">When you send a search request by using the EWS Managed API or EWS, you specify a view size, which controls the maximum number of items returned. However, the number of items on the server that match your search might be larger than the view size. In this case, the server indicates that more items are available. You can [use paging to repeat your search](how-to-perform-paged-searches-by-using-ews-in-exchange.md) and get the next set of results.</span></span>

<span data-ttu-id="1e4cf-223">たとえば、ビュー サイズが 10 の検索要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-223">For example, you can send a search request with a view size of 10.</span></span> <span data-ttu-id="1e4cf-224">サーバー上には検索に一致するアイテムが15個あるかもしれませんが、最初の10はインジケーター ( [Finditemsresults) と共に返されます \<TItem\> 。](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx)EWS マネージ API を使用している場合は、さらに多くのプロパティを使用して、サーバー上にさらに結果があることを示します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-224">There might be 15 items on the server that match your search, but you will only get back the first 10, along with an indicator (the [FindItemsResults\<TItem\>.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property if you're using the EWS Managed API) that there are more results on the server.</span></span> <span data-ttu-id="1e4cf-225">その場合、オフセットを 10 にして同じ検索を送信し、検索条件に一致する次の 10 アイテムを要求することができます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-225">You can then send the same search with an offset of 10 to ask for the next 10 items that match your search.</span></span> <span data-ttu-id="1e4cf-226">サーバーは残りの 5 つのアイテムを返します。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-226">The server will return the remaining five items.</span></span>

<span data-ttu-id="1e4cf-227">**図 1. ページングされた検索の例**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-227">**Figure 1. Paged search example**</span></span>

![図は、ページ検索を示しています。初期要求は 10 アイテムに送信されます。2 番目の要求は次の 10 アイテムに送信されます。](media/Ex15_Search_PagedSearch.png)

### <a name="grouping"></a><span data-ttu-id="1e4cf-231">グループ化</span><span class="sxs-lookup"><span data-stu-id="1e4cf-231">Grouping</span></span>

 <span data-ttu-id="1e4cf-p126"> Exchange では、特定のフィールドで検索結果をグループ化できます。これにより、検索結果を管理可能なセットに分割することができます。たとえば、「meeting notes」を検索した結果を、送信者別にグループ化できます。次の図に示されているように、返されたアイテムは複数のグループに分けられます。条件に一致するアイテムで同じ送信者からのものはすべて 1 つのグループに、条件に一致するアイテムで別の送信者からのものはすべて別のグループに、というように分けられます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p126">Exchange enables you to group search results by a specific field. This can help break up search results into more manageable sets. For example, you can search for "meeting notes" and group the results by sender. As shown in the following figure, the items returned will be separated into groups, with all the items that match the criteria from the same sender in one group, all the matching items from another sender in another group, and so on.</span></span>

<span data-ttu-id="1e4cf-236">**図 2. 送信者別にグループ化された検索結果**</span><span class="sxs-lookup"><span data-stu-id="1e4cf-236">**Figure 2. Search results grouped by sender**</span></span>

![図は、送信者別にグループ化された検索結果を示しています。](media/Ex15_Search_GroupedResults.png)

## <a name="search-folders"></a><span data-ttu-id="1e4cf-238">検索フォルダー</span><span class="sxs-lookup"><span data-stu-id="1e4cf-238">Search folders</span></span>
<span data-ttu-id="1e4cf-239"><a name="bk_SearchFolders"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-239"><a name="bk_SearchFolders"> </a></span></span>

<span data-ttu-id="1e4cf-p127">通常の検索では、検索が実行されると、結果は処理用にアプリケーションに返され、検索は存在しなくなります。検索フォルダーは、検索を永続的なものにする方法を提供します。これは、検索を複数回実行することがわかっている場合の優れたオプションです。同じ検索を繰り返し実行してサーバーで毎回最初から検索を評価するのではなく、検索フォルダーでは検索を常にオンにします。これにより、アイテムが検索範囲に追加されたり、検索範囲から削除されたりしたときに、サーバーは既存の結果セットを更新できます。検索フォルダーは、アイテムが含まれるフォルダーとして表示されるという意味で、通常のフォルダーと同じように動作します。違いは、フォルダーに含まれるアイテムだけが、フォルダーに関連付けられている検索条件に一致するということです。検索フォルダーが作成されると、アプリケーションは、フォルダーの内容を確認するだけで検索の最新結果を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p127">With a regular search, the search is executed, the results are returned to your application for processing, and the search ceases to exist. Search folders provide a way to make a search persistent. This is a great option for searches that you know you will want to execute multiple times. Rather than executing the same search repeatedly, causing the server to evaluate the search from scratch each time, a search folder makes a search always on, allowing the server to update the existing result set as items are added to or removed from the search scope. Search folders act like regular folders, in that they appear as folders that have items in them. The difference is that the only items contained in the folder are those that match the search criteria that are associated with the folder. After a search folder is created, your application can get up-to-date results of the search just by checking the contents of the folder.</span></span>

<span data-ttu-id="1e4cf-p128">検索フィルターの作成方法をすでに習得していれば、検索フォルダーを作成するのは簡単です。次の例では、件名に「meeting notes」が含まれるすべてのメールを表示する検索フォルダーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1e4cf-p128">Creating a search folder is simple when you've mastered creating search filters. In the following example, a search folder is created to show all email with a subject that contains "meeting notes".</span></span>

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

## <a name="in-this-section"></a><span data-ttu-id="1e4cf-249">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="1e4cf-249">In this section</span></span>
<span data-ttu-id="1e4cf-250"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="1e4cf-250"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="1e4cf-251">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-251">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)

- [<span data-ttu-id="1e4cf-252">Exchange で EWS を使用して AQS 検索を実行する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-252">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)

- [<span data-ttu-id="1e4cf-253">Exchange で EWS を使用してページング検索を実行する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-253">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)

- [<span data-ttu-id="1e4cf-254">Exchange で EWS を使用して、グループ化された検索を実行する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-254">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)

- [<span data-ttu-id="1e4cf-255">Exchange で EWS を使用して検索フォルダーを操作する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-255">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)

## <a name="see-also"></a><span data-ttu-id="1e4cf-256">関連項目</span><span class="sxs-lookup"><span data-stu-id="1e4cf-256">See also</span></span>


- [<span data-ttu-id="1e4cf-257">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="1e4cf-257">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)

- [<span data-ttu-id="1e4cf-258">回復可能なアイテム フォルダー</span><span class="sxs-lookup"><span data-stu-id="1e4cf-258">Recoverable Items Folder</span></span>](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)

- [<span data-ttu-id="1e4cf-259">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="1e4cf-259">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)

- [<span data-ttu-id="1e4cf-260">EWS の検索操作に影響を与える調整ポリシーのパラメーター</span><span class="sxs-lookup"><span data-stu-id="1e4cf-260">Throttling policy parameters that affect EWS search operations</span></span>](ews-throttling-in-exchange.md#throttling-policy-parameters-that-affect-ews-search-operations)
