---
title: Exchange で EWS を使用して、予定を削除し、会議をキャンセルする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Exchange の EWS マネージ API または EWS を使用して、予定と会議を削除する方法を説明します。
ms.openlocfilehash: c71272bf753432a9f343adc917b444424fe3ba33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354079"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="5e1bc-103">Exchange で EWS を使用して、予定を削除し、会議をキャンセルする</span><span class="sxs-lookup"><span data-stu-id="5e1bc-103">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>

<span data-ttu-id="5e1bc-104">Exchange の EWS マネージ API または EWS を使用して、予定と会議を削除する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-104">Learn how to delete appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5e1bc-105">会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいない点です。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="5e1bc-106">予定も会議も、単一のインスタンスまたは定期的に連続で発生するアイテムの一部ですが、予定は出席者、会議室、またはリソースを含まないため、メッセージの送信を必要としません。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="5e1bc-107">内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="5e1bc-108">EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) または EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) 要素を使用して、会議や予定を操作します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-108">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="5e1bc-109">**表 1. 予定や会議を削除するための EWS マネージ API メソッドおよび EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5e1bc-109">**Table 1.  EWS Managed API methods and EWS operations for deleting appointments and meetings**</span></span>

|<span data-ttu-id="5e1bc-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="5e1bc-110">**EWS Managed API method**</span></span>|<span data-ttu-id="5e1bc-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5e1bc-111">**EWS operation**</span></span>|<span data-ttu-id="5e1bc-112">**目的**</span><span class="sxs-lookup"><span data-stu-id="5e1bc-112">**What it does**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="5e1bc-113">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="5e1bc-113">Appointment.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5e1bc-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5e1bc-114">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |<span data-ttu-id="5e1bc-115">予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-115">Deletes an appointment.</span></span>  <br/> |
|[<span data-ttu-id="5e1bc-116">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="5e1bc-116">Appointment.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5e1bc-117">Createitem (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="5e1bc-117">CreateItem (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md) <br/> |<span data-ttu-id="5e1bc-118">会議を削除します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-118">Deletes a meeting.</span></span>  <br/> |
   
<span data-ttu-id="5e1bc-119">EWS を使用して予定を削除する場合、[DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用しますが、会議を削除する場合は、[CreateItem](../web-service-reference/createitem-operation-calendar-item.md) 操作を使用することにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-119">Note that when you delete an appointment by using EWS, you use the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, but when you delete a meeting, you use the [CreateItem ](../web-service-reference/createitem-operation-calendar-item.md) operation. This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> <span data-ttu-id="5e1bc-120">直観に反しているように思えるかもしれませんが、これは会議出席依頼の返信オブジェクトを作成して、会議のキャンセル メッセージを出席者に送信する必要があるためです。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-120">Note that when you delete an appointment by using EWS, you use the DeleteItem operation, but when you delete a meeting, you use the CreateItem  operation. This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> 

<span data-ttu-id="5e1bc-121"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5e1bc-121"></span></span>

## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="5e1bc-122">EWS マネージ API を使用して予定を削除する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-122">Delete an appointment by using the EWS Managed API</span></span>

<span data-ttu-id="5e1bc-123">次のコード例は、[Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) メソッドを使用して予定表フォルダーから予定を削除する方法と、[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドを使用して削除済みアイテム フォルダー内で予定を検索し、予定が削除されたことを確認する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-123">The following code example shows how to use the [Deletehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method to delete an appointment from your calendar folder, and the [ExchangeService.FindItemshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method to verify that the appointment was deleted by looking for it in the Deleted Items folder.</span></span> 
  
<span data-ttu-id="5e1bc-124">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-124">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="5e1bc-125">ローカル変数 `appointmentId` は、既存の予定に関連付けられた識別子です。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-125">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
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

<span data-ttu-id="5e1bc-p104">この例では、削除済みアイテム フォルダー内の最初のアイテムの件名と削除された予定の件名が一致していることを確認することで、予定が削除されたことを確認する簡単な方法を示します。予定が削除されたことの確認をどのように行うかは、アプリケーションのニーズによって異なります。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-p104">This example shows a simple way to verify that the appointment was deleted, by verifying that the subject of the first item in the Deleted Items folder matches that of the deleted appointment. How you choose to verify that your appointment was deleted will vary based the needs of your application.</span></span>
  
<span data-ttu-id="5e1bc-p105">ご覧のように、予定を削除するのは簡単で、ほぼ予想通りに行えます。検証手順を作成する場合、削除済みアイテム フォルダー内にある予定アイテムの ItemId は、予定表フォルダーの予定アイテムの ItemId とは異なることにご注意ください。アイテムは、単に削除済アイテム フォルダーに移動されるのではなく、コピーされて削除されます。 </span><span class="sxs-lookup"><span data-stu-id="5e1bc-p105">As you can see, deleting an appointment is straightforward and pretty much what you might expect. Note when you create your verification step that the appointment item in the Deleted Items folder has a different ItemId than the appointment item in the calendar folder. The item is copied and deleted rather than simply moved to the Deleted Items folder.</span></span> 
  
## <a name="delete-an-appointment-by-using-ews"></a><span data-ttu-id="5e1bc-131">EWS を使用して予定を削除する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-131">Delete an appointment by using EWS</span></span>
<span data-ttu-id="5e1bc-132"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5e1bc-132"></span></span>

<span data-ttu-id="5e1bc-133">次の例の要求と応答の XML は、「[EWS マネージ API を使用して予定を削除する](#bk_DeleteApptEWSMA)」の EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-133">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update an appointment by using the EWS Managed API](#bk_DeleteApptEWSMA).</span></span> <span data-ttu-id="5e1bc-134">予定アイテムが削除済みアイテム フォルダー内にあることを確認する要求と応答の XML も同様に示されています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-134">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in Delete an appointment using the EWS Managed API. The request and response XML that verifies that the appointment item is in the Deleted Items folder is shown as well.</span></span>
  
<span data-ttu-id="5e1bc-135">次の例は、[DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を利用して予定を削除するときの、要求 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-135">The following example shows the request XML for the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation to delete an appointment.</span></span> 
  
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

<span data-ttu-id="5e1bc-136">次の例は、[DeleteItem](../web-service-reference/deleteitem-operation.md) 操作で返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-136">The following example shows the response XML that is returned by the [GetItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> <span data-ttu-id="5e1bc-137">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="5e1bc-138">次の例は、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作の要求 XML を表しています。この操作は、アイテムの件名と削除された予定のオブジェクトの件名を比較するために、削除済みアイテム フォルダー内の最初のアイテムを取得します。 </span><span class="sxs-lookup"><span data-stu-id="5e1bc-138">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
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

<span data-ttu-id="5e1bc-139">次の例は、検証手順で、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作によって返される応答 XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-139">The following example shows the response XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5e1bc-140">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-140">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="5e1bc-141"><a name="bk_DeleteMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="5e1bc-141"></span></span>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="5e1bc-142">EWS マネージ API を使用して会議を削除する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-142">Delete a meeting by using the EWS Managed API</span></span>

<span data-ttu-id="5e1bc-p108">予定表フォルダーから予定アイテムを削除することに加え、会議を削除する場合は、出席者に会議のキャンセルを送信することもできます。会議をキャンセルするのに、次の 3 つのメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-p108">When you delete a meeting, in addition to removing the appointment item from the calendar folder, you might also want to send meeting cancellations to attendees. You can use the following three methods to cancel a meeting:</span></span>
  
- [<span data-ttu-id="5e1bc-145">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="5e1bc-145">Appointment.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5e1bc-146">Appointment.CancelMeeting</span><span class="sxs-lookup"><span data-stu-id="5e1bc-146">Appointment.CancelMeeting</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="5e1bc-147">CancelMeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5e1bc-147">CancelMeetingMessage</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
<span data-ttu-id="5e1bc-148">選択するメソッドは、キャンセルのメッセージで指定する必要のある詳細レベルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-148">The method that you choose depends on the level of detail you need to provide in your cancellation message.</span></span> <span data-ttu-id="5e1bc-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) を使用すると、更新されたメッセージをパラメーターとして渡すことによって、キャンセルのメッセージを簡単に更新できます。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) makes it easy to update the cancellation message by passing an updated message as a parameter.</span></span> <span data-ttu-id="5e1bc-150">[CancelMeetingMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) では、メッセージのプロパティを変更してからキャンセル通知を送信できるので、開封確認の要求などの操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-150">[CancelMeetingMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) allows you to modify properties on your message before sending a cancellation, so you can do things like request a receipt.</span></span> 
  
<span data-ttu-id="5e1bc-151">このセクションのコード例では、会議を削除して、会議のキャンセル通知を送信する異なる方法を示します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-151">The code examples in this section show the different ways to delete a meeting and send meeting cancellations.</span></span> <span data-ttu-id="5e1bc-152">これらの例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-152">The examples assume that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="5e1bc-153">ローカル変数 `meetingId` は、対象のユーザーが会議開催者である既存の会議に関連付けられた識別子です。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-153">The local variable  `meetingId` is an identifier associated with an existing meeting where the target user is the meeting organizer.</span></span> 
  
<span data-ttu-id="5e1bc-154">次のコード例は、[Appointment.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) メソッドを使用して会議を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-154">The following code example shows how to delete a meeting by using the [Appointment.Deletehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="5e1bc-155">次のコード例は、[CancelMeeting](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) メソッドを使用して会議を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-155">The following code example shows how to delete a meeting by using the [CancelMeetinghttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

<span data-ttu-id="5e1bc-156">次のコード例は、[Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) メソッドを使用して会議を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-156">The following code example shows how to delete a meeting by using the [Appointment.CreateCancelMeetingMessagehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) method.</span></span> 
  
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

## <a name="delete-a-meeting-by-using-ews"></a><span data-ttu-id="5e1bc-157">EWS を使用して会議を削除する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-157">Delete a meeting by using EWS</span></span>
<span data-ttu-id="5e1bc-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span><span class="sxs-lookup"><span data-stu-id="5e1bc-158"></span></span>

<span data-ttu-id="5e1bc-159">次の例の要求と応答の XML は、「[EWS マネージ API を使用して予定を削除する](#bk_DeleteMtgEWSMA)」の [Appointment.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) メソッドを使用した EWS マネージ API コードの呼び出しに対応します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-159">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete a meeting using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the [Appointment.Deletehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="5e1bc-160">次の例では、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、出席者にキャンセルのメッセージを送信し、会議を削除する場合の要求 XML を示します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-160">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to send cancellation messages to attendees and delete a meeting.</span></span> 
  
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

<span data-ttu-id="5e1bc-161">次の例では、会議の削除に使用される [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作要求への応答として返される XML の例を示します。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-161">The following example shows the XML that is returned in response to a [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation request used to delete a meeting.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5e1bc-162">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-162">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="5e1bc-163">次の例は、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作の要求 XML を表しています。この操作は、アイテムの件名と削除された予定のオブジェクトの件名を比較するために、削除済みアイテム フォルダー内の最初のアイテムを取得します。 </span><span class="sxs-lookup"><span data-stu-id="5e1bc-163">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
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

<span data-ttu-id="5e1bc-164">次の例は、検証手順で、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作によって返される XML を表しています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-164">The following example shows the XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5e1bc-165">**Id** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-165">The **Id** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="5e1bc-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e1bc-166">See also</span></span>

- [<span data-ttu-id="5e1bc-167">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="5e1bc-167">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)    
- [<span data-ttu-id="5e1bc-168">Exchange 2013 で EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-168">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="5e1bc-169">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-169">How to: Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="5e1bc-170">Exchange で EWS を使用して予定と会議を更新する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-170">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="5e1bc-171">Exchange で EWS を使用して会議の新しい日時を提案する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-171">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="5e1bc-172">Exchange で EWS を使用して会議の新しい日時を提案する</span><span class="sxs-lookup"><span data-stu-id="5e1bc-172">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

