---
title: Exchange EWS を使用して一連の定期的な更新プログラム
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c922072f-ce33-4bff-97b0-1c1d0f9b880d
description: Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム全体を一度に更新する方法を説明します。
ms.openlocfilehash: 03f414845674bfcacca62ef96fdb84f8b8823920
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759056"
---
# <a name="update-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="e5ccf-103">Exchange EWS を使用して一連の定期的な更新プログラム</span><span class="sxs-lookup"><span data-stu-id="e5ccf-103">Update a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="e5ccf-104">Exchange の EWS マネージ API または EWS を使用して、定期的なアイテム全体を一度に更新する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-104">Learn how to update an entire recurring series at once by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="e5ccf-105">系列全体を更新するか、 [1 回を更新](how-to-update-a-recurring-series-by-using-ews.md)することによって定期的な系列を更新するのには、EWS のマネージ API または EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-105">You can use the EWS Managed API or EWS to update a recurring series by either updating the entire series, or by [updating a single occurrence](how-to-update-a-recurring-series-by-using-ews.md).</span></span> <span data-ttu-id="e5ccf-106">この資料では、データ系列全体を一度に更新する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-106">In this article we'll discuss how to update the entire series at once.</span></span>
  
<span data-ttu-id="e5ccf-107">一般に、定期的な一連の更新は、 [1 つの予定を変更](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)するのには非常に似ています。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-107">In general, updating a recurring series is very similar to [modifying a single appointment](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="e5ccf-108">同じメソッドと、操作を使用するが、一連の定期的なマスターの項目の ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-108">You use the same methods and operations, but you use the item ID of the series' recurring master.</span></span> <span data-ttu-id="e5ccf-109">場合によっては可能性がありますを開始すると、定期的なマスターと[マスターの定期的なアイテムの ID を検索](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-109">In some cases you might not start with the recurring master, and you might need to [find the item ID for the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="e5ccf-110">ただし、定期的に更新する際に考慮すべき主な違いがある: 定期的なパターンを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-110">However, there is one key difference to consider when updating a recurring series: updating the recurrence pattern.</span></span> <span data-ttu-id="e5ccf-111">定期的なパターンを更新するだけでは定期的なマスター、およびパターンへの変更は追加したり、アイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-111">Updating the recurrence pattern is only possible with the recurring master, and changes to the pattern can add or remove occurrences.</span></span> <span data-ttu-id="e5ccf-112">定期的なパターンを再評価すると、現在の値よりも後の日付に[Recurrence.EndDate](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx)プロパティを変更する場合や別の箇所を追加することがありますなど。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-112">For example, if you modify the [Recurrence.EndDate](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) property to a date later than its current value, the recurrence pattern is reevaluated, and additional occurrences might be added.</span></span> 
  
## <a name="modify-all-occurrences-in-a-series-by-using-the-ews-managed-api"></a><span data-ttu-id="e5ccf-113">EWS マネージ API を使用して定期的なアイテム内のアイテムをすべて変更する</span><span class="sxs-lookup"><span data-stu-id="e5ccf-113">Modify all occurrences in a series by using the EWS Managed API</span></span>

<span data-ttu-id="e5ccf-114">定期的なアイテム内のアイテムをすべて変更するには、次にようにします。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-114">To modify all occurrences in a series you:</span></span>
  
1. <span data-ttu-id="e5ccf-115">定期的なマスターに、 [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)メソッドまたは[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx)メソッドを使用して、一連の定期的なマスターにバインドします。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-115">Bind to the recurring master for the series by using the [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) or [Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) method on a recurring master.</span></span> 
    
2. <span data-ttu-id="e5ccf-116">定期的なマスター[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-116">Update the properties on the recurring master [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object.</span></span> 
    
3. <span data-ttu-id="e5ccf-117">[Appointment.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)メソッドを使用して定期的なマスターに変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-117">Save the changes to the recurring master by using the [Appointment.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="e5ccf-118">、出席者を追加する次の例は、場所を変更する定期的な系列を更新し、定期的なパターンを変更します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-118">The following example updates a recurring series to change the location, add an attendee, and modify the recurrence pattern.</span></span> <span data-ttu-id="e5ccf-119">次の使用例では、[資格情報](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx)と[Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx)のプロパティで有効な値を持つ_サービス_のパラメーターに渡された[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトが初期化されたことを前提としています。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-119">This example assumes that the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="e5ccf-120">_定期的な予定_のパラメーターは、発生または更新する、一連の定期的なマスターのいずれかにバインドされている**予定**オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-120">The  _recurringAppointment_ parameter is an **Appointment** object bound to either an occurrence or the recurring master for the series to be updated.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
public static bool UpdateRecurringSeries(ExchangeService service, Appointment recurringAppointment)
{
    Appointment recurringMaster = null;
    // If the item is a single appointment, fail.
    if (recurringAppointment.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringAppointment.AppointmentType != AppointmentType.RecurringMaster)
    {
        // If an occurrence was passed in, bind to the master.
        try
        {
            // This method results in a call to EWS.
            recurringMaster = Appointment.BindToRecurringMaster(service, recurringAppointment.Id);
        }
        catch (Exception ex)
        {
            Console.WriteLine("Couldn't bind to master: {0}", ex.Message);
            return false;
        }
    }
    else
    {
        // Bind to the appointment to load all properties.
        // This method results in a call to EWS.
        recurringMaster = Appointment.Bind(service, recurringAppointment.Id);
    }
    // Basic updates. These kinds of updates are the same
    // as if you were updating a single appointment.
    // Update the location. All occurrences will update to this new location.
    recurringMaster.Location = "Conference Room 2";
    // Add an attendee.
    Attendee newAttendee = new Attendee("sadie@contoso.com");
    recurringMaster.RequiredAttendees.Add(newAttendee);
    // Changes to the recurrence. This is only applicable to a recurring
    // master.
    // If the series has an end date, extend the series to add two more occurrences.
    if (recurringMaster.Recurrence.HasEnd)
    {
        // NumberOfOccurrences is only set if the user created the
        // appointment with a set number of occurrences.
        // Otherwise, there's a start and end date.
        if (recurringMaster.Recurrence.NumberOfOccurrences != null)
        {
            recurringMaster.Recurrence.NumberOfOccurrences += 2;
        }
        else
        {
            // This is a bit more complicated if you want to add two more
            // occurrences. You need to calculate a new end date.
            Type recurrenceType = recurringMaster.Recurrence.GetType();
            switch (recurrenceType.Name)
            {
                case "DailyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddDays(2);
                    break;
                case "WeeklyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddDays(14);
                    break;
                case "YearlyPattern":
                    recurringMaster.Recurrence.EndDate =
                        recurringMaster.Recurrence.EndDate.Value.AddYears(2);
                    break;
                default:
                    // Do nothing here. There are other recurrence
                    // types but for simplicity, these aren't covered.
                    break;
            }
        }
    }
    else
    {
        // If it has no end, set an end date to 2 weeks from today.
        recurringMaster.Recurrence.EndDate = DateTime.Now.AddDays(14);
    }
    // Update the series.
    try
    {
        // This method results in a call to EWS.
        recurringMaster.Update(ConflictResolutionMode.AutoResolve);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating series: {0}", ex.Message);
        return false;
    }
    return true;
}
```

## <a name="modify-all-occurrences-in-a-series-by-using-ews"></a><span data-ttu-id="e5ccf-121">EWS を使用して定期的なアイテム内のアイテムをすべて変更する</span><span class="sxs-lookup"><span data-stu-id="e5ccf-121">Modify all occurrences in a series by using EWS</span></span>

<span data-ttu-id="e5ccf-122">系列内のすべての出現箇所を変更するには、 [UpdateItem 操作](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)を使用して、要求内の[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)で定期的なマスターの項目 ID を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-122">To modify all occurrences in a series, you need to use the [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) with the item ID of the recurring master in the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element in the request.</span></span> <span data-ttu-id="e5ccf-123">要求の構造は、1 つの予定を更新する要求と同じです。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-123">The structure of the request is the same as a request to update a single appointment.</span></span> 
  
<span data-ttu-id="e5ccf-124">次の例では、定期的なアイテムが次のように更新されます。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-124">The following example updates the recurring series in the following ways:</span></span>
  
- <span data-ttu-id="e5ccf-125">[Location](http://msdn.microsoft.com/library/3fcf7133-ae1c-47b4-a187-660045f71df0%28Office.15%29.aspx)要素を設定することにより、一連の場所を更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-125">Updates the location of the series by setting the [Location](http://msdn.microsoft.com/library/3fcf7133-ae1c-47b4-a187-660045f71df0%28Office.15%29.aspx) element.</span></span> 
    
- <span data-ttu-id="e5ccf-126">[RequiredAttendees](http://msdn.microsoft.com/library/422f8d44-b0eb-49ca-af0f-0e22b54c78d2%28Office.15%29.aspx)要素を設定することで、出席者を更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-126">Updates the attendees by setting the [RequiredAttendees](http://msdn.microsoft.com/library/422f8d44-b0eb-49ca-af0f-0e22b54c78d2%28Office.15%29.aspx) element.</span></span> 
    
- <span data-ttu-id="e5ccf-127">[(RecurrenceType) の繰り返し](http://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx)要素を設定することにより、定期的なアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-127">Updates the recurrence by setting the [Recurrence (RecurrenceType)](http://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) element.</span></span> 
    
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>Conference Room 2</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>mack@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie Daniels</t:Name>
                      <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Recurrence" />
              <t:CalendarItem>
                <t:Recurrence>
                  <t:WeeklyRecurrence>
                    <t:Interval>1</t:Interval>
                    <t:DaysOfWeek>Tuesday</t:DaysOfWeek>
                  </t:WeeklyRecurrence>
                  <t:EndDateRecurrence>
                    <t:StartDate>2014-05-06</t:StartDate>
                    <t:EndDate>2014-06-22-04:00</t:EndDate>
                  </t:EndDateRecurrence>
                </t:Recurrence>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:MeetingTimeZone" />
              <t:CalendarItem>
                <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e5ccf-128">**NoError**更新が正常に完了したことを示す値を持つ[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)の要素を含む[UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx)要素を使用して、サーバーが応答します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-128">The server responds with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) element that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element with a value of **NoError**, which indicates that the update was successful.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e5ccf-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5ccf-129">See also</span></span>


- [<span data-ttu-id="e5ccf-130">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="e5ccf-130">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="e5ccf-131">定期的なパターンと EWS</span><span class="sxs-lookup"><span data-stu-id="e5ccf-131">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="e5ccf-132">Exchange EWS を使用して予定および会議を更新します。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-132">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="e5ccf-133">EWS を使用して一連の定期的な更新プログラム</span><span class="sxs-lookup"><span data-stu-id="e5ccf-133">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="e5ccf-134">Exchange で EWS を使用して、定期的にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="e5ccf-134">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    

