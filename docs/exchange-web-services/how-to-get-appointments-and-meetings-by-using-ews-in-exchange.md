---
title: Exchange の EWS を使用して予定と会議を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bae582a-8cb3-4e77-be2a-7e107fad26fe
description: EWS マネージ API または Exchange の EWS を使用して、予定と会議を取得する方法を説明します。
ms.openlocfilehash: c78d70ca2266bd192b82f644d902ad8c958d2d4a
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353694"
---
# <a name="get-appointments-and-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="fae71-103">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="fae71-103">How to: Get appointments and meetings by using EWS in Exchange</span></span>

<span data-ttu-id="fae71-104">EWS マネージ API または Exchange の EWS を使用して、予定と会議を取得する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="fae71-104">Learn how to get appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fae71-105">[CalendarFolder.FindAppointments](http://msdn.microsoft.com/ja-JP/library/dd636179%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS 操作を使用して、予定表フォルダーから予定と会議を取得できます。</span><span class="sxs-lookup"><span data-stu-id="fae71-105">You can retrieve appointments and meetings from a calendar folder by using the [CalendarFolder.FindAppointmentshttp://msdn.microsoft.com/en-us/library/dd636179(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd636179%28v=exchg.80%29.aspx) EWS Managed API method or the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation.</span></span> 
  
## <a name="get-appointments-by-using-the-ews-managed-api"></a><span data-ttu-id="fae71-106">EWS マネージ API を使用して、予定を取得する</span><span class="sxs-lookup"><span data-stu-id="fae71-106">Get appointments by using the EWS Managed API</span></span>
<span data-ttu-id="fae71-107"><a name="bk_retrieveappsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fae71-107"></span></span>

<span data-ttu-id="fae71-108">次のコード例は、EWS マネージ API を使用して、指定した開始時刻から終了時刻までの範囲にあるユーザーの予定を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fae71-108">The following code example shows how to use the EWS Managed API to retrieve a user's appointments that fall between a specified start and end time.</span></span>
  
```cs
       // Initialize values for the start and end times, and the number of appointments to retrieve.
            DateTime startDate = DateTime.Now;
            DateTime endDate = startDate.AddDays(30);
            const int NUM_APPTS = 5;
            // Initialize the calendar folder object with only the folder ID. 
            CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
            // Set the start and end time and number of appointments to retrieve.
            CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
            // Limit the properties returned to the appointment's subject, start time, and end time.
            cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
            // Retrieve a collection of appointments by using the calendar view.
            FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
            Console.WriteLine("\nThe first " + NUM_APPTS + " appointments on your calendar from " + startDate.Date.ToShortDateString() + 
                              " to " + endDate.Date.ToShortDateString() + " are: \n");
            
            foreach (Appointment a in appointments)
            {
                Console.Write("Subject: " + a.Subject.ToString() + " ");
                Console.Write("Start: " + a.Start.ToString() + " ");
                Console.Write("End: " + a.End.ToString());
                Console.WriteLine();
            }

```

<br/>

<span data-ttu-id="fae71-109">以下に示すのは、コード例からの出力です。</span><span class="sxs-lookup"><span data-stu-id="fae71-109">The following is the output from the code example.</span></span>
  
```text
The first five appointments on your calendar from 8/21/2013 to 9/20/2013 are: 
  
Subject: Contoso devs team meeting Start: 8/21/2013 12:30:00 PM End: 8/21/2013 1:00:00 PM
  
Subject: Daily status meeting Start: 8/21/2013 1:00:00 PM End: 8/21/2013 2:00:00 PM
  
Subject: Lunch with sales team Start: 8/21/2013 2:30:00 PM End: 8/21/2013 3:30:00 PM
  
Subject: Tennis at the club Start: 8/22/2013 11:00:00 AM End: 8/22/2013 12:00:00 PM
  
Subject: Online training webcast: 8/22/2013 2:00:00 PM End: 8/22/2013 3:00:00 PM
```

## <a name="get-appointments-by-using-ews"></a><span data-ttu-id="fae71-110">EWS を使用して、予定を取得する</span><span class="sxs-lookup"><span data-stu-id="fae71-110">Get appointments by using EWS</span></span>
<span data-ttu-id="fae71-111"><a name="bk_xml"> </a></span><span class="sxs-lookup"><span data-stu-id="fae71-111"></span></span>

<span data-ttu-id="fae71-112">次の XML は [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作のフォルダー ID を返す [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作の要求を示します。</span><span class="sxs-lookup"><span data-stu-id="fae71-112">The following XML shows a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request to return a folder ID for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)  operation.</span></span> 
  
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
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="fae71-p101">次の XML は **GetFolder** 応答を示します。**FolderID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="fae71-p101">The following XML shows the **GetFolder** response. Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:CalendarFolder>
              <t:FolderId Id="AAMk" ChangeKey="AgAA" />
            </t:CalendarFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<br/>

<span data-ttu-id="fae71-p102">次の XML は、要求された予定を返すために使用される **FindItem** 要求を示します。**FolderID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="fae71-p102">The following XML shows the **FindItem** request used to return the requested appointments. Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-08-21T17:30:24.127Z" EndDate="2013-09-20T17:30:24.127Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAMk" ChangeKey="AgAA" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="fae71-p103">次の XML は **FindItem** 応答を示します。**ItemID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="fae71-p103">The following XML shows the **FindItem** response. Note that the **ItemID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="33" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Contoso devs team meeting</t:Subject>
                <t:Start>2013-08-21T19:30:00Z</t:Start>
                <t:End>2013-08-21T20:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Daily status meeting</t:Subject>
                <t:Start>2013-08-21T20:00:00Z</t:Start>
                <t:End>2013-08-21T21:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Lunch with sales team</t:Subject>
                <t:Start>2013-08-21T21:30:00Z</t:Start>
                <t:End>2013-08-21T22:30:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Tennis at the club</t:Subject>
                <t:Start>2013-08-22T18:00:00Z</t:Start>
                <t:End>2013-08-22T19:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAA" />
                <t:Subject>Online training webcast</t:Subject>
                <t:Start>2013-08-22T21:00:00Z</t:Start>
                <t:End>2013-08-22T22:00:00Z</t:End>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="recurring-meetings-and-the-calendar-view"></a><span data-ttu-id="fae71-119">定期的な会議および予定表の表示</span><span class="sxs-lookup"><span data-stu-id="fae71-119">Recurring meetings and the calendar view</span></span>
<span data-ttu-id="fae71-120"><a name="bk_recurring"> </a></span><span class="sxs-lookup"><span data-stu-id="fae71-120"></span></span>

<span data-ttu-id="fae71-121">繰り返し連続で発生するアイテムや、繰り返し連続で発生するアイテムの例外は、メールボックス内の実際のアイテムではなく、定期的なマスターへの添付物として内部に格納されるため、予定表フォルダーはメールボックス内の他のフォルダーとは少し異なります。</span><span class="sxs-lookup"><span data-stu-id="fae71-121">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master. Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view. To learn more about retrieving appointments and calendar views, see How to: Get appointments and meetings by using EWS in Exchange.</span></span> <span data-ttu-id="fae71-122">つまり、[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)、または EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作など、EWS マネージ API **FindItems** メソッドのいずれかを使用して、**開始**値と**終了**値のセット間の値を返す EWS 要求を作成することができますが、EWS は各予定表アイテムの添付テーブルを確認して、例外や発生アイテムを検索することはしません。</span><span class="sxs-lookup"><span data-stu-id="fae71-122">The calendar folder is a little different from other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master. This means that although you can create an EWS request that returns values between a set of **start** and **end** values by using one of the EWS Managed API **FindItems** overload methods, such as [ExchangeService.FindItemshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or the EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, EWS would not look through the attachment table of every calendar item to find exceptions and occurrences.</span></span> 
  
<span data-ttu-id="fae71-123">むしろ、本当に実行したいことは、[CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) オブジェクトを使用して、2 つの SQL テーブルのユニオン上に *Dataview* を適用する操作に類似する操作です。</span><span class="sxs-lookup"><span data-stu-id="fae71-123">Instead, what you really want to do is something akin to applying a  *Dataview*  onto a union of two SQL tables, using a [CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="fae71-124">パフォーマンス上の理由から、[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) プロパティを使用して、返すことを望む予定や会議の件数や望みのプロパティを指示し、応答のサイズを制限することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="fae71-124">Instead, what you really want to do is something akin to applying a Dataview onto a union of two SQL tables, using a  CalendarView http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview(v=exchg.80).aspx  object. Note that for performance reasons, we recommend that you use the  PropertySet http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset(v=exchg.80).aspx  property to limit the size of the response by indicating the number of appointments or meetings you want returned, as well as the specific properties you want.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fae71-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="fae71-125">See also</span></span>
<span data-ttu-id="fae71-126"><a name="bk_additional"> </a></span><span class="sxs-lookup"><span data-stu-id="fae71-126"></span></span>

- [<span data-ttu-id="fae71-127">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="fae71-127">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)   
- [<span data-ttu-id="fae71-128">Exchange 2013 の EWS を使用して予定と会議を作成する</span><span class="sxs-lookup"><span data-stu-id="fae71-128">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="fae71-129">Exchange の EWS を使用して予定と会議を更新する</span><span class="sxs-lookup"><span data-stu-id="fae71-129">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="fae71-130">Exchange で EWS を使用して、予定を削除し、会議をキャンセルする</span><span class="sxs-lookup"><span data-stu-id="fae71-130">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="fae71-131">Exchange 用の Web サービス クライアントの開発</span><span class="sxs-lookup"><span data-stu-id="fae71-131">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

