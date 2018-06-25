---
title: EWS を使用して Exchange、AQS 検索を実行します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: EWS マネージ API または EWS アプリケーションで、クエリ文字列および AQS を使用して検索する方法を確認します。
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759055"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>EWS を使用して Exchange、AQS 検索を実行します。

EWS マネージ API または EWS アプリケーションで、クエリ文字列および AQS を使用して検索する方法を確認します。
  
クエリ文字列は、検索条件を記述するため、[フィルター](how-to-use-search-filters-with-ews-in-exchange.md)の代わりに検索を提供します。 クエリ文字列を使用する最大の利点は、検索する 1 つのプロパティを指定する必要はありません。 値を提供できるだけで、検索は、一般的に使用されるすべてのフィールド項目に適用されます。 単純な値の代わりに高度なクエリ構文 (AQS) を使用して検索を絞り込むこともできます。 ただし、クエリ文字列には、注意すべきのコントロールをツールボックスに追加する前に次の制限があります。 
  
- **特定のプロパティを検索する機能に制限あり。** 単純なクエリ文字列の値を検索すると、すべてのインデックス付きプロパティに対して検索が実行されます。 特定のプロパティに検索を絞り込むことができますが、AQS 文字列で使用できるプロパティに限定されます。 プロパティを検索するには、AQS の使用可能なプロパティのいずれかがいない場合は、検索フィルターを使用することを検討してください。 
    
- **カスタム プロパティが検索されません。** インデックスにクエリ文字列の検索が実行され、カスタム プロパティは、そのインデックスには含まれません。 カスタム プロパティを検索する場合は、検索フィルターを使用してください。 
    
- **制限のコントロールの文字列を検索します。** クエリ文字列の検索は常に、大文字と小文字を無視し、部分文字列の検索は、常に。 大文字小文字を区別をする場合は、プレフィックス、または完全一致の検索は、検索フィルターを使用します。 
    
- **フォルダーまたは検索フォルダーは使用できません。** クエリ文字列を使用してフォルダーを検索するための EWS の操作がサポートされていません。 さらに、検索フォルダーには、クエリ文字列をサポートしません。 どちらの場合も、検索フィルターとは、唯一のオプションです。 
    
## <a name="creating-a-query-string"></a>クエリ文字列の作成
<a name="bk_CreateQueryString"> </a>

EWS マネージ API および EWS のクエリ文字列は、AQS 構文の一部であると解釈されます。AQS 文字列は、値またはキーワード/値のペアのいずれかで構成され、コロン (:) で区切られます。
  
`keyword:value`

キーワードを使用せずに値を指定した場合、すべてのインデックス付きプロパティでその値が検索されます。キーワードが値とペアになっている場合、キーワードは対応する値を検索するプロパティを指定します。
  
**表 1 です。AQS キーワードがサポートされています。**

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
|size  <br/> |数値  <br/> |サイズ:\>5000  <br/> |
   
別の値の型がどのように動作するかを見てみましょう。
  
### <a name="using-a-string-value-type"></a>文字列値型の使用

文字列値の型は、既定のプレフィックスの文字列が検索され、大文字小文字を区別するいないと検索では。 件名: プロジェクトの検索と一致する次の項目のいずれかのことを意味します。 
  
- Project meeting notes
    
- Do you have the project plans?
    
- December sales projections
    
引用符で囲まれた文字列を囲むことによって一致するプレフィックスではなく、単語全体を必要とする検索を変更します。 件名を検索する:「プロジェクト」が候補一覧から「12 月の売上予測」値を削除します。 値がまだない大文字小文字を区別に注意してください。 
  
クエリ文字列に複数の単語を使用する場合の一致では、両方の単語が検索フィールドに表示されている必要があります。 などの件名: プロジェクト計画の検索は一致する次の項目のいずれかの。 
  
- Project plan
    
- Do you have the project plans?
    
- Please send me the plan for our project
    
- Planning project milestones
    
複数の単語を引用符で囲むと、1 つの句として扱われます。 件名を検索する:「プロジェクト プラン」には、前のリストから「プロジェクト プラン」の対象が一致する、のみです。 
  
### <a name="using-an-item-type-value-type"></a>アイテムの種類の値の型の使用

電子メールや会議出席依頼などのアイテムの特定の種類のみに検索結果を制限するのに**ような**キーワードを使用して次の項目の種類の値を使用できます。 
  
- contacts    
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

いくつかの異なる方法で日付の値の型を検索できます。 最も単純な特定の日付を検索します。 検索を受信しました: 12/11/2013 は 2013 年 12 月 11 日に受信したすべての項目を返します。 ただし、特定性の低いことができます。 検索を受信しました: 12/11 は現在の年の 12 月 11 日に受信したすべての項目を返します。 
  
別のオプションでは、月の名前を使用します。 検索を行うことができますを受信しました: 2013 年 12 月 11 日または 12 月 11 日 ~ を受信すると、同じ結果を得る: 2013/12/11 および受信した: 12/11、それぞれ。 検索することもできます。 受信した: 現在の年の 12 月に受信したすべての項目を取得するには、年 12 月。 
  
週の曜日名を使用しては、また、オプションです。 受信で検索: 火曜日は現在の週の火曜日に受信したすべての項目を返します。 
  
日付値型は、現在の時刻を基準にした検索のキーワードのセットもサポートします。サポートされているキーワードは次のとおりです。
  
- today  
- tomorrow
- yesterday
- this week    
- last week    
- next month    
- past month    
- coming year
    
も大きいか小さいのようなリレーショナル演算子を使用して日付の値の型を比較することも、範囲演算子 **.** の範囲として指定されたのか。たとえば、受信:\>2013/11/30 が送信される:\>昨日、= received:12/1/2013..today は、すべての有効なクエリ文字列とします。 
  
### <a name="using-a-boolean-value-type"></a>ブール値型の使用

ブール値型は、"true"または"false"にあります。 Isread:false は isread:FALSE と同じ結果になりますので、値は、大文字小文字を区別ではありません。
  
### <a name="using-a-number-value-type"></a>数値型の使用

として完全一致の場合は、番号の値の型を検索できますも検索するよりも大きいか小さいのようなリレーショナル演算子を使用するよりもします。 サイズ: 10000 が正確に、10000 バイトですが、サイズのサイズを持っているアイテムのみを取得するたとえば、:\>= 10000 は 10000 バイト以上のサイズを持っているアイテムを返します。 範囲演算子 ( **.**) を使用して範囲を指定することもできます。 たとえば、サイズ: 7000..8000 は 7000 と 8000 の間のサイズを持っているアイテムに戻ります。 
  
### <a name="using-logical-operators"></a>論理演算子の使用

クエリ文字列は、次の論理演算子をサポートします。
  
**表 2 になります。論理演算子がサポートされています。**

|**演算子**|**例**|
|:-----|:-----|
|AND  <br/> |project AND from:"Sadie Daniels"  <br/> subject:(project AND plan)  <br/> |
|OR  <br/> |subject:meeting OR from:"Hope Gross"  <br/> from:("Sadie Daniels" OR "Hope Gross")  <br/> |
|NOT  <br/> |NOT from:"Ronnie Sturgis"  <br/> received:NOT today  <br/> |
   
複数の条件を結合する、または 1 つのキーワード/値ペア内の複数の値を結合するに、これらの演算子を使用することに注意してください。 ただし、1 つのキーワード/値ペアで複数の値を結合し、ときに、複数の値を囲むかっこを使用してください。 理由を理解してから検索を検討してください:"Sadie Daniels"または「を期待して粗」です。 実際にこの検索は、次の条件として解釈されます。
  
- アイテムが Sadie Daniels からのもの、または
    
- アイテムのインデックス付きプロパティのいずれかに「Hope Gross」という語句がある。
    
対照的に、: ("Sadie Daniels"または「を期待して粗」) として解釈されます。 
  
- アイテムが Sadie Daniels からのもの、または
    
- アイテムが Hope Gross からのもの
    
既定の演算子と、複数の条件が指定されていますが、論理演算子は含まれていません。 たとえば、添付ファイル: true は、件名: プロジェクトは、: 添付ファイル: true AND 件名: プロジェクトです。
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>例:クエリ文字列と EWS マネージ API を使用してアイテムを検索する
<a name="bk_ExampleEWSMA"> </a>

この例では、 **SearchWithQueryString**と呼ばれるメソッドを定義します。 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクト、 [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)オブジェクト、およびパラメーターとしてクエリ文字列を表す**string**オブジェクトがかかります。 次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ**ExchangeService**オブジェクトが初期化されたことを前提としています。 
  
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

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>例:クエリ文字列と EWS を使用してアイテムを検索する
<a name="bk_ExampleEWS"> </a>

この例では、SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)要求は、件名に「プロジェクト計画」という語句で受信トレイのすべての項目を検索します。 
  
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
- [EWS を使って Exchange 検索フィルターを使用します。](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- 
  [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

