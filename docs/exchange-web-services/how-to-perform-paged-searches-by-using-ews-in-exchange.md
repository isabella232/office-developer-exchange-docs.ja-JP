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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759038"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Exchange EWS を使用してページ検索を実行します。

Exchange を対象とする EWS マネージ API または EWS のアプリケーションでページングされた検索を実行する方法を説明します。
  
ページングは、検索結果のサイズを制御するための EWS の機能です。1 度の EWS の応答で検索セット全体を取得する代わりに、複数の EWS 応答で小さなセットに分けて取得できます。たとえば、受信トレイに 10,000 件のメール メッセージがあるユーザーについて検討します。仮に、10,000 件のメールすべてを 1 度の大規模な応答で取得できる場合でも、帯域幅またはパフォーマンス上の理由でより管理しやすいチャンクに分割することを望まれるかもしれません。ページングは、そうするのに最適なツールを提供します。
  
> [!NOTE]
> 実際に要求が 1 つで 10,000 個のアイテムを取得することができますと仮定、EWS の調整のため可能性がありますこれはありません。 詳細については、 [EWS が Exchange で調整](ews-throttling-in-exchange.md)を参照してください。 
  
**表 1 です。EWS のマネージ API および EWS でのページングのパラメーター**

|**設定または取得する、.**|**EWS のマネージ API で次のコマンドを使用してください.**|**EWS で次のコマンドを使用してください.**|
|:-----|:-----|:-----|
|応答中のアイテムまたはフォルダーの最大数  <br/> |**PageSize**パラメーター [ItemView のコンス トラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx)または[FolderView コンス トラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Or  <br/> [PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)プロパティ  <br/> |[IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要素または[IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)要素の**MaxEntriesReturned**属性  <br/> |
|アイテムまたはフォルダーのリストの開始点  <br/> |**OffsetBasePoint** **ItemView**コンス トラクターまたは**FolderView**コンス トラクターのパラメーター  <br/> Or  <br/> [PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)プロパティ  <br/> |**IndexedPageItemView**要素または**IndexedPageFolderView**要素の**ベース ポイント**属性  <br/> |
|開始点からのオフセット  <br/> |**ItemView**コンス トラクターまたは**FolderView**コンス トラクターに**offset**パラメーター  <br/> Or  <br/> [PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)プロパティ  <br/> |**オフセット**属性は、 **IndexedPageItemView**要素または**IndexedPageFolderView**要素の  <br/> |
|サーバー上の結果の総数  <br/> |[FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)プロパティ  <br/> |[RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx)の要素に[して (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)の要素の**TotalItemsInView**属性  <br/> |
|現在の応答に含まれない次のアイテムまたはフォルダーのオフセット  <br/> |[FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)プロパティ  <br/> |**RootFolder**要素の**IndexedPagingOffset**属性  <br/> |
|応答が最後のアイテムまたはフォルダーをリストに含んでいるかどうかを示すインジケーター  <br/> |[FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx)プロパティまたは[FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)プロパティ  <br/> |**RootFolder**要素の**IncludesLastItemInRange**属性  <br/> |
   
## <a name="how-paging-works"></a>ページングのしくみ
<a name="bk_HowPagingWorks"> </a>

ページングのしくみを理解するには、フォルダー内のメッセージを屋外に並べられた広告版に置き換えて考えると分かりやすくなります。これらの広告版のいくつかを魔法のウィンドウを通して見ることができます。ウィンドウのサイズを変更 (同時に表示する広告版の数を増やすまたは減らすため) したり、ウィンドウを移動 (表示する広告版を制御するため) したりできます。このウィンドウの操作がページングです。  
  
要求を Exchange サーバーに送信する際、返すアイテム数を指定するためにウィンドウのサイズを指定します。開始点 (行の先頭または末尾) とその開始点からのオフセット (アイテム数で表す) を指定して、ウィンドウの位置を設定します。ウィンドウの先頭は、開始点からのオフセットで指定されたアイテムの数です。
  
ページングの魅力は、サーバーの応答と、その応答をアプリケーションで使用して次の要求を形成する際に発揮されます。次の要求に備えて "ウィンドウ" を構成する方法を決定するのに使用できる次の 3 つの情報がサーバーから提供されます。  
  
- 応答に含まれている結果に、サーバー上の結果セット全体の最後のアイテムが含まれているかどうか。
    
- サーバー上の結果セットのアイテムの合計数。
    
- 現在の応答に含まれていない、結果セット内の次のアイテムにウィンドウを移動する場合に指定すべきオフセットの値。
    
簡単な例を見てみましょう。受信トレイに 15 件のメッセージがあるとします。アプリケーションによって、メッセージのリストの初めから最大 10 個のアイテム (オフセットは 0 になります) を取得するための最初の要求が送信されます。サーバーからの応答には最初の 10 件のメッセージが含まれ、応答には最後のアイテムが含まれておらず、合計 15 個のアイテムがあり、次のオフセットを 10 にする必要があることが示されます。
  
**図 1 です。15 項目の一覧の先頭からオフセット 0 から 10 個のアイテムを要求します。**

![15 アイテムのリストの初めからオフセット 0 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_FirstPage.png)
  
次にアプリケーションは、同じ要求をサーバーに再送信します。変更されたのはオフセットが 10 になったという点だけです。サーバーは、最後の 5 アイテムを返し、応答に最後のアイテムが含まれており、合計 15 個のアイテムがあり、次のオフセットを 15 にする必要があることが示されます (もちろん、末尾に達したため、次のオフセットはありません)。
  
**図 2 になります。15 項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**

![15 アイテムのリストの初めからオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>ページングのデザイン上の考慮事項
<a name="bk_DesignConsiderations"> </a>

アプリケーションでページングを最大限活用するには、考慮すべき事項があります。たとえば、"ウィンドウ" のサイズをどのように決めるか、"ウィンドウ" の移動中にサーバ上の結果を変更された場合にどうするかなどです。
  
### <a name="determine-the-size-of-your-window"></a>ウィンドウのサイズの決定

すべてのアプリケーションが使用するべき、あらゆる状況に適したエントリの最大数といったものはありません。アプリケーションにとって適切な数は、いくつかの異なる要素に基づいて決定されます。しかし、次のガイドラインに従うと便利です。
  
- 既定で、Exchange では 1 つの要求に返すことのできる最大アイテム数を 1000 に限定しています。
    
- エントリの最大数を大きい数字に設定すると、すべてのアイテムを取得するのに送信する要求の数は少なくなりますが、応答の待機時間が長くなります。
    
- エントリの最大数を小さい数に設定すると、応答時間が短くなりますが、すべてのアイテムを取得するのに送信する要求の数が増えます。
    
### <a name="handling-changes-to-the-result-set"></a>結果セットが変更された場合の処理

前述の例では、ユーザーの受信トレイ内のアイテム数が一定でした。ただし、実際には、受信トレイ内のアイテム数は頻繁に変更されることがあります。いつでも、新しいメッセージが到着したり、アイテムが削除または移動されることがあります。これは、どのようにページングに影響するでしょうか?前述の例のシナリオを変更して確認しましょう。
  
再度、ユーザーの受信トレイには 15 アイテムある設定で、同じ最初の要求を送信します。先の例同様、サーバーからの応答として最初の 10 件のメッセージが含まれ、応答に最後のアイテムが含まれておらず、合計 15 個のアイテムがあり、次のオフセットを 10 にする必要があることが示されます (図 1)。
  
アプリケーションでそれら 10 のアイテムが処理されている間、新しいメッセージが受信トレイに到着し、サーバーの結果セットに追加されます。アプリケーションが同じ要求をサーバーに再送信します (オフセットが 10 に設定されている)。今回の場合、サーバーは 6 アイテムを返し、合計 16 アイテムが結果セットにあることが示されます。
  
この時点で、これが問題かどうか認識できないかもしれません。結局のところ、2 つの応答を通して 16 アイテムが返されただけのことです。答えは、新しいアイテムがリストのどこに配置されたかによって異なります。最も古いアイテム (受信した日時順) が先頭に来るようにリストが並べ替えられている場合、このシナリオでは心配する要因となるものはありません。新しいアイテムはリストの末尾に配置され、2 番目の応答に含まれます。
  
**図 3 です。新しいされているリスト内の 16 の項目で 16 の項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**

![16 番目のアイテムがリストの終わりに追加されたときに、16 アイテムのリストの最初からオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
最新のアイテムが最初になるように、リストが並べ替えられている場合は、別の話です。この例では、2 番目の要求の最初のアイテムがその前の要求の最後のアイテムになり、残りの 5 アイテムは元の 15 アイテムのものです。仮想的な魔法のウィンドウという観点で考えると、ウィンドウの位置は 10 移動しましたが、広告版自体も 1 移動したことになります。
  
**図 4 です。新しいされているリストの最初の項目で 16 の項目の一覧の先頭からのオフセット 10 に 10 個のアイテムを要求します。**

![16 番目のアイテムがリストの初めに追加されたときに、16 アイテムのリストの最初からオフセット 10 で 10 アイテムを要求した結果を表示している図。](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
サーバー上の結果に加えられた変更を特定する 1 つの方法は、アンカー アイテムの概念を使用することです。アンカー アイテムは、結果の残りの部分と一緒には処理されない、応答に追加されたアイテムです。次の結果と比較して、アイテム自体が移動したかどうかを確認するために使用されます。先の簡単な例では、アプリケーションで "ウィンドウ" のサイズを 10 に設定している場合、実際には戻るアイテムの最大数を 11 に設定していることになります。アプリケーションでは、通常どおり、応答の最初の 10 アイテムを処理します。最後のアイテムについて、アイテムの識別子をアンカーとして保存してから、オフセットが 10 の次の要求を発行します。データが変更されていない場合、2 番目の応答の最初のアイテムにはアンカーと一致するアイテムの識別子があるはずです。アイテムの識別子が一致しない場合は、データが削除されたか、既にページングしたリストの特定の箇所に挿入されたことが分かります。
  
わかっている場合、データが変更されたことをする必要がありますに対処する方法を決定します。 か、この質問のニーズによって異なるものの応答がありません。 アクションは、アプリケーションとすべての項目を取得することが重要な方法の性質によって異なります。 完全無視して、先頭から処理を再開または、トラックをバックアップするか、および変更の発生場所を検出しようとしています。 可能性があります。
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>例:EWS マネージ API を使用して、ページング検索を実行する
<a name="bk_PagedSearchEWSMA"> </a>

ページングは、次の EWS マネージ API メソッドによってサポートされています。
  
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
EWS のマネージ API を使用する場合、アプリケーションが[ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx)または[FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx)クラスでページングを構成し、サーバーから情報を受け取り、 [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx)または[FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx)からのページングに関連クラスです。 
  
次の例では、各応答で 5 アイテムを返すページング検索を使用してフォルダー内のすべてのアイテムを取得します。さらに、サーバー上の結果の変更を検出するためにアンカーとして機能する追加のアイテムを取得します。  
  
次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>例:EWS を使用して、ページング検索を実行する
<a name="bk_PagedSearchEWS"> </a>

ページングは、次の EWS 操作によってサポートされています。
  
- [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
EWS を使用する場合、アプリケーションは[IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要素または[IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)要素を使って、ページングを構成し、サーバーから情報を受信して (の[からのページングに関連FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) [(FindFolderResponseMessage) をして](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)要素または要素。 
  
この要求の例では、ユーザーの受信トレイ内のアイテムの一覧の先頭からゼロのオフセットから始まる、6 つの項目の最大の**FindItem**要求が送信されます。 
  
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

サーバーは、6 アイテムを含む次の応答を返します。さらに応答は、サーバー上の結果にアイテムが合計 8 あり、結果リストの最後のアイテムがこの応答には存在しないことを示します。
  
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

この例では、同じ要求を送信すると、ですが、今回は、**オフセット**属性は 5 で、サーバーが最大で 5 先頭からのオフセットから始まる 6 つの項目を返す必要があることを示します。 
  
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

サーバーは、3 アイテムを含む次の応答を送信します。応答は、サーバー上の結果の合計アイテム数が 8 のままで、結果リストの最後のアイテムがこの応答に含まれていることも示します。
  
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

## <a name="see-also"></a>関連項目


- [Exchange の検索と EWS](search-and-ews-in-exchange.md)
    
- [ExchangeService.FindFolders メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders メソッド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- 
  [FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- 
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [EWS の交換で調整](ews-throttling-in-exchange.md)
    

