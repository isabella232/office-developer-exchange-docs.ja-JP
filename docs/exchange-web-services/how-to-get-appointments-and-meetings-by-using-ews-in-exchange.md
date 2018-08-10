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
# <a name="get-appointments-and-meetings-by-using-ews-in-exchange"></a>Exchange の EWS を使用して予定と会議を取得する

EWS マネージ API または Exchange の EWS を使用して、予定と会議を取得する方法を説明します。
  
[CalendarFolder.FindAppointments](http://msdn.microsoft.com/ja-JP/library/dd636179%28v=exchg.80%29.aspx) EWS マネージ API メソッド、または [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS 操作を使用して、予定表フォルダーから予定と会議を取得できます。 
  
## <a name="get-appointments-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、予定を取得する
<a name="bk_retrieveappsEWSMA"> </a>

次のコード例は、EWS マネージ API を使用して、指定した開始時刻から終了時刻までの範囲にあるユーザーの予定を取得する方法を示しています。
  
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

以下に示すのは、コード例からの出力です。
  
```text
The first five appointments on your calendar from 8/21/2013 to 9/20/2013 are: 
  
Subject: Contoso devs team meeting Start: 8/21/2013 12:30:00 PM End: 8/21/2013 1:00:00 PM
  
Subject: Daily status meeting Start: 8/21/2013 1:00:00 PM End: 8/21/2013 2:00:00 PM
  
Subject: Lunch with sales team Start: 8/21/2013 2:30:00 PM End: 8/21/2013 3:30:00 PM
  
Subject: Tennis at the club Start: 8/22/2013 11:00:00 AM End: 8/22/2013 12:00:00 PM
  
Subject: Online training webcast: 8/22/2013 2:00:00 PM End: 8/22/2013 3:00:00 PM
```

## <a name="get-appointments-by-using-ews"></a>EWS を使用して、予定を取得する
<a name="bk_xml"> </a>

次の XML は [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作のフォルダー ID を返す [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作の要求を示します。 
  
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

次の XML は **GetFolder** 応答を示します。**FolderID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。 
  
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

次の XML は、要求された予定を返すために使用される **FindItem** 要求を示します。**FolderID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。 
  
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

次の XML は **FindItem** 応答を示します。**ItemID** 属性と **ChangeKey** 属性は読みやすいように短縮されていますので、ご注意ください。 
  
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

## <a name="recurring-meetings-and-the-calendar-view"></a>定期的な会議および予定表の表示
<a name="bk_recurring"> </a>

繰り返し連続で発生するアイテムや、繰り返し連続で発生するアイテムの例外は、メールボックス内の実際のアイテムではなく、定期的なマスターへの添付物として内部に格納されるため、予定表フォルダーはメールボックス内の他のフォルダーとは少し異なります。 つまり、[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)、または EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作など、EWS マネージ API **FindItems** メソッドのいずれかを使用して、**開始**値と**終了**値のセット間の値を返す EWS 要求を作成することができますが、EWS は各予定表アイテムの添付テーブルを確認して、例外や発生アイテムを検索することはしません。 
  
むしろ、本当に実行したいことは、[CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) オブジェクトを使用して、2 つの SQL テーブルのユニオン上に *Dataview* を適用する操作に類似する操作です。 パフォーマンス上の理由から、[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) プロパティを使用して、返すことを望む予定や会議の件数や望みのプロパティを指示し、応答のサイズを制限することをお勧めします。 
  
## <a name="see-also"></a>関連項目
<a name="bk_additional"> </a>

- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)   
- [Exchange 2013 の EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [Exchange の EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [Exchange で EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [Exchange 用の Web サービス クライアントの開発](develop-web-service-clients-for-exchange.md)
    

