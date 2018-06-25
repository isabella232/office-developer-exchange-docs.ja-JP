---
title: 予定を削除して、Exchange で EWS を使用して会議をキャンセル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Exchange の EWS マネージ API または EWS を使用して、予定と会議を削除する方法を説明します。
ms.openlocfilehash: bd7eac803fedffc51133324259f68fd25652fcff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758944"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a>予定を削除して、Exchange で EWS を使用して会議をキャンセル

Exchange の EWS マネージ API または EWS を使用して、予定と会議を削除する方法を説明します。
  
会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいない点です。 予定と会議の両方は、単一のインスタンスまたは定期的な一連の一部ですが、予定の出席者、会議室、またはリソースを含まないため、必要としないメッセージを送信します。 内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。 EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)か、EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) 要素を使用して、会議や予定を操作します。 
  
**表 1 です。EWS のマネージ API のメソッドとの予定や会議を削除するための EWS の操作**

|**EWS マネージ API メソッド**|**EWS の操作**|**できること**|
|:-----|:-----|:-----|
|[Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |予定を削除します。  <br/> |
|[Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Createitem メソッド (予定表アイテム)](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) <br/> |会議を削除します。  <br/> |
   
EWS を使用して予定を削除すると、 [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)操作を使用することに注意してください、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用する会議を削除するとします。 直感に反するかもしれませんが、会議を作成する必要があるための出席者に会議のキャンセル通知を送信する応答オブジェクトのメッセージです。 
  
## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して予定を削除する
<a name="bk_DeleteApptEWSMA"> </a>

次のコード例では、予定表フォルダーから予定を削除する[Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)メソッドと[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)メソッドを探して、削除済みアイテム フォルダー内で予定が削除されたことを確認するのにを使用する方法を示します。 
  
次の使用例は、認証済み Exchange サーバーおよび**サービス**をという名前の[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを取得することを想定しています。 ローカル変数`appointmentId`は、既存の予定に関連付けられた識別子。 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet());
// Delete the appointment. Note that the item ID will change when the item is moved to the Deleted Items folder.
appointment.Delete(DeleteMode.MoveToDeletedItems);
// Verify that the appointment has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The appointment " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

この例では、削除済みアイテム フォルダー内の最初のアイテムの件名と削除された予定の件名が一致していることを確認することで、予定が削除されたことを確認する簡単な方法を示します。予定が削除されたことの確認をどのように行うかは、アプリケーションのニーズによって異なります。
  
ご覧のように、予定を削除するのは簡単で、ほぼ予想通りに行えます。検証手順を作成する場合、削除済みアイテム フォルダー内にある予定アイテムの ItemId は、予定表フォルダーの予定アイテムの ItemId とは異なることにご注意ください。アイテムは、単に削除済アイテム フォルダーに移動されるのではなく、コピーされて削除されます。  
  
## <a name="delete-an-appointment-by-using-ews"></a>EWS を使用して予定を削除する
<a name="bk_DeleteApptEWSMA"> </a>

要求と応答 XML を次の例では、 [EWS のマネージ API を使用して予定を削除する](#bk_DeleteApptEWSMA)EWS のマネージ API のコードの呼び出しに対応します。 要求と応答は、同様に予定アイテムが削除済みアイテム フォルダーであることを確認するための XML が表示されます。
  
予定を削除するのには、 [DeleteItem](http://msdn.microsoft.com/library/e2152410-41ce-1fe7-8169-f206d5081ebc%28Office.15%29.aspx)の操作の要求の XML の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

[DeleteItem 操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)によって返される XML 応答の例を次に示します。 **アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作での予定が削除されたオブジェクトのアイテムの件名を比較するために [削除済みアイテム フォルダー内の最初の項目を取得する要求の XML の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages
" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

応答検証の手順で[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作によって返される XML の例を次に示します。 
  
> [!NOTE]
> **アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10748" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA=" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Tennis lesson</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_DeleteMtgEWSMA"> </a>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して会議を削除する

予定表フォルダーから予定アイテムを削除することに加え、会議を削除する場合は、出席者に会議のキャンセルを送信することもできます。会議をキャンセルするのに、次の 3 つのメソッドを使用できます。
  
- [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
選択したメソッドは、キャンセルについてのメッセージで指定する必要の詳細レベルによって異なります。 [Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)では、パラメーターとして、更新されたメッセージを渡すことによって取り消しについてのメッセージを更新するのには簡単。 [CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)を使用すると、開封確認メッセージの要求などを行うことができますので、キャンセルの通知を送信する前に、メッセージのプロパティを変更できます。 
  
このセクションのコード例では、会議を削除して、会議のキャンセル通知を送信する方法を表示します。 この例では、認証済み Exchange サーバーおよび**サービス**をという名前の[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを取得することが前提です。 ローカル変数`meetingId`ターゲットである会議の開催者は、既存の会議に関連付けられている識別子です。 
  
次のコード例では、 [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)メソッドを使用して会議を削除する方法を示します。 
  
```cs
// Instantiate an appointment object for the meeting by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
            
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the Delete method.
meeting.Delete(DeleteMode.MoveToDeletedItems, SendCancellationsMode.SendToAllAndSaveCopy);
// Verify that the meeting has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The meeting " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

次のコード例では、 [CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)メソッドを使用して会議を削除する方法を示します。 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

次のコード例では、 [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx)メソッドを使用して会議を削除する方法を示します。 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CreateCancelMeetingMessage method.
CancelMeetingMessage cancelMessage = meeting.CreateCancelMeetingMessage();
cancelMessage.Body = new MessageBody("The outdoor meeting has been canceled due to hailstorms.");
cancelMessage.IsReadReceiptRequested = true;
cancelMessage.SendAndSaveCopy();

```

## <a name="delete-a-meeting-by-using-ews"></a>EWS を使用して会議を削除する
<a name="bk_EWSDeleteApptAndMeeting"> </a>

要求と応答 XML を次の例では、EWS のマネージ API コードは、 [EWS のマネージ API を使用して会議を削除する](#bk_DeleteMtgEWSMA) [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)メソッドを使用して呼び出しに対応します。 
  
次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して、出席者に取り消しメッセージを送信し、会議を削除するときに XML 要求を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:NewBodyContent BodyType="HTML">The outdoor meeting has been canceled due to hailstorms.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

次の例では、会議を削除するために、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作要求への応答で返される XML を示します。 
  
> [!NOTE]
> **アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作での予定が削除されたオブジェクトのアイテムの件名を比較するために [削除済みアイテム フォルダー内の最初の項目を取得する要求の XML の例を次に示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

検証の手順で[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作によって返される XML の例を次に示します。 
  
> [!NOTE]
> **Id**と**変更キー**の属性は、読みやすくするために短縮されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10750" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Team building exercise</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>関連項目

- [Calendars and EWS in Exchange](calendars-and-ews-in-exchange.md)    
- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [Exchange EWS を使用して予定および会議を取得します。](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [Exchange EWS を使用して予定および会議を更新します。](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [Exchange EWS を使用して、会議の新しい日時を提案します。](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [Exchange EWS を使用して、会議の新しい日時を提案します。](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

