---
title: Exchange EWS を使用してページ検索を実行します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Exchange を対象とする EWS マネージ API または EWS のアプリケーションでページングされた検索を実行する方法を説明します。
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759038"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="9e84e-103">Exchange EWS を使用してページ検索を実行します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="9e84e-104">Exchange を対象とする EWS マネージ API または EWS のアプリケーションでページングされた検索を実行する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="9e84e-p101">ページングは、検索結果のサイズを制御するための EWS の機能です。1 度の EWS の応答で検索セット全体を取得する代わりに、複数の EWS 応答で小さなセットに分けて取得できます。たとえば、受信トレイに 10,000 件のメール メッセージがあるユーザーについて検討します。仮に、10,000 件のメールすべてを 1 度の大規模な応答で取得できる場合でも、帯域幅またはパフォーマンス上の理由でより管理しやすいチャンクに分割することを望まれるかもしれません。ページングは、そうするのに最適なツールを提供します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p101">Paging is a feature in EWS that enables you to control the size of the results of a search. Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses. For example, consider a user with 10,000 email messages in their Inbox. Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons. Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="9e84e-110">実際に要求が 1 つで 10,000 個のアイテムを取得することができますと仮定、EWS の調整のため可能性がありますこれはありません。</span><span class="sxs-lookup"><span data-stu-id="9e84e-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="9e84e-111">詳細については、 [EWS が Exchange で調整](ews-throttling-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e84e-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="9e84e-112">**表 1 です。EWS のマネージ API および EWS でのページングのパラメーター**</span><span class="sxs-lookup"><span data-stu-id="9e84e-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="9e84e-113">**設定または取得する、.**</span><span class="sxs-lookup"><span data-stu-id="9e84e-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="9e84e-114">**EWS のマネージ API で次のコマンドを使用してください.**</span><span class="sxs-lookup"><span data-stu-id="9e84e-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="9e84e-115">**EWS で次のコマンドを使用してください.**</span><span class="sxs-lookup"><span data-stu-id="9e84e-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9e84e-116">応答中のアイテムまたはフォルダーの最大数</span><span class="sxs-lookup"><span data-stu-id="9e84e-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="9e84e-117">**PageSize**パラメーター [ItemView のコンス トラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx)または[FolderView コンス トラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="9e84e-117">The **pageSize** parameter to the [ItemView constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="9e84e-118">Or</span><span class="sxs-lookup"><span data-stu-id="9e84e-118">Or</span></span>  <br/> <span data-ttu-id="9e84e-119">[PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-119">The [PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-120">[IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要素または[IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)要素の**MaxEntriesReturned**属性</span><span class="sxs-lookup"><span data-stu-id="9e84e-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="9e84e-121">アイテムまたはフォルダーのリストの開始点</span><span class="sxs-lookup"><span data-stu-id="9e84e-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="9e84e-122">**OffsetBasePoint** **ItemView**コンス トラクターまたは**FolderView**コンス トラクターのパラメーター</span><span class="sxs-lookup"><span data-stu-id="9e84e-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="9e84e-123">Or</span><span class="sxs-lookup"><span data-stu-id="9e84e-123">Or</span></span>  <br/> <span data-ttu-id="9e84e-124">[PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-124">The [PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-125">**IndexedPageItemView**要素または**IndexedPageFolderView**要素の**ベース ポイント**属性</span><span class="sxs-lookup"><span data-stu-id="9e84e-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="9e84e-126">開始点からのオフセット</span><span class="sxs-lookup"><span data-stu-id="9e84e-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="9e84e-127">**ItemView**コンス トラクターまたは**FolderView**コンス トラクターに**offset**パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e84e-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="9e84e-128">Or</span><span class="sxs-lookup"><span data-stu-id="9e84e-128">Or</span></span>  <br/> <span data-ttu-id="9e84e-129">[PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-129">The [PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-130">**オフセット**属性は、 **IndexedPageItemView**要素または**IndexedPageFolderView**要素の</span><span class="sxs-lookup"><span data-stu-id="9e84e-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="9e84e-131">サーバー上の結果の総数</span><span class="sxs-lookup"><span data-stu-id="9e84e-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="9e84e-132">[FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-132">The [FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-133">[RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx)の要素に[して (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)の要素の**TotalItemsInView**属性</span><span class="sxs-lookup"><span data-stu-id="9e84e-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="9e84e-134">現在の応答に含まれない次のアイテムまたはフォルダーのオフセット</span><span class="sxs-lookup"><span data-stu-id="9e84e-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="9e84e-135">[FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-135">The [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-136">**RootFolder**要素の**IndexedPagingOffset**属性</span><span class="sxs-lookup"><span data-stu-id="9e84e-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="9e84e-137">応答が最後のアイテムまたはフォルダーをリストに含んでいるかどうかを示すインジケーター</span><span class="sxs-lookup"><span data-stu-id="9e84e-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="9e84e-138">[FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e84e-138">The [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="9e84e-139">**RootFolder**要素の**IncludesLastItemInRange**属性</span><span class="sxs-lookup"><span data-stu-id="9e84e-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="9e84e-140">ページングのしくみ</span><span class="sxs-lookup"><span data-stu-id="9e84e-140">How paging works</span></span>
<span data-ttu-id="9e84e-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="9e84e-141"></span></span>

<span data-ttu-id="9e84e-p103">ページングのしくみを理解するには、フォルダー内のメッセージを屋外に並べられた広告版に置き換えて考えると分かりやすくなります。これらの広告版のいくつかを魔法のウィンドウを通して見ることができます。ウィンドウのサイズを変更 (同時に表示する広告版の数を増やすまたは減らすため) したり、ウィンドウを移動 (表示する広告版を制御するため) したりできます。このウィンドウの操作がページングです。 </span><span class="sxs-lookup"><span data-stu-id="9e84e-p103">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house. You can see some of these billboards through a magical window. You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see). This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="9e84e-p104">要求を Exchange サーバーに送信する際、返すアイテム数を指定するためにウィンドウのサイズを指定します。開始点 (行の先頭または末尾) とその開始点からのオフセット (アイテム数で表す) を指定して、ウィンドウの位置を設定します。ウィンドウの先頭は、開始点からのオフセットで指定されたアイテムの数です。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p104">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return. You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items. The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="9e84e-p105">ページングの魅力は、サーバーの応答と、その応答をアプリケーションで使用して次の要求を形成する際に発揮されます。次の要求に備えて "ウィンドウ" を構成する方法を決定するのに使用できる次の 3 つの情報がサーバーから提供されます。 </span><span class="sxs-lookup"><span data-stu-id="9e84e-p105">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request. The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="9e84e-151">応答に含まれている結果に、サーバー上の結果セット全体の最後のアイテムが含まれているかどうか。</span><span class="sxs-lookup"><span data-stu-id="9e84e-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="9e84e-152">サーバー上の結果セットのアイテムの合計数。</span><span class="sxs-lookup"><span data-stu-id="9e84e-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="9e84e-153">現在の応答に含まれていない、結果セット内の次のアイテムにウィンドウを移動する場合に指定すべきオフセットの値。</span><span class="sxs-lookup"><span data-stu-id="9e84e-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="9e84e-p106">簡単な例を見てみましょう。受信トレイに 15 件のメッセージがあるとします。アプリケーションによって、メッセージのリストの初めから最大 10 個のアイテム (オフセットは 0 になります) を取得するための最初の要求が送信されます。サーバーからの応答には最初の 10 件のメッセージが含まれ、応答には最後のアイテムが含まれておらず、合計 15 個のアイテムがあり、次のオフセットを 10 にする必要があることが示されます。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p106">Let's look at a simple example. Imagine an Inbox with 15 messages in it. Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero). The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="9e84e-158">**図 1 です。15 項目の一覧の先頭からオフセット 0 から 10 個のアイテムを要求します。**</span><span class="sxs-lookup"><span data-stu-id="9e84e-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![15 アイテムのリストの初めからオフセット 0 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="9e84e-p107">次にアプリケーションは、同じ要求をサーバーに再送信します。変更されたのはオフセットが 10 になったという点だけです。サーバーは、最後の 5 アイテムを返し、応答に最後のアイテムが含まれており、合計 15 個のアイテムがあり、次のオフセットを 15 にする必要があることが示されます (もちろん、末尾に達したため、次のオフセットはありません)。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p107">Your application then resends the same request to the server, with the only change being that the offset is now 10. The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="9e84e-162">**図 2 になります。15 項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**</span><span class="sxs-lookup"><span data-stu-id="9e84e-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![15 アイテムのリストの初めからオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="9e84e-164">ページングのデザイン上の考慮事項</span><span class="sxs-lookup"><span data-stu-id="9e84e-164">Design considerations for paging</span></span>
<span data-ttu-id="9e84e-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="9e84e-165"></span></span>

<span data-ttu-id="9e84e-p108">アプリケーションでページングを最大限活用するには、考慮すべき事項があります。たとえば、"ウィンドウ" のサイズをどのように決めるか、"ウィンドウ" の移動中にサーバ上の結果を変更された場合にどうするかなどです。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p108">Making the most out of paging in your application does require some consideration. For example, how large do you make your "window"? What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="9e84e-169">ウィンドウのサイズの決定</span><span class="sxs-lookup"><span data-stu-id="9e84e-169">Determine the size of your window</span></span>

<span data-ttu-id="9e84e-p109">すべてのアプリケーションが使用するべき、あらゆる状況に適したエントリの最大数といったものはありません。アプリケーションにとって適切な数は、いくつかの異なる要素に基づいて決定されます。しかし、次のガイドラインに従うと便利です。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p109">There is no "one-size-fits-all" maximum number of entries that all applications should use. Determining the number that's right for your application depends on several different factors. However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="9e84e-173">既定で、Exchange では 1 つの要求に返すことのできる最大アイテム数を 1000 に限定しています。</span><span class="sxs-lookup"><span data-stu-id="9e84e-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="9e84e-174">エントリの最大数を大きい数字に設定すると、すべてのアイテムを取得するのに送信する要求の数は少なくなりますが、応答の待機時間が長くなります。</span><span class="sxs-lookup"><span data-stu-id="9e84e-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="9e84e-175">エントリの最大数を小さい数に設定すると、応答時間が短くなりますが、すべてのアイテムを取得するのに送信する要求の数が増えます。</span><span class="sxs-lookup"><span data-stu-id="9e84e-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="9e84e-176">結果セットが変更された場合の処理</span><span class="sxs-lookup"><span data-stu-id="9e84e-176">Handling changes to the result set</span></span>

<span data-ttu-id="9e84e-p110">前述の例では、ユーザーの受信トレイ内のアイテム数が一定でした。ただし、実際には、受信トレイ内のアイテム数は頻繁に変更されることがあります。いつでも、新しいメッセージが到着したり、アイテムが削除または移動されることがあります。これは、どのようにページングに影響するでしょうか?前述の例のシナリオを変更して確認しましょう。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p110">In the simple example earlier in this article, the number of items in the user's Inbox remained constant. However, in reality, the number of items in an Inbox can change frequently. New messages can arrive and items can be deleted or moved at any time. But how does this impact paging? Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="9e84e-p111">再度、ユーザーの受信トレイには 15 アイテムある設定で、同じ最初の要求を送信します。先の例同様、サーバーからの応答として最初の 10 件のメッセージが含まれ、応答に最後のアイテムが含まれておらず、合計 15 個のアイテムがあり、次のオフセットを 10 にする必要があることが示されます (図 1)。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p111">We'll start again with the 15 items in the user's Inbox, and send the same initial request. As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="9e84e-p112">アプリケーションでそれら 10 のアイテムが処理されている間、新しいメッセージが受信トレイに到着し、サーバーの結果セットに追加されます。アプリケーションが同じ要求をサーバーに再送信します (オフセットが 10 に設定されている)。今回の場合、サーバーは 6 アイテムを返し、合計 16 アイテムが結果セットにあることが示されます。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p112">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server. Your application resends the same request to the server (only with the offset set to 10). This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="9e84e-p113">この時点で、これが問題かどうか認識できないかもしれません。結局のところ、2 つの応答を通して 16 アイテムが返されただけのことです。答えは、新しいアイテムがリストのどこに配置されたかによって異なります。最も古いアイテム (受信した日時順) が先頭に来るようにリストが並べ替えられている場合、このシナリオでは心配する要因となるものはありません。新しいアイテムはリストの末尾に配置され、2 番目の応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p113">At this point you might be wondering if this is even a problem. After all, you got 16 items back over the two responses, so why all the fuss? The answer depends on where in the list the new item is placed. If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario. The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="9e84e-192">**図 3 です。新しいされているリスト内の 16 の項目で 16 の項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**</span><span class="sxs-lookup"><span data-stu-id="9e84e-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![16 番目のアイテムがリストの終わりに追加されたときに、16 アイテムのリストの最初からオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="9e84e-p114">最新のアイテムが最初になるように、リストが並べ替えられている場合は、別の話です。この例では、2 番目の要求の最初のアイテムがその前の要求の最後のアイテムになり、残りの 5 アイテムは元の 15 アイテムのものです。仮想的な魔法のウィンドウという観点で考えると、ウィンドウの位置は 10 移動しましたが、広告版自体も 1 移動したことになります。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p114">If the list is sorted so that the newest items are first, it's a different story. In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15. To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="9e84e-197">**図 4 です。新しいされているリストの最初の項目で 16 の項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**</span><span class="sxs-lookup"><span data-stu-id="9e84e-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![16 番目のアイテムがリストの初めに追加されたときに、16 アイテムのリストの最初からオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="9e84e-p115">サーバー上の結果に加えられた変更を特定する 1 つの方法は、アンカー アイテムの概念を使用することです。アンカー アイテムは、結果の残りの部分と一緒には処理されない、応答に追加されたアイテムです。次の結果と比較して、アイテム自体が移動したかどうかを確認するために使用されます。先の簡単な例では、アプリケーションで "ウィンドウ" のサイズを 10 に設定している場合、実際には戻るアイテムの最大数を 11 に設定していることになります。アプリケーションでは、通常どおり、応答の最初の 10 アイテムを処理します。最後のアイテムについて、アイテムの識別子をアンカーとして保存してから、オフセットが 10 の次の要求を発行します。データが変更されていない場合、2 番目の応答の最初のアイテムにはアンカーと一致するアイテムの識別子があるはずです。アイテムの識別子が一致しない場合は、データが削除されたか、既にページングしたリストの特定の箇所に挿入されたことが分かります。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p115">One way to detect a change to the results on the server is to use the concept of an anchor item. An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted. Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11. Your application processes the first 10 items in the response as usual. For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10. If the data has not changed, the first item in the second response should have an item identifier that matches the anchor. If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="9e84e-206">わかっている場合、データが変更されたことをする必要がありますに対処する方法を決定します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="9e84e-207">か、この質問のニーズによって異なるものの応答がありません。</span><span class="sxs-lookup"><span data-stu-id="9e84e-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="9e84e-208">アクションは、アプリケーションとすべての項目を取得することが重要な方法の性質によって異なります。</span><span class="sxs-lookup"><span data-stu-id="9e84e-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="9e84e-209">完全無視して、先頭から処理を再開または、トラックをバックアップするか、および変更の発生場所を検出しようとしています。 可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9e84e-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="9e84e-210">例:EWS マネージ API を使用して、ページング検索を実行する</span><span class="sxs-lookup"><span data-stu-id="9e84e-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="9e84e-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="9e84e-211"></span></span>

<span data-ttu-id="9e84e-212">ページングは、次の EWS マネージ API メソッドによってサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9e84e-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="9e84e-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="9e84e-213">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="9e84e-214">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="9e84e-215">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="9e84e-216">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="9e84e-217">EWS のマネージ API を使用する場合、アプリケーションが[ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx)または[FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx)クラスでページングを構成し、サーバーから情報を受け取り、 [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx)または[FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx)からのページングに関連クラスです。</span><span class="sxs-lookup"><span data-stu-id="9e84e-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="9e84e-p117">次の例では、各応答で 5 アイテムを返すページング検索を使用してフォルダー内のすべてのアイテムを取得します。さらに、サーバー上の結果の変更を検出するためにアンカーとして機能する追加のアイテムを取得します。 </span><span class="sxs-lookup"><span data-stu-id="9e84e-p117">The following example retrieves all the items in a folder using a paged search that returns five items in each response. It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="9e84e-220">次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。</span><span class="sxs-lookup"><span data-stu-id="9e84e-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems &amp;&amp; anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
            anchorId = results.Items.Last<Item>().Id;
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="9e84e-221">例:EWS を使用して、ページング検索を実行する</span><span class="sxs-lookup"><span data-stu-id="9e84e-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="9e84e-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="9e84e-222"></span></span>

<span data-ttu-id="9e84e-223">ページングは、次の EWS 操作によってサポートされています。</span><span class="sxs-lookup"><span data-stu-id="9e84e-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="9e84e-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="9e84e-224">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="9e84e-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="9e84e-225">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="9e84e-226">EWS を使用する場合、アプリケーションは[IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要素または[IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)要素を使って、ページングを構成し、サーバーから情報を受信して (の[からのページングに関連FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) [(FindFolderResponseMessage) をして](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)要素または要素。</span><span class="sxs-lookup"><span data-stu-id="9e84e-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="9e84e-227">この要求の例では、ユーザーの受信トレイ内のアイテムの一覧の先頭からゼロのオフセットから始まる、6 つの項目の最大の**FindItem**要求が送信されます。</span><span class="sxs-lookup"><span data-stu-id="9e84e-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9e84e-p118">サーバーは、6 アイテムを含む次の応答を返します。さらに応答は、サーバー上の結果にアイテムが合計 8 あり、結果リストの最後のアイテムがこの応答には存在しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p118">The server returns the following response, which contains six items. The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="9e84e-230">この例では、同じ要求を送信すると、ですが、今回は、**オフセット**属性は 5 で、サーバーが最大で 5 先頭からのオフセットから始まる 6 つの項目を返す必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9e84e-p119">サーバーは、3 アイテムを含む次の応答を送信します。応答は、サーバー上の結果の合計アイテム数が 8 のままで、結果リストの最後のアイテムがこの応答に含まれていることも示します。</span><span class="sxs-lookup"><span data-stu-id="9e84e-p119">The server sends the following response, which contains three items. The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="9e84e-233">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e84e-233">See also</span></span>


- [<span data-ttu-id="9e84e-234">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="9e84e-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="9e84e-235">ExchangeService.FindFolders メソッド</span><span class="sxs-lookup"><span data-stu-id="9e84e-235">ExchangeService.FindFolders method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-236">ExchangeService.FindItems メソッド</span><span class="sxs-lookup"><span data-stu-id="9e84e-236">ExchangeService.FindItems method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-237">Folder.FindFolders メソッド</span><span class="sxs-lookup"><span data-stu-id="9e84e-237">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="9e84e-238">Folder.FindFolders メソッド</span><span class="sxs-lookup"><span data-stu-id="9e84e-238">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- <span data-ttu-id="9e84e-239">
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="9e84e-239">[FindFolder operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)</span></span>
    
- <span data-ttu-id="9e84e-240">
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="9e84e-240">[FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)</span></span>
    
- [<span data-ttu-id="9e84e-241">EWS の交換で調整</span><span class="sxs-lookup"><span data-stu-id="9e84e-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

