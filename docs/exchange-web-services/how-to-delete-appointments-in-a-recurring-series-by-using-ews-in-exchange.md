---
title: Exchange EWS を使用して一連の定期的な予定を削除します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム内の予定を削除する方法を説明します。
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758960"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="6f11e-103">Exchange EWS を使用して一連の定期的な予定を削除します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="6f11e-104">Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム内の予定を削除する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6f11e-105">予定または会議の系列または系列内の 1 つのインスタンスを削除するのには、EWS のマネージ API または EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="6f11e-106">シリーズ全体を削除するのにを使用するプロセスは、本質的には、1 つのアイテムのみを削除するのにを使用するプロセスと同じです。</span><span class="sxs-lookup"><span data-stu-id="6f11e-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="6f11e-107">EWS のマネージ API と同じ方法または[単独の予定または会議を削除](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)するために使用、EWS の操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6f11e-108">違いは、メソッドまたは操作に含まれる項目 id です。</span><span class="sxs-lookup"><span data-stu-id="6f11e-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="6f11e-109">どのように両方のシナリオは、同じを見ていきましょう。</span><span class="sxs-lookup"><span data-stu-id="6f11e-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="6f11e-p102">定期的なアイテムや、定期的なアイテム中の単独のアイテムのみを削除する場合、削除対象のアイテムまたは定期的なアイテムを見つけ、その後、適切なメソッドまたは操作を呼び出して削除します。あらゆる種類の予定を簡単に削除できますが、出席者や開催者については最新の情報を保持し、削除対象ユーザーが開催した会議はキャンセルし、対象ユーザーが開催しなかった会議は辞退することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6f11e-p102">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it. While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="6f11e-112">その方法はシナリオ別でしょうか。</span><span class="sxs-lookup"><span data-stu-id="6f11e-112">So how are the scenarios different?</span></span> <span data-ttu-id="6f11e-113">メソッド (EWS のマネージ API) またはアイテムの ID を呼び出すために使用する[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)のオブジェクトの概要に記載 (EWS) の操作の要求。</span><span class="sxs-lookup"><span data-stu-id="6f11e-113">It's all about the [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="6f11e-114">シリーズ全体を削除するには、マスターの定期的な**予定**のオブジェクトまたは要素 ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f11e-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="6f11e-115">1 つのオカレンスを削除するには、発生する**予定**のオブジェクトまたは要素 ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f11e-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="6f11e-116">EWS マネージ API を使用して定期的な予定を削除する</span><span class="sxs-lookup"><span data-stu-id="6f11e-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="6f11e-117">次の使用例は、認証済み Exchange サーバーおよび**サービス**をという名前の[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを取得することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="6f11e-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="6f11e-118">_RecurringItem_パラメーターは、1 回または定期的なマスターのいずれかの**予定**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6f11e-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="6f11e-119">_DeleteEntireSeries_パラメーターでは、 _recurringItem_の一部になっているデータ系列全体を削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

<span data-ttu-id="6f11e-120">次の使用例を使用するには、[発生または定期的なマスターのいずれかにバインド](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)する必要があるし、**予定**オブジェクトをメソッドに渡します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="6f11e-121">予定を[予定表ビュー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx)クラスを使用してアクセスすると、結果として得られるアイテムが、1 つのすべての出現に留意してください。</span><span class="sxs-lookup"><span data-stu-id="6f11e-121">Keep in mind that if you access appointments by using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="6f11e-122">逆に、 [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx)クラスを使用する場合、結果として得られる項目は、すべての定期的なマスターになります。</span><span class="sxs-lookup"><span data-stu-id="6f11e-122">Conversely, if you use the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="6f11e-123">EWS を使用して定期的な予定を削除する</span><span class="sxs-lookup"><span data-stu-id="6f11e-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="6f11e-124">[単独の会議を削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)ことでは、EWS を使用して定期的な系列を削除します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6f11e-125">実際には、SOAP 要求は、同じ形式を実行します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="6f11e-126">もう一度、キーは、要求で使用されている項目の ID です。</span><span class="sxs-lookup"><span data-stu-id="6f11e-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="6f11e-127">品目 ID は、定期的なマスターに対応して、データ系列全体が削除されます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="6f11e-128">項目 ID は、1 回の発生に対応して、そのアイテムのみが削除されます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6f11e-129">次のコードの例では**アイテム Id**、**変更キー**、および**RecurringMasterId**の属性は読みやすさの短縮します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="6f11e-130">この例では、 [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx)要素を使用して[CreateItem 操作](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)を使用して、ユーザーは開催者の会議をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="6f11e-130">This example uses the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="6f11e-131">[ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx)要素の値は、取り消すには、アイテムを指定し、定期的なマスター、または 1 つの項目 ID を指定できます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-131">The value of the [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f11e-132">この例では、 [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx)要素を使用して**CreateItem 操作**を使用して、対象のユーザーは開催者の会議を辞退します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-132">This example uses the **CreateItem operation** with a [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="6f11e-133">**ReferenceItemId**要素の値がこれを拒否すると、アイテムを指定する前の例のようにと、定期的なマスター、または 1 つの項目 ID を指定できます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f11e-134">この例では、 [DeleteItem の操作](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)を使用していない参加者との予定の 1 つのアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-134">This example uses the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="6f11e-135">発生を削除するのには、定期的なマスターの項目の ID と、出現する位置のインデックスが作成される[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx)要素によって指定されます。</span><span class="sxs-lookup"><span data-stu-id="6f11e-135">The occurrence to delete is specified by the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
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
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f11e-136">ように、出現する位置の項目の ID が含まれている[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)要素を使用して**OccurrenceItemId**要素を置き換えることによって同じ結果を得ることができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6f11e-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="6f11e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f11e-137">See also</span></span>


- [<span data-ttu-id="6f11e-138">定期的なパターンと EWS</span><span class="sxs-lookup"><span data-stu-id="6f11e-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="6f11e-139">Exchange で EWS を使用して、定期的にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="6f11e-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="6f11e-140">Exchange EWS を使用して定期的な系列を作成します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="6f11e-141">EWS を使用して一連の定期的な更新プログラム</span><span class="sxs-lookup"><span data-stu-id="6f11e-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="6f11e-142">Exchange EWS を使用して一連の定期的な更新プログラム</span><span class="sxs-lookup"><span data-stu-id="6f11e-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="6f11e-143">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="6f11e-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="6f11e-144">Exchange 2013 の EWS を使用して予定および会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="6f11e-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="6f11e-145">予定を削除して、Exchange で EWS を使用して会議をキャンセル</span><span class="sxs-lookup"><span data-stu-id="6f11e-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

