---
title: Exchange で EWS を使用して予定表に代理人としてアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。
ms.openlocfilehash: 609e5f0bb22c78174289a2eb10210999c8391a3d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353841"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>Exchange で EWS を使用して予定表に代理人としてアクセスする

Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。
  
EWS マネージ API または EWS を使用して、メールボックス所有者の予定表フォルダーへの代理人アクセス権をユーザーに付与できます。 そうすることにより代理人は、アクセス許可に応じて、メールボックス所有者の代理としての会議出席依頼の作成、予定の作成、会議出席依頼への応答、メールボックス所有者の予定表フォルダーにある会議の取得、更新、および削除を行えます。
  
代理人は、自分自身の予定表フォルダーにアクセスする際に使用するのと同じメソッドと操作を使用して、メールボックス所有者の予定表フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して予定表アイテムまたは予定表サブフォルダーを検索または作成する必要がある点です。アイテム ID またはフォルダー ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、または削除できます。 
  
**表 1. 代理人として予定表にアクセスするための EWS マネージ API メソッドと EWS 操作**

|**目的**|**使用する EWS マネージ API メソッド…**|**使用する EWS 操作…**|
|:-----|:-----|:-----|
|会議または予定を代理人として作成する  <br/> |[Appointment.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx): [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の予定表フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|複数の会議または予定を代理人として作成する  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|予定または会議を代理人として検索または検出する  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|予定または会議を代理人として取得する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|予定または会議を代理人として更新する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Appointment.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|予定または会議を代理人として削除する  <br/> |[Appointment.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Appointment.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> この記事のコード例では、primary@contoso.com がメールボックス所有者です。 
  
## <a name="prerequisite-tasks"></a>事前に必要なタスク
<a name="bk_prereq"> </a>

ユーザーが代理人としてメールボックス所有者の予定表フォルダーにアクセスするためには、そのユーザーは、メールボックス所有者の予定表フォルダーに、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)追加されていなければなりません。 
  
代理人は、メールボックス所有者の予定表を更新するには、自身のアカウントにアタッチされたメールボックスが必要です。
  
代理人が会議出席依頼と応答だけを処理すればよい場合は、予定表フォルダーに代理人を追加し、既定の [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS マネージ API 列挙値または [DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS 要素値 **DelegatesAndSendInformationToMe** を使用して、出席依頼を代理人に送信し、情報メッセージをメールボックス所有者に送信します。 こうすると、メールボックス所有者の受信トレイ フォルダーへのアクセス権を代理人に付与する必要はありません。 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して会議または予定を代理人として作成する
<a name="bk_createewsma"> </a>

EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成できます。 この例は、[Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。 
  
この例では、**service** が代理人の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、メールボックス所有者の予定表フォルダーに対する適切なアクセス許可が代理人に付与されいることを前提にしています。 
  
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

アイテムの保存時には、[Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッド呼び出しでメールボックス所有者の予定表フォルダーを識別する必要があることにご注意ください。 メールボックス所有者の予定表フォルダーを指定しない場合、会議出席依頼はメールボックス所有者の予定表フォルダーではなく、代理人の予定表フォルダーに保存されます。 メールボックス所有者の予定表フォルダーは、2 つの方法で **Save** メソッド呼び出しに含めることができます。 メールボックス所有者の [WellKnownFolderName](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) と SMTP アドレスを使用して、[FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) オブジェクトの新しいインスタンスをインスタンス化することをお勧めします。 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

ただし、最初に予定表フォルダーに [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) してから、**Save** メソッド呼び出しでフォルダーの ID を使用することもできます。 ただし、これにより追加の EWS 呼び出しが作成されることにご注意ください。 
  
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

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成できます。この例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。 
  
これは、**Save** メソッドを使用して[会議または予定を代理人として作成する](#bk_createewsma)場合に EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで **CreateItem** 要求に応答します。このメッセージには、会議が正常に作成されたことを示す [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値 **NoError** が含まれます。また、この応答には新しく作成された会議のアイテム ID も含まれます。
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して会議または予定を代理人として検索する
<a name="bk_searchewsma"> </a>

会議を検索するには、メールボックス所有者の予定表フォルダーを指定するために、[FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターが含まれるいずれかの [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドを使用する必要があります。 
  
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

**FindItems** 呼び出しが ID を含む応答を返すと、ID と[暗黙的アクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して対象の会議を取得、更新、削除できます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>EWS を使用して会議または予定を代理人として検索する
<a name="bk_searchews"> </a>

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、検索条件のセットに一致する予定および会議を検索できます。この例は、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、メールボックス所有者の予定表フォルダーの中で件名に "building" という単語が含まれる会議を検索する方法を示しています。  
  
これは、**FindItem** メソッドを使用して[会議または予定を代理人として検索する](#bk_searchewsma)場合に EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、[FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) メッセージで **FindItem** 要求に応答します。このメッセージには、検索が正常に完了したことを示す [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値 **NoError** が含まれます。この応答には、検索条件に一致する予定または会議の [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) が含まれます。この例では、検出された会議は 1 つだけです。 
  
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

条件と一致する会議の **ItemId** が分かったので、**ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して、会議の取得、更新、削除を行えます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して予定表アイテムを代理人として取得、更新、または削除する
<a name="bk_geteswma"> </a>

EWS マネージ API を使用して、代理人アクセスを使用しない場合と同じ方法で、会議または予定を取得、更新、または削除できます。 唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。 **Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の予定表フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 2. 予定および会議を代理人として処理するための EWS マネージ API メソッド**

|**タスク**|**EWS マネージ API メソッド**|**コード例**|
|:-----|:-----|:-----|
|予定または会議を取得する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|予定または会議を更新する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用して会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|予定または会議を削除する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用して会議を削除する](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>EWS を使用して予定表アイテムを代理人として取得、更新、または削除する
<a name="bk_getews"> </a>

EWS を使用して、代理人アクセスを使用しない場合と同じ方法で、会議または予定を取得、更新、または削除できます。 唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。 [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の予定表フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 3. 予定および会議を代理人として処理するための EWS 操作**

|**タスク**|**EWS 操作**|**コード例**|
|:-----|:-----|:-----|
|予定または会議を取得する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[EWS を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|予定または会議を更新する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[EWS を使用して会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|予定または会議を削除する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)   
- [Exchange で EWS を使用して代理人を追加および削除する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    

