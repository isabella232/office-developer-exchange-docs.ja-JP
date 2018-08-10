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
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Exchange で EWS を使用して AQS 検索を実行する

EWS マネージ API または EWS アプリケーションで、クエリ文字列および AQS を使用して検索する方法を確認します。
  
クエリ文字列は、検索条件を表現する[検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)に代わる方法を提供します。 クエリ文字列を使用する最大の利点は、検索するプロパティを 1 つも指定する必要がないということです。 値を指定するだけで、アイテム上の一般的に使用されるすべてのフィールドに検索が適用されます。 単純な値の代わりに高度な検索テクニック (AQS) を使用して検索を絞り込むこともできます。 ただし、クエリ文字列には、ツールボックスに追加する前に注意すべき次の制限があります。 
  
- **特定のプロパティを検索する機能に制限がある。** クエリ文字列で単純な値を検索すると、検索はすべてのインデックス付きプロパティに対して実行されます。 特定のプロパティに検索を絞り込むことはできますが、AQS 文字列で使用できるプロパティは限定されます。 検索するプロパティが AQS で使用可能なプロパティのいずれでもない場合は、検索フィルターを使用することを検討してください。 
    
- **カスタム プロパティは検索されない。** クエリ文字列の検索はインデックスに対して実行されますが、カスタム プロパティはそのインデックスに含まれません。 カスタム プロパティを検索する必要がある場合は、代わりに検索フィルターを使用してください。 
    
- **文字列検索の制御が限定されている。** クエリ文字列の検索は常に、大文字と小文字の違いを無視し、部分文字列の検索になります。 大文字と小文字を区別する場合、プレフィックスの検索、完全一致の検索を実行する場合は、検索フィルターを使用してください。 
    
- **フォルダーまたは検索フォルダーでは使用できない。** フォルダーを検索するための EWS 操作では、クエリ文字列の使用がサポートされていません。 さらに、検索フォルダーは、クエリ文字列をサポートしません。 どちらの場合も、検索フィルターが唯一のオプションになります。 
    
## <a name="creating-a-query-string"></a>クエリ文字列の作成
<a name="bk_CreateQueryString"> </a>

EWS マネージ API および EWS のクエリ文字列は、AQS 構文の一部であると解釈されます。AQS 文字列は、値またはキーワード/値のペアのいずれかで構成され、コロン (:) で区切られます。
  
`keyword:value`

キーワードを使用せずに値を指定した場合、すべてのインデックス付きプロパティでその値が検索されます。キーワードが値とペアになっている場合、キーワードは対応する値を検索するプロパティを指定します。
  
**表 1. サポートされている AQS キーワード**

|**キーワード**|**値の型**|**例**|
|:-----|:-----|:-----|
|subject  <br/> |文字列  <br/> |subject:project  <br/> |
|body  <br/> |文字列  <br/> |body:sales figures  <br/> |
|attachment  <br/> |文字列  <br/> |attachment:report  <br/> |
|to  <br/> |文字列  <br/> |to:"Sadie Daniels"  <br/> |
|from  <br/> |文字列  <br/> |from:hope  <br/> |
|cc  <br/> |文字列  <br/> |cc:"Ronnie Sturgis"  <br/> |
|bcc  <br/> |文字列  <br/> |bcc:mack  <br/> |
|participants  <br/> |文字列  <br/> |participants:sadie  <br/> |
|category  <br/> |文字列  <br/> |category:project  <br/> |
|importance  <br/> |文字列  <br/> |importance:high  <br/> |
|kind  <br/> |アイテムの種類  <br/> |kind:meetings  <br/> |
|sent  <br/> |日付  <br/> |sent:12/10/2013  <br/> |
|received  <br/> |日付  <br/> |received:yesterday  <br/> |
|hasattachment  <br/> |ブール型  <br/> |Has attachment:true  <br/> |
|isflagged  <br/> |ブール型  <br/> |isflagged:true  <br/> |
|isread  <br/> |ブール型  <br/> |isread:false  <br/> |
|size  <br/> |数値  <br/> |size:\>5000  <br/> |
   
別の値の型がどのように動作するかを見てみましょう。
  
### <a name="using-a-string-value-type"></a>文字列値型の使用

文字列値型は既定で、大文字と小文字を区別しないプレフィックス部分文字列として検索されます。 つまり、subject:project を検索すると、次の項目のいずれかと一致します。 
  
- Project meeting notes
    
- Do you have the project plans?
    
- December sales projections
    
文字列を引用符で囲むことによってプレフィックスと一致させるのではなく、完全に一致する単語を要求するように検索を変更できます。 subject:"project" を検索すると、候補一覧から「December sales projections」値が削除されます。 この場合でも、値は大文字と小文字が区別されないことに注意してください。 
  
クエリ文字列に複数の単語を使用する場合、両方の単語が検索対象フィールドにあるものが一致します。 たとえば、subject:project plan を検索すると、次の項目のいずれかと一致します。 
  
- Project plan
    
- Do you have the project plans?
    
- Please send me the plan for our project
    
- Planning project milestones
    
複数の単語を引用符で囲むと、それらは 1 つの句として扱われます。 subject:"project plan" を検索すると、先ほどのリストの「Project plan」という件名だけが一致します。 
  
### <a name="using-an-item-type-value-type"></a>アイテムの種類の値の型の使用

**kind** キーワードで次のアイテムの種類の値を使用して、検索結果をメールや会議出席依頼などの特定の種類のアイテムのみに制限することができます。 
  
- 連絡先    
- docs    
- email    
- faxes    
- im (インスタント メッセージに相当)    
- journals    
- meetings (予定や会議出席依頼に相当)    
- notes    
- posts    
- rssfeeds    
- tasks    
- voicemail
    
### <a name="using-a-date-value-type"></a>日付値型の使用

日付値型はいくつかの異なる方法で検索できます。 最も単純なのは特定の日付を検索することです。 received:12/11/2013 で検索すると、2013 年 12 月 11 日に受信したすべてのアイテムが返されます。 ただし、指定の仕方を簡単な形式にすることもできます。 received:12/11 で検索すると、現在の年の 12 月 11 日に受信したすべてのアイテムが返されます。 
  
別のオプションとして、月の名前を使用することができます。 received:December 11, 2013 または December 11 で検索すると、received:12/11/2013 および received:12/11 と同じ結果を取得できます。 received:December で検索し、現在の年の 12 月に受信したすべてのアイテムを取得することもできます。 
  
週の曜日の名前を使用することもできます。 received:Tuesday で検索すると、現在の週の火曜日に受信したすべてのアイテムが返されます。 
  
日付値型は、現在の時刻を基準にした検索のキーワードのセットもサポートします。サポートされているキーワードは次のとおりです。
  
- 今日  
- tomorrow
- yesterday
- this week    
- last week    
- next month    
- past month    
- coming year
    
日付値型は、greater than または less than のような関係演算子で比較したり、範囲演算子 **..** を使用して範囲として指定したりすることもできます。たとえば、received:\>11/30/2013, sent:\>=yesterday、received:12/1/2013..today はすべて、有効なクエリ文字列です。 
  
### <a name="using-a-boolean-value-type"></a>ブール値型の使用

ブール値型は "true" または "false" にできます。 値は大文字と小文字を区別しないので、isread:false と isread:FALSE で生成される結果は同じです。
  
### <a name="using-a-number-value-type"></a>数値型の使用

数値型は、完全一致として検索できますが、greater than または less than のような関係演算子を使用して検索することもできます。 たとえば、size:10000 では、正確に 10000 バイトのサイズを持つアイテムのみが返されますが、size:\>=10000 では 10000 バイト以上のサイズを持つアイテムが返されます。 範囲演算子 (**..**) を使用して範囲を指定することもできます。 たとえば、size:7000..8000 ではサイズが 7000 と 8000 の間のアイテムが返されます。 
  
### <a name="using-logical-operators"></a>論理演算子の使用

クエリ文字列は、次の論理演算子をサポートします。
  
**表 2. サポートされる論理演算子**

|**演算子**|**例**|
|:-----|:-----|
|AND  <br/> |project AND from:"Sadie Daniels"  <br/> subject:(project AND plan)  <br/> |
|OR  <br/> |subject:meeting OR from:"Hope Gross"  <br/> from:("Sadie Daniels" OR "Hope Gross")  <br/> |
|NOT  <br/> |NOT from:"Ronnie Sturgis"  <br/> received:NOT today  <br/> |
   
これらの演算子を使用して、複数の条件を結合したり、1 つのキーワード/値のペア内で複数の値を結合したりできることに注意してください。 ただし、1 つのキーワード/値ペアで複数の値を結合する場合は、かっこを使用して複数の値を囲む必要があります。 その理由を理解するために、from:"Sadie Daniels" OR "Hope Gross" で検索してみてください。 この検索は、実際には次の条件として解釈されます。
  
- アイテムが Sadie Daniels からのもの、または
    
- アイテムのインデックス付きプロパティのいずれかに「Hope Gross」という語句がある。
    
対照的に、from:("Sadie Daniels" OR "Hope Gross") は次のように解釈されます。 
  
- アイテムが Sadie Daniels からのもの、または
    
- アイテムが Hope Gross からのもの
    
複数の条件が指定されているものの論理演算子は含まれていない場合の既定の演算子は AND です。 たとえば、has attachment:true subject:project は has:attachment:true AND subject:project と同じです。
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>例: クエリ文字列と EWS マネージ API を使用してアイテムを検索する
<a name="bk_ExampleEWSMA"> </a>

この例では、**SearchWithQueryString** というメソッドが定義されています。 パラメーターとして、[ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、[WellKnownFolderName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) オブジェクト、クエリ文字列を表す **string** オブジェクトを取ります。 この例では、**ExchangeService** オブジェクトは [Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。 
  
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

このメソッドを使用して、この例のように、件名に「project plan」という語句が含まれるすべてのアイテムを検索することができます。
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>例: クエリ文字列と EWS を使用してアイテムを検索する
<a name="bk_ExampleEWS"> </a>

この例では、SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要求で、件名に「project plan」という語句が含まれる受信トレイ内のすべてのアイテムを検索します。 
  
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

次の例は、検索結果を含むサーバーからの応答を示しています。
  
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

## <a name="see-also"></a>関連項目

- [Exchange の検索と EWS](search-and-ews-in-exchange.md)    
- [Exchange で EWS とともに検索フィルターを使用する](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

