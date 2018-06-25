---
title: EWS を使用して Exchange で Exchange メールボックスのアイテムを扱う
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Exchange で EWS マネージ API または EWS を使用して、アイテムを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: e70ac499da57faa60b4bcb6082648b23d1a7e791
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759082"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>EWS を使用して Exchange で Exchange メールボックスのアイテムを扱う

Exchange で EWS マネージ API または EWS を使用して、アイテムを作成、取得、更新、削除する方法について説明します。
  
EWS のマネージ API または EWS を使用するには、メールボックス内のアイテムに対する作業をします。 汎用アイテムを使用することができます-EWS のマネージ API の[項目](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)のオブジェクトまたは EWS の[項目](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx)の種類-(アイテムを取得または項目を削除する項目の識別子を使用して) いくつかの操作を実行するにはただし、ほとんどの[項目を厳密に型指定](folders-and-items-in-ews-in-exchange.md#bk_item)を使用して取得操作を実行またはプロパティにアクセスする必要がありますので、操作を更新する必要があります、厳密に型指定された項目を特定します。 

たとえば、開始を含む項目を取得し、終了日に一般的なアイテムを使用することはできません -、EWS のマネージ API の[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)オブジェクトまたはそのためには、EWS の[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)の種類が必要です。 EWS のマネージ API を使用する場合を使用して常に、厳密に型指定された項目を作成する**品目**のジェネリック クラスにはコンス トラクターがないためです。 ない厳密に型指定されるアイテムを扱う場合、アイテムを操作する**項目**の基本クラスを常に使用することができます。 
  
**表 1. アイテムを処理するための EWS マネージ API メソッドと EWS 操作**

|**目的…**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|汎用アイテムを作成する  <br/> |なし。EWS マネージ API を使用して特定のアイテムの種類のみを作成できます。汎用アイテムを作成することはできません。  <br/> |[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|アイテムを取得する  <br/> |[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|アイテムを更新する  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|アイテムを削除する  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
この記事では、タスクを実行するために、汎用基本クラスを使用する場合と、厳密に型指定されたアイテムを使用する場合とについて説明します。コード例では、基本クラスを使用する方法と、基本クラスを使用できないとき、または基本クラスがニーズに合わないときの対処法を示しています。
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアイテムを作成する
<a name="bk_createewsma"> </a>

EWS マネージ API には、[Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) クラスの公式コンストラクターがないため、アイテムを作成するには、作成したい特定のアイテムの種類のためのコンストラクターを使用する必要があります。たとえば、 [EmailMessage クラス コンストラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)を使用して、新しい電子メール メッセージを作成したり、[Contact クラス コンストラクター](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)を使用して新しい連絡先を作成したりします。同様に、サーバーは応答で汎用 **Item** オブジェクトを返すことはありません。すべての汎用アイテムは、 **EmailMessage** オブジェクトとして返されます。 
  
作成するアイテムの種類が分かっている場合、わずかな手順だけでタスクを完了できます。この手順は、すべてのアイテムの種類について同様になります。
  
1. パラメータとして [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オプジェクトを持ついずれかの [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) クラスの新しいインスタンスを初期化します。 
    
2. アイテムのプロパティを設定します。スキーマはアイテムの種類ごとに異なるため、利用できるプロパティはアイテムに応じて異なってきます。
    
3. アイテムを保存するか、アイテムを保存して送信します。
    
たとえば、[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトを作成して、 [Subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx)、[Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)、および [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) の各プロパティを設定し、 [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを使用して送信できます。 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

EWS のマネージ API を使用して会議または予定アイテムを作成する方法については、[予定および会議では、Exchange 2013 の EWS を使用して作成](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)を参照してください。
  
## <a name="create-an-item-by-using-ews"></a>EWS を使用してアイテムを作成する
<a name="bk_createews"> </a>

EWS を使用して、汎用アイテムまたは厳密に型指定されたアイテムを作成できます。この手順は、すべてのアイテムの種類について同様になります。
  
1. [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) 操作を使用して、Exchange ストアのアイテムを作成します。 
    
2. [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) 要素を使用して、作成する 1 つ以上のアイテムを含めます。 
    
3. アイテムのプロパティを設定します。
    
たとえば、次の例のコードを使用し、電子メール メッセージを作成して送信できます。これは、[SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
EWS を使用して会議または予定アイテムを作成する方法については、[予定および会議では、Exchange 2013 の EWS を使用して作成](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)を参照してください。
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアイテムを取得する
<a name="bk_getewsma"> </a>

取得するアイテムの [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) が分かっている場合に EWS マネージ API を使用してアイテムを取得するには、アイテムに対して [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドのいずれかを呼び出すだけでアイテムが取得されます。ベスト プラクティスとして、必要なものだけを返すようにプロパティを制限することをお勧めします。次の例では、アイテムの **Id** プロパティと **Subject** プロパティを返します。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

特定の条件を満たすアイテムを検索している場合は、次の操作を行います。
  
1. 取得するアイテムを含むフォルダーにバインドします。
    
2. [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) または [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) をインスタンス化して、返すアイテムをフィルターにかけます。 
    
3. [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) オブジェクトまたは [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) オブジェクトをインスタンス化して、返すアイテムの数を指定します。 
    
4. [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを呼び出します。 
    
たとえば、受信トレイに未読の電子メール メッセージを取得する場合は、次の例のコードを使用します。この例では、 **SearchFilterCollection** を使用して **FindItems** メソッドの結果を未読のメッセージに制限し、 **ItemView** を制限して結果を 1 つのアイテムに制限します。 [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) の値が [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx).の一部であるため、この特定のコードは、 **EmailMessage** オブジェクトでのみ機能します。 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

また、次のコード例に示すように、[PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) を使用して検索結果を制限することもできます。この例では、 [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを使用して、次の 30 日間で発生する最大 5 つの予定を取得します。このコードは、予定表アイテムでのみ機能します。 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

**Bind** メソッドの応答でサーバーが返す情報は、 **FindItem** メソッドまたは **FindAppointment** メソッドの応答でサーバーが返す情報とは異なります。 **Bind** メソッドは、すべてのスキーマ化されたプロパティを返すことができますが、 **FindItem** メソッドと **FindAppointment** メソッドは、スキーマ化されたすべてのプロパティを返しません。このため、アイテムに対するフル アクセスが必要な場合は、 **Bind** メソッドを使用する必要があります。取得するアイテムの **Id** アイテムがない場合は、 **FindItem** メソッドまたは **FindAppointment** メソッドを使用して ID を取得し、 **Bind** メソッドを使用して必要なプロパティを取得します。 
  
EWS のマネージ API を使用して会議または予定のアイテムを取得する方法については、[予定および Exchange EWS を使用して会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="get-an-item-by-using-ews"></a>EWS を使用してアイテムを取得する
<a name="bk_getews"> </a>

取得するアイテムの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が分かっている場合は、 [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用してアイテムを取得できます。 
  
次の例は、特定の [ItemId](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) を持つアイテムの **件名**を取得する XML の要求を示しています。これは、 [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) で **Bind** メソッドを呼び出す際に EWS マネージ API が送信する XML 要求でもあります。読みやすくするため、一部の属性と要素の値が短縮されています。
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

次の例は、 **GetItem** 操作の処理後にサーバーから返される XML 応答を示しています。この応答は、アイテムが正常に取得されたことを示しています。読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

取得したいアイテムの **ItemId** が分からない場合は、 [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用してアイテムを見つけることができます。 **FindItem** 操作を使用するには、検索しているフォルダーをまず識別する必要があります。 **DistinguinguishedFolderName** または [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) を使用して、フォルダーを識別できます。 [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) または [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作のいずれかを使用して、必要な **FolderId** を取得することができます。 **FindItem** 操作を使用して、検索フィルターに一致する結果をそのフォルダーで検索します。EWS マネージ APIとは異なり、EWS は、予定のための別の検索操作を提供しません。 **FindItem** 操作がすべての種類のアイテムを取得します。 
  
次の例では、次の 30 日以内に発生する予定表フォルダー内で予定を検索するためにサーバーに送信される XMLの **FindItem** 操作要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**FindItemResponse** メッセージで [FindItem](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) 要求に応答します。このメッセージには、操作が正常に完了したことを示す、 [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** の値が含まれます。予定表アイテムがフィルターの条件を満たしている場合、それらのアイテムは応答に含まれます。
  
**GetItem** 操作の応答でサーバーが返す情報は、 **FindItem** 操作または **FindAppointment** 操作の応答でサーバーが返す情報とは異なります。 **GetItem** 操作は、すべてのスキーマ化されたプロパティを返すことができますが、 **FindItem** 操作と **FindAppointment** 操作は、スキーマ化されたすべてのプロパティを返しません。このため、アイテムに対するフル アクセスが必要な場合は、 **GetItem** 操作を使用する必要があります。取得するアイテムの **ItemId** がない場合は、 **FindItem** 操作または **FindAppointment** 操作を使用して **ItemId** を取得し、 **GetItem** 操作を使用して必要な要素を取得します。 
  
EWS を使用して会議または予定のアイテムを取得する方法については、[予定および Exchange EWS を使用して会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアイテムを更新する
<a name="bk_updateewsma"> </a>

EWS マネージ API を使用してアイテムを更新する手順は、すべてのアイテムの種類について同様になります。ただし、アイテムのプロパティは、アイテムの種類ごとに異なり、[Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) メソッドには、選択できる多くのオーバーロードされたメソッドがあります。アイテムを更新するには: 
  
1. 最新バージョンのアイテムをまだ持っていない場合は、[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドを使用して取得します。厳密に型指定されたアイテム固有のプロパティを更新するには、その種類のアイテムにバインドする必要があります。汎用アイテムの種類で利用できるプロパティを更新するために、 [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトにバインドできます。 
    
2. アイテムのプロパティを更新します。
    
3. **Update** メソッドを呼び出します。 
    
たとえば、次の例のコードに示すように、汎用アイテムの種類を使用して、電子メールの件名を更新できます。
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

EWS のマネージ API を使用して会議または予定のアイテムを更新する方法については、[予定と Exchange の EWS を使用して、会議の更新](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="update-an-item-by-using-ews"></a>EWS を使用してアイテムを更新する
<a name="bk_updateews"> </a>

EWS を使用してアイテムを更新するには、次の操作を行います。
  
1. [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用し、最新バージョンのアイテムをまだ持っていない場合は取得します。 
    
2. [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作を使用して、更新するフィールドを指定し、それらのフィールドに新しい値を割り当てます。 
    
次の例は、電子メール メッセージの **Subject** の値を更新するためにサーバーに送信される XML [UpdateItem](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) 操作要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**UpdateItemResponse** メッセージを含む [UpdateItem](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) 要求に応答します。このメッセージには、アイテムが正常に更新されたことを示す、 [NoError](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値が含まれます。
  
EWS を使用して会議または予定のアイテムを更新する方法については、[予定と Exchange の EWS を使用して、会議の更新](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアイテムを削除する
<a name="bk_deleteewsma"> </a>

アイテムを、削除済みアイテム フォルダーまたはごみ箱に移動して、削除できます。削除するアイテムの [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) が分かっている場合は、アイテムに対して [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) メソッドを呼び出します。 
  
削除する前にアイテムを検索する必要がある場合は、次の操作を行います。
  
1. [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを呼び出して、削除するアイテムを検索します。 
    
1. [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) をインスタンス化して返すプロパティに制限するか、 [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) を使用して特定のアイテムを検索します。 
    
2. [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) または [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) をインスタンス化して、返すアイテムの数を指定します。 
    
2. [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) メソッドを呼び出します。 
    
たとえば次のコードは、電子メール メッセージを、削除済みアイテム フォルダーに移動する方法を示しています。
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

アイテムの削除の詳細については、「[Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)」を参照してください。 EWS のマネージ API を使用して会議または予定のアイテムを削除する方法については、[予定を削除して Exchange で EWS を使用して会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="delete-an-item-by-using-ews"></a>EWS を使用してアイテムを削除する
<a name="bk_deleteews"> </a>

[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) 操作を使用して、アイテムを削除できます。 
  
次の例は、電子メール メッセージを削除済みアイテム フォルダーに移動するためにサーバーに送信される XML 要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**DeleteItemResponse** メッセージを含む [DeleteItem](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) 要求に応答します。このメッセージには、アイテムが正常に更新されたことを示す、 [NoError](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値が含まれます。
  
アイテムの削除の詳細については、「[Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)」を参照してください。 EWS を使用して会議または予定のアイテムを削除する方法については、[予定を削除して Exchange で EWS を使用して会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="move-or-copy-items-to-another-mailbox"></a>別のメールボックスにアイテムを移動またはコピーする
<a name="bk_movecopybtnmailboxes"> </a>

[ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) 操作と [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) 操作を使用して、メールボックス間でアイテムを移動またはコピーできます。詳細については、「 [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)」を参照してください。
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)    
- [Exchange EWS を使用してフォルダーを操作します。](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)
    

