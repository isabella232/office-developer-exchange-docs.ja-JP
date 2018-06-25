---
title: EWS を使用して Exchange によってグループ化された検索を実行します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。
ms.openlocfilehash: 63a796e2c724351c15287a5596a9a063954f8b40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759035"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a>EWS を使用して Exchange によってグループ化された検索を実行します。

EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。
  
グループ化された検索は、検索結果を整理する方法を管理できるという点が便利です。検索結果を整理することにより、管理可能な方法で、アプリケーションが結果を処理したり結果をエンド ユーザーに表示したりすることが簡単にできるようになります。
  
特定のフィールドの同じ値を持つ結果セット内のすべてのアイテムをグループに配置してグループ化します。たとえば、送信者ごとに結果をグループ化でき、同じ人のすべてのアイテムは別のグループに入れられ、各グループ内のアイテムはビューで指定した順序に従って並べ替えられます。グループ自体は、選択したフィールドに基づく集約値で並べ替えられます。
  
**表 1 です。EWS のマネージ API のメソッドおよび検索結果を整理するための EWS の操作**

|**目的…**|**EWS のマネージ API で次のコマンドを使用してください.**|**EWS で次のコマンドを使用してください.**|
|:-----|:-----|:-----|
|結果内の特定のプロパティが同じ値のアイテムをグループに分類する  <br/> |[Grouping.GroupOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) [GroupBy](http://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)要素の子要素  <br/> |
|特定のプロパティの値によって各グループ内でアイテムを並べ替える  <br/> |[ItemView.OrderBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |[SortOrder](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx)要素  <br/> |
|グループを並べ替える  <br/> |[Grouping.AggregateOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [Grouping.AggregateType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [Grouping.SortDirection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |**FieldURI**要素は、 [AggregateOn](http://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)要素の子要素として<br/><br/> **AggregateOn**要素の属性を**集計**<br/><br/>**GroupBy**要素の属性を**注文**  <br/> |
   
それぞれ順を追って説明します。
  
## <a name="group-results-by-a-specific-property"></a>特定のプロパティによる結果のグループ化
<a name="bk_GroupResults"> </a>

プロパティを選択するか、属性のグループ化] を Exchange ストア内のアイテムをグループ化を使用する最初の手順では。 EWS のマネージ API は、EWS を XML 要素として公開するときに、対応するクラスで、クラスのプロパティとして公開されています。 カスタムまたは拡張のプロパティを含め、任意のプロパティを選択することができますが、項目がグループ化方法を選択するプロパティの値に基づいてを理解するおくと便利です。 

別にグループ化するプロパティに同じ値を持つすべての項目グループにまとめられます。 当たり前のことがありますが、重要なの詳細情報です。 考慮 EWS のマネージ API では、 [Item.DateTimeReceived](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx)または EWS の[DateTimeReceived](http://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx)要素など、日付/時刻プロパティでグループ化するかどうか。 同じ日からの項目を格納している各グループに、グループに、結果を整理するために意図があります。 ただし、グループ化は、時間が含まれます、全体の値を表示します。 

最終的には独自のグループ、2 番目に、同時に受信したアイテムになるよう、アイテムをグループ化にすることです。 結果は、ほとんどの場合多数の各グループ内の項目の数が少ないグループに並べ替えられます。 
  
結果セットのグループの数を減らして、各グループ内の項目の多くを取得するには、 [EmailMessage.From](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx)または EWS マネージ API では、または[から](http://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx)の[Item.Categories](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx)などの値の数を少なくする可能性があるプロパティを選択します。または EWS で[カテゴリ](http://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx)を選択します。 次の図は、受信トレイ内に表示される電子メールの一覧を示します。 
  
**図 1 です。受信トレイ内のメッセージ**

![ユーザーの [受信トレイ] のメッセージのサンプル リスト](media/Ex15_GroupedSearch_MsgList.png)
  
**EmailMessage.From**プロパティでは、図 1 内のアイテムをグループ化する場合、結果になります期待しての総額によって送信されたメッセージと Sadie Daniels から送信されたメッセージの 2 つのグループです。 
  
**図 2 になります。メッセージの From プロパティに基づいてグループ分け**

![From プロパティで 2 つのリストに分類されたメッセージを表示したイメージ。](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a>グループ内でアイテムを並べ替える
<a name="bk_SortItems"> </a>

EWS のマネージ API では、 [ItemView.OrderBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx)プロパティまたは EWS での[並べ替え順序](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx)の要素を使用して、「各グループ内の項目の並べ替え方法を制御することができます。 同じ順序は、各グループに適用されます。 などの降順の順序で、 **Item.DateTimeReceived**プロパティでは、図 1 からのアイテムを並べ替える場合を期待して総額から最後に受信された項目は期待粗グループで最初になり Sadie Daniels から最近受信したアイテムになりますSadie Daniels のグループの最初の。 便利なことに、図 2 のグループはこの方法で、ソートされます。 
  
## <a name="sort-the-groups"></a>グループを並べ替える
<a name="bk_SortGroups"> </a>

決済のグループがある場合は、これで最後の手順は、グループ全体を並べ替えます。 グループ自体が特定の値を持たないためグループ化プロセスはグループごとに並べ替え値を割り当てるには。 これは、EWS の[AggregateOn](http://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)要素の子として、EWS のマネージ API で、または[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx)要素の[Grouping.AggregateOn](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx)プロパティで指定された各グループ内の特定のプロパティの値の集計を実行します。 EWS のマネージ API (または、EWS の**AggregateOn**要素の属性が**集計**) で[Grouping.AggregateType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx)プロパティの指定グループの並べ替え値を各グループ内のアイテムの値が割り当てられている、いずれか、最大値または最小値。 最後に、並べ替えの順序 (降順または昇順) は、EWS のマネージ API で、または EWS に[GroupBy](http://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)要素の**順序**属性の[Grouping.SortDirection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx)プロパティによって指定されます。 
  
たとえば、図 2 からのグループを並べ替える場合は、 **Item.DateTimeReceived**プロパティを集約することにより、最小の値を使用して、降順で並べ替え項目が返されますに示すように図 3 の順序で。 
  
**図 3 です。DateTimeReceived プロパティによって並べ替えられたグループにグループ化された検索結果**

![From プロパティでグループ化された、並べ替えられたメッセージのリストを表示しているイメージ。グループは最小の受信日時で並び替えられています。](media/Ex15_GroupedSearch_Results.png)
  
次のセクションでは、コードでグループ化と並べ替えをまとめてプルする方法を説明します。
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a>例:EWS マネージ API を使用して、グループ化された検索を実行する
<a name="bk_GroupSearchEWSMA"> </a>

次の EWS マネージ API メソッドではグループ化を使用できます。
  
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
**ExchangeService.FindItems**メソッドを使用して、次の使用例ただし、同じ規則や概念は、 **Folder.FindItems**メソッドに適用されます。 この例では、 **GroupItemsByFrom**と呼ばれるメソッドを定義します。 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと[WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)オブジェクトはパラメーターとして受け取ります。 **EmailMessage.From**プロパティは、 **Item.DateTimeReceived**プロパティの順序を降順で並べ替え、グループ化、フォルダー内の最初の 50 のアイテムを要求します。 グループ自体は、降順で、その項目の最小の**Item.DateTimeReceived**プロパティの値に基づいて並べ替えられます。 
  
次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a>例:EWS を使用して、グループ化された検索を実行する
<a name="bk_GroupSearchEWS"> </a>

要求の例を次は、フォルダー**から**要素を**DateTimeReceived**の要素の順序を降順で並べ替え、グループ化された[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)要求の最初の 50 の項目を示しています。 最小**DateTimeReceived**要素の値の降順に並べ替え、アイテムの上では、グループ全体が並べ替えられます。 
  
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
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
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

サーバーは次の応答を返します。
  
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
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a>バージョンの相違点
<a name="bk_VersionDiffs"> </a>

15 のメジャー バージョンとで開始および終了ビルド 15.0.775.38 戻り値要素を**グループ化**(型**GroupedItemsType**) の[GroupedItems](http://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx)要素の代わりに、SOAP 応答での Exchange のバージョンです。 EWS のマネージ API を使用する場合は、0 のオブジェクトを格納する[GroupedFindItemsResults.ItemGroups](http://msdn.microsoft.com/en-us/library/office/dd633961%28v=exchg.80%29.aspx)コレクションなります。 EWS を使用する場合は、 **GroupedItems**の要素として要素を**グループ化**を処理する必要があります。 
  
15 のメジャー バージョンの Exchange のバージョンでは、 **xsi:nil**属性が**true**では、SOAP 応答に設定を**グループ**または**GroupedItems**の余分な要素を返します。 EWS のマネージ API を使用する場合、これらの余分な要素には、 [ServiceXmlDeserializationException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx)がスローされますが発生します。 EWS を使用する場合は、これらの余分な要素は無視されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の検索と EWS](search-and-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [クラスをグループ化](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- 
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

