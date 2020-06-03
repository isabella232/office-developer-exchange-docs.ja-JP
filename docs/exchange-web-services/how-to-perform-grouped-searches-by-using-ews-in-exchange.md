---
title: Exchange で EWS を使用して、グループ化された検索を実行する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527932"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、グループ化された検索を実行する

EWS マネージ API または Exchange を対象とする EWS アプリケーションで、グループ化された検索を実行する方法を説明します。
  
グループ化された検索は、検索結果を整理する方法を管理できるという点が便利です。検索結果を整理することにより、管理可能な方法で、アプリケーションが結果を処理したり結果をエンド ユーザーに表示したりすることが簡単にできるようになります。
  
特定のフィールドの同じ値を持つ結果セット内のすべてのアイテムをグループに配置してグループ化します。たとえば、送信者ごとに結果をグループ化でき、同じ人のすべてのアイテムは別のグループに入れられ、各グループ内のアイテムはビューで指定した順序に従って並べ替えられます。グループ自体は、選択したフィールドに基づく集約値で並べ替えられます。
  
**表 1. 検索結果を整理するための EWS マネージ API のメソッドと EWS 操作**

|**目的…**|**EWS マネージ API で使用するもの**|**EWS で使用するもの**|
|:-----|:-----|:-----|
|結果内の特定のプロパティが同じ値のアイテムをグループに分類する  <br/> |[Grouping.GroupOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |[GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) 要素の子としての [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 要素  <br/> |
|特定のプロパティの値によって各グループ内でアイテムを並べ替える  <br/> |[ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) 要素  <br/> |
|グループを並べ替える  <br/> |[Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |[AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) 要素の子としての **FieldURI** 要素<br/><br/> **AggregateOn** 要素の **Aggregate** 属性<br/><br/>**GroupBy** 要素の **Order** 属性  <br/> |
   
それぞれ順を追って説明します。
  
## <a name="group-results-by-a-specific-property"></a>特定のプロパティによる結果のグループ化
<a name="bk_GroupResults"> </a>

グループ化を使用する最初の手順は、グループ化するための、Exchange ストア内のアイテムのプロパティまたは属性を選択することです。 EWS マネージ API はこれらを対応するクラスのクラス プロパティとして公開するのに対し、EWS は XML 要素として公開します。 カスタム プロパティまたは拡張プロパティなど、任意のプロパティを選択することができますが、選択するプロパティの値に基づいてアイテムがグループ化される方法について理解しておくと役に立ちます。 

グループ化するために選択されたプロパティに同じ値を持つすべてのアイテムは、グループにまとめられます。 これは当然のことのようですが、重要な点です。 EWS マネージ API の [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx)、または EWS の [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) 要素など、日付/時刻プロパティでグループ化するとどうなるかを考えてみましょう。 それぞれ同じ日のアイテムを含むグループになるよう、結果をグループ分けする場合があります。 ただし、グループ化では値全体が対象になります。これには時間が含まれます。 

最終的には、同時に (秒単位で正確に) 受け取られたアイテムが独自のグループに入るようにグループ化されます。 ほとんどの場合、各グループでアイテムの数が少ない多数のグループに並べ替えられることになります。 
  
グループの数が少なくかつ各グループでアイテムの数が多い結果セットを取得するには、値の数が少ない可能性の高いプロパティ (EWS マネージ API の [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) または [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx)、または EWS の [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) または [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) など) を選択します。 次の図は、受信トレイ内に表示されるメールの一覧を示します。 
  
**図 1. 受信トレイ内のメッセージ**

![ユーザーの [受信トレイ] のメッセージのサンプル リスト。](media/Ex15_GroupedSearch_MsgList.png)
  
**EmailMessage.From** プロパティで図 1 のアイテムをグループ化すると、2 つのグループに分けられます。1 つは Hope Gross から送信されたメッセージで、もう 1 つは Sadie Daniels から送信されたメッセージです。 
  
**図 2. From プロパティに基づいてグループ分けされたメッセージ**

![From プロパティで 2 つのリストに分類されたメッセージを表示したイメージ。](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a>グループ内でアイテムを並べ替える
<a name="bk_SortItems"> </a>

EWS マネージ API の [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) プロパティ、または EWS の [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) 要素を使用して、各グループ内でアイテムを並べ替える方法を制御することができます。 同じ順序を各グループに適用します。 たとえば、**Item.DateTimeReceived** プロパティで図 1 のアイテムを降順に並べ替えると、Hope Gross から受信した最新のアイテムが Hope Gross グループの一番上になります。また、Sadie Daniels から受信した最新のアイテムは Sadie Daniels グループの一番上になります。 便利なことに、図 2 のグループは既にこの方法で並べ替えられています。 
  
## <a name="sort-the-groups"></a>グループを並べ替える
<a name="bk_SortGroups"> </a>

これでグループが確定したので、最後の手順でグループ自体を並べ替えます。 グループ自体に特定の値がないため、グループ化のプロセスでグループごとに並べ替えの値を割り当てる必要があります。 これを行うには、EWS マネージ API の [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) プロパティ、または EWS の [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) 要素の子としての [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 要素で指定して、各グループ内で特定のプロパティの値を集約します。 EWS マネージ API の [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) プロパティ (または EWS の **AggregateOn** 要素の **Aggregate** 属性) は、グループの並べ替え対象の値 (最大値または最小値のいずれか) として割り当てる各グループ内のアイテムの値を指定します。 最後に、並べ替えの順序 (降順または昇順) を、EWS マネージ API の [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) プロパティまたは EWS の [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) 要素の **Order** 属性で指定します。 
  
たとえば、図 2 のグループを **Item.DateTimeReceived** プロパティで集約し、最小値を使用して降順で並べ替えると、アイテムは図 3 に示す順序で返されます。 
  
**図 3. DateTimeReceived プロパティによって並べ替えられたグループでのグループ化された検索結果**

![From プロパティでグループ化された、並べ替えられたメッセージのリストを表示しているイメージ。グループは最小の受信日時で並び替えられています。](media/Ex15_GroupedSearch_Results.png)
  
次のセクションでは、コードでグループ化と並べ替えをまとめてプルする方法を説明します。
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a>例: EWS マネージ API を使用して、グループ化された検索を実行する
<a name="bk_GroupSearchEWSMA"> </a>

次の EWS マネージ API メソッドではグループ化を使用できます。
  
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
次の例では **ExchangeService.FindItems** メソッドを使用しますが、同じルールと概念が **Folder.FindItems** メソッドにも適用されます。 この例では、**GroupItemsByFrom** と呼ばれるメソッドが定義されます。 パラメーターとして、[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトと [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクトを使用します。 **EmailMessage.From** プロパティでグループ化し **Item.DateTimeReceived** プロパティで降順に並べ替えた、フォルダー内の最初の 50 アイテムを要求します。 グループ自体は、グループのアイテムの **Item.DateTimeReceived** プロパティの最小値によって降順で並べ替えられます。 
  
この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 
  
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

## <a name="example-perform-a-grouped-search-by-using-ews"></a>例: EWS を使用して、グループ化された検索を実行する
<a name="bk_GroupSearchEWS"> </a>

次の要求例では、**From** 要素でグループ化し **DateTimeReceived** 要素で降順に並べ替えた、フォルダー内の最初の 50 アイテムに対する [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)要求を示します。 グループ自体は、グループのアイテムの **DateTimeReceived** 要素の最小値によって降順で並べ替えられます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

メジャー バージョン 15 以降のビルド 15.0.775.38 以前のバージョンの Exchange では、SOAP 応答で [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) 要素の代わりに **Group** 要素 (型 **GroupedItemsType**) が返されます。 EWS マネージ API を使用している場合、これは [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) コレクションに含まれるオブジェクトが 0 になる原因になります。 EWS を使用している場合は、**Group** 要素は **GroupedItems** 要素として処理される必要があります。 
  
メジャー バージョン 15 以降のバージョンの Exchange では、SOAP 応答で **true** に設定された **xsi:nil** 属性を持つ追加の **Group** 要素または **GroupedItems** 要素が返されます。 EWS マネージ API を使用している場合、これらの追加の要素は [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) がスローされる原因となります。 EWS を使用している場合は、これらの余分な要素は無視します。 
  
## <a name="see-also"></a>関連項目

- [Exchange の検索と EWS](search-and-ews-in-exchange.md)    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [クラスのグループ化](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [FindItem 操作](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

