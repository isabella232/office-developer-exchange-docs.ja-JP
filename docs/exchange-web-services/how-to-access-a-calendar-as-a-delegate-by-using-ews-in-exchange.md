---
title: Exchange で EWS を使用して予定表に代理人としてアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 20ec294ddc4ccf014f0b2148c786c8c3ef8a6069
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528294"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="99cdb-103">Exchange で EWS を使用して予定表に代理人としてアクセスする</span><span class="sxs-lookup"><span data-stu-id="99cdb-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="99cdb-104">Exchange で EWS マネージ API または EWS を使用して予定表に代理人としてアクセスする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="99cdb-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="99cdb-105">EWS マネージ API または EWS を使用して、メールボックス所有者の予定表フォルダーへの代理人アクセス権をユーザーに付与できます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="99cdb-106">そうすることにより代理人は、アクセス許可に応じて、メールボックス所有者の代理としての会議出席依頼の作成、予定の作成、会議出席依頼への応答、メールボックス所有者の予定表フォルダーにある会議の取得、更新、および削除を行えます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="99cdb-p102">代理人は、自分自身の予定表フォルダーにアクセスする際に使用するのと同じメソッドと操作を使用して、メールボックス所有者の予定表フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して予定表アイテムまたは予定表サブフォルダーを検索または作成する必要がある点です。アイテム ID またはフォルダー ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-p102">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder. The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="99cdb-109">**表 1. 代理人として予定表にアクセスするための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="99cdb-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="99cdb-110">**目的**</span><span class="sxs-lookup"><span data-stu-id="99cdb-110">**If you want to…**</span></span>|<span data-ttu-id="99cdb-111">**使用する EWS マネージ API メソッド…**</span><span class="sxs-lookup"><span data-stu-id="99cdb-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="99cdb-112">**使用する EWS 操作…**</span><span class="sxs-lookup"><span data-stu-id="99cdb-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="99cdb-113">会議または予定を代理人として作成する</span><span class="sxs-lookup"><span data-stu-id="99cdb-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="99cdb-114">[Appointment.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx): [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の予定表フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="99cdb-114">[Appointment.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="99cdb-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合</span><span class="sxs-lookup"><span data-stu-id="99cdb-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="99cdb-116">複数の会議または予定を代理人として作成する</span><span class="sxs-lookup"><span data-stu-id="99cdb-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="99cdb-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="99cdb-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="99cdb-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="99cdb-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="99cdb-119">予定または会議を代理人として検索または検出する</span><span class="sxs-lookup"><span data-stu-id="99cdb-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="99cdb-120">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の予定表フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="99cdb-120">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="99cdb-121">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="99cdb-121">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="99cdb-122">予定または会議を代理人として取得する</span><span class="sxs-lookup"><span data-stu-id="99cdb-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="99cdb-123">Appointment.Bind</span><span class="sxs-lookup"><span data-stu-id="99cdb-123">Appointment.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="99cdb-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="99cdb-124">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="99cdb-125">予定または会議を代理人として更新する</span><span class="sxs-lookup"><span data-stu-id="99cdb-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="99cdb-126">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-126">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="99cdb-127">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-127">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="99cdb-128">予定または会議を代理人として削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="99cdb-129">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-129">[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="99cdb-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="99cdb-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="99cdb-131">この記事のコード例では、primary@contoso.com がメールボックス所有者です。</span><span class="sxs-lookup"><span data-stu-id="99cdb-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="99cdb-132">事前に必要なタスク</span><span class="sxs-lookup"><span data-stu-id="99cdb-132">Prerequisite tasks</span></span>
<span data-ttu-id="99cdb-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-133"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="99cdb-134">ユーザーが代理人としてメールボックス所有者の予定表フォルダーにアクセスするためには、そのユーザーは、メールボックス所有者の予定表フォルダーに、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)追加されていなければなりません。</span><span class="sxs-lookup"><span data-stu-id="99cdb-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="99cdb-135">代理人は、メールボックス所有者の予定表を更新するには、自身のアカウントにアタッチされたメールボックスが必要です。</span><span class="sxs-lookup"><span data-stu-id="99cdb-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="99cdb-136">代理人が会議出席依頼と応答だけを処理すればよい場合は、予定表フォルダーに代理人を追加し、既定の [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS マネージ API 列挙値または [DeliverMeetingRequests](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS 要素値 **DelegatesAndSendInformationToMe** を使用して、出席依頼を代理人に送信し、情報メッセージをメールボックス所有者に送信します。</span><span class="sxs-lookup"><span data-stu-id="99cdb-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="99cdb-137">こうすると、メールボックス所有者の受信トレイ フォルダーへのアクセス権を代理人に付与する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="99cdb-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="99cdb-138">EWS マネージ API を使用して会議または予定を代理人として作成する</span><span class="sxs-lookup"><span data-stu-id="99cdb-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="99cdb-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-139"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="99cdb-140">EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成できます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="99cdb-141">この例は、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="99cdb-141">This example shows how to use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="99cdb-142">この例では、**service** が代理人の有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、メールボックス所有者の予定表フォルダーに対する適切なアクセス許可が代理人に付与されいることを前提にしています。</span><span class="sxs-lookup"><span data-stu-id="99cdb-142">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="99cdb-143">アイテムの保存時には、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッド呼び出しでメールボックス所有者の予定表フォルダーを識別する必要があることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="99cdb-143">Note that when you save the item, the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="99cdb-144">メールボックス所有者の予定表フォルダーを指定しない場合、会議出席依頼はメールボックス所有者の予定表フォルダーではなく、代理人の予定表フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="99cdb-145">メールボックス所有者の予定表フォルダーは、2 つの方法で **Save** メソッド呼び出しに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="99cdb-146">メールボックス所有者の [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) と SMTP アドレスを使用して、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) オブジェクトの新しいインスタンスをインスタンス化することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="99cdb-146">We recommend that you instantiate a new instance of the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="99cdb-147">ただし、最初に予定表フォルダーに [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) してから、**Save** メソッド呼び出しでフォルダーの ID を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-147">However, you can also [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="99cdb-148">ただし、これにより追加の EWS 呼び出しが作成されることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="99cdb-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="99cdb-149">EWS を使用して会議または予定を代理人として作成する</span><span class="sxs-lookup"><span data-stu-id="99cdb-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="99cdb-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-150"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="99cdb-p107">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の予定表アイテムを作成できます。この例は、[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="99cdb-p107">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner. This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="99cdb-153">これは、**Save** メソッドを使用して[会議または予定を代理人として作成する](#bk_createewsma)場合に EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="99cdb-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="99cdb-154">簡潔にするために、次の例では SOAP ヘッダーが削除されています。</span><span class="sxs-lookup"><span data-stu-id="99cdb-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="99cdb-p108">サーバーは、[CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで **CreateItem** 要求に応答します。このメッセージには、会議が正常に作成されたことを示す [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値 **NoError** が含まれます。また、この応答には新しく作成された会議のアイテム ID も含まれます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-p108">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully. The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="99cdb-157">EWS マネージ API を使用して会議または予定を代理人として検索する</span><span class="sxs-lookup"><span data-stu-id="99cdb-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="99cdb-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-158"><a name="bk_searchewsma"> </a></span></span>

<span data-ttu-id="99cdb-159">会議を検索するには、メールボックス所有者の予定表フォルダーを指定するために、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターが含まれるいずれかの [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99cdb-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="99cdb-160">**FindItems** 呼び出しが ID を含む応答を返すと、ID と[暗黙的アクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して対象の会議を取得、更新、削除できます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="99cdb-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="99cdb-161">EWS を使用して会議または予定を代理人として検索する</span><span class="sxs-lookup"><span data-stu-id="99cdb-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="99cdb-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-162"><a name="bk_searchews"> </a></span></span>

<span data-ttu-id="99cdb-p109">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、検索条件のセットに一致する予定および会議を検索できます。この例は、[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、メールボックス所有者の予定表フォルダーの中で件名に "building" という単語が含まれる会議を検索する方法を示しています。 </span><span class="sxs-lookup"><span data-stu-id="99cdb-p109">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria. This example shows how to use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="99cdb-165">これは、**FindItem** メソッドを使用して[会議または予定を代理人として検索する](#bk_searchewsma)場合に EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="99cdb-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="99cdb-p110">サーバーは、[FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) メッセージで **FindItem** 要求に応答します。このメッセージには、検索が正常に完了したことを示す [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値 **NoError** が含まれます。この応答には、検索条件に一致する予定または会議の [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) が含まれます。この例では、検出された会議は 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="99cdb-p110">The server responds to the **FindItem** request with a [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully. The response contains a [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria. In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="99cdb-169">[ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="99cdb-169">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="99cdb-170">条件と一致する会議の **ItemId** が分かったので、**ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して、会議の取得、更新、削除を行えます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="99cdb-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="99cdb-171">EWS マネージ API を使用して予定表アイテムを代理人として取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="99cdb-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-172"><a name="bk_geteswma"> </a></span></span>

<span data-ttu-id="99cdb-173">EWS マネージ API を使用して、代理人アクセスを使用しない場合と同じ方法で、会議または予定を取得、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="99cdb-174">唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。</span><span class="sxs-lookup"><span data-stu-id="99cdb-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="99cdb-175">**Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の予定表フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="99cdb-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="99cdb-176">**表 2. 予定および会議を代理人として処理するための EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="99cdb-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="99cdb-177">**タスク**</span><span class="sxs-lookup"><span data-stu-id="99cdb-177">**Task**</span></span>|<span data-ttu-id="99cdb-178">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="99cdb-178">**EWS Managed API method**</span></span>|<span data-ttu-id="99cdb-179">**コード例**</span><span class="sxs-lookup"><span data-stu-id="99cdb-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="99cdb-180">予定または会議を取得する</span><span class="sxs-lookup"><span data-stu-id="99cdb-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="99cdb-181">Bind</span><span class="sxs-lookup"><span data-stu-id="99cdb-181">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="99cdb-182">EWS マネージ API を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="99cdb-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="99cdb-183">予定または会議を更新する</span><span class="sxs-lookup"><span data-stu-id="99cdb-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="99cdb-184">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-184">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="99cdb-185">EWS マネージ API を使用して会議を更新する</span><span class="sxs-lookup"><span data-stu-id="99cdb-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="99cdb-186">予定または会議を削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="99cdb-187">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-187">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="99cdb-188">EWS マネージ API を使用して会議を削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="99cdb-189">EWS を使用して予定表アイテムを代理人として取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="99cdb-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="99cdb-190"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="99cdb-191">EWS を使用して、代理人アクセスを使用しない場合と同じ方法で、会議または予定を取得、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="99cdb-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="99cdb-192">唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。</span><span class="sxs-lookup"><span data-stu-id="99cdb-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="99cdb-193">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の予定表フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="99cdb-193">The item ID included in the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="99cdb-194">**表 3. 予定および会議を代理人として処理するための EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="99cdb-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="99cdb-195">**タスク**</span><span class="sxs-lookup"><span data-stu-id="99cdb-195">**Task**</span></span>|<span data-ttu-id="99cdb-196">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="99cdb-196">**EWS operation**</span></span>|<span data-ttu-id="99cdb-197">**コード例**</span><span class="sxs-lookup"><span data-stu-id="99cdb-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="99cdb-198">予定または会議を取得する</span><span class="sxs-lookup"><span data-stu-id="99cdb-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="99cdb-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="99cdb-199">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="99cdb-200">EWS を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="99cdb-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="99cdb-201">予定または会議を更新する</span><span class="sxs-lookup"><span data-stu-id="99cdb-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="99cdb-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="99cdb-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="99cdb-203">EWS を使用して会議を更新する</span><span class="sxs-lookup"><span data-stu-id="99cdb-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="99cdb-204">予定または会議を削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="99cdb-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="99cdb-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99cdb-206">関連項目</span><span class="sxs-lookup"><span data-stu-id="99cdb-206">See also</span></span>

- [<span data-ttu-id="99cdb-207">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="99cdb-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="99cdb-208">Exchange で EWS を使用して代理人を追加および削除する</span><span class="sxs-lookup"><span data-stu-id="99cdb-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="99cdb-209">Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="99cdb-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="99cdb-210">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="99cdb-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

