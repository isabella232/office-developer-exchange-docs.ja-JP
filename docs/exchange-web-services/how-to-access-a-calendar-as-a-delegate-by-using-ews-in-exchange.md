---
title: EWS を使用して Exchange 内で代理人に予定表にアクセスします。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。
ms.openlocfilehash: 24327c28f58e728807fc5581b480d3c01d3b7208
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758916"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>EWS を使用して Exchange 内で代理人に予定表にアクセスします。

Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。
  
EWS のマネージ API を使用することができます。 または EWS をユーザーに与えるにはメールボックス所有者の予定表フォルダーへのアクセスを委任します。 代理人ことができますし、メールボックス所有者の代理として会議出席依頼を作成、予定を作成、会議出席依頼への対応し取得、更新、およびアクセス許可に応じて、メールボックス所有者の予定表フォルダーから会議を削除します。
  
代理人は、自分の予定表フォルダーへのアクセスに使用するメールボックスの所有者の予定表フォルダーにアクセスするのには、同じメソッドと演算を使用します。 主な違いは、アイテム ID またはフォルダー ID を識別した後ことができます[アクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用する暗黙の型を取得、更新、またはアイテムを削除するを検索] または [予定表アイテムまたは予定表のサブフォルダーを作成する[明示的なアクセス権](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用する必要です。 
  
**表 1 です。EWS のマネージ API のメソッドとデリゲートとして予定表にアクセスするための EWS の操作**

|**目的…**|**この EWS 管理 API メソッドを使用してください.**|**EWS 操作を使用してください.**|
|:-----|:-----|:-----|
|会議または予定を代理人として作成する  <br/> |[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) [フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターが、メールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定  <br/> |
|複数の会議または予定を代理人として作成する  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定  <br/> |
|予定または会議を代理人として検索または検出する  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定  <br/> |
|予定または会議を代理人として取得する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|予定または会議を代理人として更新する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)の後に <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて <br/> |
|予定または会議を代理人として削除する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)の後に <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に <br/> |
   
> [!NOTE]
> この記事のコード例では、primary@contoso.com がメールボックス所有者です。 
  
## <a name="prerequisite-tasks"></a>事前に必要なタスク
<a name="bk_prereq"> </a>

ユーザーは、代理人にメールボックス所有者の予定表] フォルダーにアクセスできる、前に、ユーザーがメールボックス所有者の予定表フォルダーへの[アクセス許可を持つ代理人として追加](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)する必要があります。 
  
代理人は、メールボックス所有者の予定表を更新するには、自身のアカウントにアタッチされたメールボックスが必要です。
  
代理人が会議出席依頼や出欠の返答を操作する必要がある場合のみ、予定表フォルダーに代理人を追加して既定[MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS のマネージ API の列挙値、または、[を使用して、DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx)代理人および情報のメッセージをメールボックスの所有者に要求を送信する**DelegatesAndSendInformationToMe**の EWS の要素の値です。 メールボックスの所有者の受信トレイ フォルダーに対するアクセス権を付与することにし、代理人は必要ありません。 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して会議または予定を代理人として作成する
<a name="bk_createewsma"> </a>

EWS のマネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成することができます。 この例では、 [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)メソッドを使用して、会議を作成し、出席者に会議出席依頼を送信する方法を示します。 
  
この例ではその**サービス**は、デリゲートの有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと代理人にメールボックス所有者の予定表フォルダーに対する適切なアクセス許可が付与されています。 
  
```cs
private static void DelegateAccessCreateMeeting(ExchangeService service)
{
    Appointment meeting = new Appointment(service);
    // Set the properties on the meeting object to create the meeting.
    meeting.Subject = "Team building exercise";
    meeting.Body = "Let's learn to really work as a team and then have lunch!";
    meeting.Start = DateTime.Now.AddDays(2);
    meeting.End = meeting.Start.AddHours(4);
    meeting.Location = "Conference Room 12";
    meeting.RequiredAttendees.Add("sadie@contoso.com");
    meeting.ReminderMinutesBeforeStart = 60;
    // Save the meeting to the Calendar folder for 
    // the mailbox owner and send the meeting request.
    // This method call results in a CreateItem call to EWS.
    meeting.Save(new FolderId(WellKnownFolderName.Calendar, 
        "primary@contoso.com"), 
        SendInvitationsMode.SendToAllAndSaveCopy);
    // Verify that the meeting was created.
    Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
    Console.WriteLine("\nMeeting created: " + item.Subject + "\n");
}
```

アイテムを保存するとき[保存](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)メソッドの呼び出しは、メールボックス所有者の予定表フォルダーを指定する必要があることに注意してください。 メールボックス所有者の予定表フォルダーが指定されていない場合、会議出席依頼が代理人の予定表およびメールボックス所有者の予定表フォルダーではなく保存されます。 **保存**メソッドの呼び出しで 2 つの方法では、メールボックス所有者の予定表フォルダーを含めることができます。 [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)とメールボックス所有者の SMTP アドレスを使用して、[フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)のオブジェクトの新しいインスタンスをインスタンス化することをお勧めします。 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

ただし、することも[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)予定表フォルダーを最初に、し、**保存**メソッドの呼び出し内のフォルダーの ID を使用します。 注意してください、ただし、この EWS 呼び出しを作成します。 
  
```cs
    // Identify the mailbox owner's SMTP address
    // and bind to their Calendar folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryCalendar = Folder.Bind(service, 
        new FolderId(WellKnownFolderName.Calendar, primary)); 
…
    // Save the meeting to the Calendar folder for the mailbox owner and send the meeting request.
    meeting.Save(primaryCalendar.Id, 
        SendInvitationsMode.SendToAllAndSaveCopy);
```

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>EWS を使用して会議または予定を代理人として作成する
<a name="bk_createews"> </a>

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成することができます。 次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。 
  
[会議または予定を代理人として作成](#bk_createewsma)するのには**Save**メソッドを使用する場合、EWS のマネージ API を送信する XML 要求にもです。
  
簡潔にするために、次の例では SOAP ヘッダーが削除されています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
…
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a 
              team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-09T23:26:33.756-05:00</t:Start>
          <t:End>2014-03-10T03:26:33.756-05:00</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは、 **CreateItem**要求**NoError**会議が正常に作成されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。 応答には、新しく作成した会議のアイテムの ID も含まれています。
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して会議または予定を代理人として検索する
<a name="bk_searchewsma"> </a>

会議を検索するにする必要があります使用する、[フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)のパラメーターを含む[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)の方法のいずれかのメールボックス所有者の予定表フォルダーを指定することができますように。 
  
```cs
static void DelegateAccessSearchWithFilter
    (ExchangeService service, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Define the sort order.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching calendar items. 
        // The FindItems parameters must denote the mailbox owner,
        // mailbox, and Calendar folder.
        // This method call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(
        new FolderId(WellKnownFolderName.Calendar, 
            "primary@contoso.com"), 
            filter, 
            view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while 
            enumerating results: {0}", ex.Message);
    }
}
```

**FindItems**の呼び出しには、ID を使用して応答が返されます後の取得、更新または削除できますその会議 ID と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して、メールボックス所有者の SMTP アドレスを指定する必要はありませんし。 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>EWS を使用して会議または予定を代理人として検索する
<a name="bk_searchews"> </a>

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、予定と検索条件のセットに一致する会議を検索することができます。 [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作を使用して、件名に「建物」という単語が含まれているメールボックス所有者の予定表フォルダー内の会議を検索する方法を次の使用例に示します。 
  
EWS のマネージ API は、[会議または予定を代理人としての](#bk_searchewsma) **FindItem**メソッドを使用する場合を送信する XML 要求にもです。
  
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
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="building" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

**FindItem**要求に対して、 **NoError**を示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値の検索が正常に完了を含む[FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx)メッセージは、サーバーが応答します。 応答には、予定または会議の検索条件に一致するための[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)が含まれています。 この例では、1 つだけの会議が見つかりました。 
  
[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="IJpUAAA="
                          ChangeKey="DwAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAAAIKhS" />
                <t:Subject>Team building exercise</t:Subject>
                <t:DateTimeReceived>2014-03-04T21:27:22Z</t:DateTimeReceived>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

これで、条件に一致する会議の**アイテム Id**がある場合は、取得、更新、または削除できますその会議**ItemId**と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して、メールボックス所有者の SMTP アドレスを指定する必要はありませんし。 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して予定表アイテムを代理人として取得、更新、または削除する
<a name="bk_geteswma"> </a>

取得、更新、または会議出席依頼や予定を代理人アクセスを使用していないときにこれらのアクションを実行すると同じ方法で削除するのには、EWS のマネージ API を使用できます。 唯一の違いは、サービス オブジェクトの代理人のユーザーです。 **バインド**メソッドの呼び出しを一意に含まれる項目 ID では、メールボックス所有者の予定表フォルダーに、メールボックス ストア内の項目を識別します。 
  
**表 2 になります。EWS のマネージ API のメソッドの代理人としての予定や会議を使用**

|**タスク**|**EWS マネージ API メソッド**|**コードの例**|
|:-----|:-----|:-----|
|予定または会議を取得する  <br/> |[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[EWS のマネージ API を使用してアイテムを取得します。](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|予定または会議を更新する  <br/> |[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx)[の更新](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)の後に <br/> |[EWS のマネージ API を使用して会議を更新します。](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|予定または会議を削除する  <br/> |の[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx)[を削除](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)後に <br/> |[EWS のマネージ API を使用して会議を削除します。](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>EWS を使用して予定表アイテムを代理人として取得、更新、または削除する
<a name="bk_getews"> </a>

取得、更新、または会議出席依頼や予定を代理人アクセスを使用していないときにこれらのアクションを実行すると同じ方法で削除するのには、EWS を使用できます。 唯一の違いは、サービス オブジェクトの代理人のユーザーです。 [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx)メソッドの呼び出しを一意に含まれる項目 ID では、メールボックス所有者の予定表フォルダーに、メールボックス ストア内の項目を識別します。 
  
**表 3。代理人としての [予定と会議を操作するための EWS の操作**

|**タスク**|**EWS 操作**|**コードの例**|
|:-----|:-----|:-----|
|予定または会議を取得する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[EWS を使用してアイテムを取得します。](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|予定または会議を更新する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて <br/> |[EWS を使用して会議を更新します。](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|予定または会議を削除する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)   
- [追加し、Exchange の EWS を使用して、デリゲートを削除します。](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可を設定します。](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Calendars and EWS in Exchange](calendars-and-ews-in-exchange.md)
    

