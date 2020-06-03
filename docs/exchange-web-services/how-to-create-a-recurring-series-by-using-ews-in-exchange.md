---
title: Exchange で EWS を使用して、定期的なアイテムを作成する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 88ed6e87-25f7-4a54-83fa-d757a0ff2528
description: Exchange で EWS マネージ API または EWS を使用して、定期的な会議を作成する方法について説明します。
ms.openlocfilehash: 1d04bd48c56a1a0e94eb1368166f776b3dfeb23a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456872"
---
# <a name="create-a-recurring-series-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、定期的なアイテムを作成する

Exchange で EWS マネージ API または EWS を使用して、定期的な会議を作成する方法について説明します。
  
定期的な予定または会議の作成は、[単独の予定または会議](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)を作成する場合とあまり違いはありません。 必要なのは、追加の定期的なスケジュールに関連するいくつかのプロパティに値を割り当てるだけです。 これらは、[ExchangeService.Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトの [Recurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) オブジェクトに設定されるか (EWS マネージ API を使用している場合)、または [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 要素の [Recurrence](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) 子要素に設定されます (EWS を使用している場合)。 単独の会議ではなく、定期的なアイテムを作成する場合に考慮すべき点は、作成する予定表アイテムが一連の定期的な予定のマスターであることです。 プロパティの数は定期的な予定のマスターにのみ設定されます。これらのプロパティは、一連の個々のインスタンスを検索、変更、削除するのに役立ちます。 このため、定期的なアイテムを作成する場合には、定期的な予定のマスターの ID の追跡に役立つ可能性があります。 
  
**表 1. 定期的な予定のマスターの予定表アイテムに設定されているプロパティ**

|**EWS マネージ API クラスまたはプロパティ**|**EWS XML 要素**|**説明**|
|:-----|:-----|:-----|
|[Recurrence クラス](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) <br/> **Recurrence** クラスは、[IntervalPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx)、[RelativeYearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx)、[YearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) のいずれかの派生パターン クラスの基本クラスです。  <br/> |[Recurrence (RecurrenceType)](https://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) <br/> |定期的なパターン (毎日、毎週、毎月など)、開始日と終了日、回数など、定期的なアイテムに関連する情報が含まれます。  <br/> |
|[FirstOccurrence プロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) <br/> |[FirstOccurrence](https://msdn.microsoft.com/library/d6748860-ce0d-4d2e-b7e4-9ed834f1e45a%28Office.15%29.aspx) <br/> |開始時刻と終了時刻、および定期的に発生する会議の最初の会議のアイテム ID が含まれます。  <br/> |
|[LastOccurrence プロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) <br/> |[LastOccurrence](https://msdn.microsoft.com/library/c9ef0fcb-4265-4e60-9986-fff0f211d00b%28Office.15%29.aspx) <br/> |開始時刻と終了時刻、および定期的に発生する会議の最後の会議のアイテム ID が含まれます。  <br/> |
|[ModifiedOccurrences プロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) <br/> |[ModifiedOccurrences](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) <br/> |定期的に発生する会議の中で元の定期的なパターンから変更されている、すべての会議のセットが含まれます。  <br/> |
|[DeletedOccurrences プロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) <br/> |[DeletedOccurrences](https://msdn.microsoft.com/library/736fb305-9528-4be8-ad37-65d7556edbf2%28Office.15%29.aspx) <br/> |定期的に発生する会議の中で元の定期的なパターンから削除された、すべての会議のセットが含まれます。  <br/> |
   
会議は基本的には参加者を含む予定であるため、この記事のコード例では定期的な会議を作成する方法を示します。定期的な予定を作成する場合は、コード例を変更して参加者に関連するコードを削除します。
  
## <a name="create-a-recurring-meeting-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的な会議を作成する
<a name="bk_CreateMtgEWSMA"> </a>

次のコード例は、定期的な会議を作成する方法を示しています。 最初に、会議の作成に使用する [Appointment オブジェクト](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)に値を設定します。次に、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して、定期的なアイテムを予定表フォルダーに保存し、出席者に会議出席依頼を送信します。 最後に、[Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) メソッドを使用して、作成した定期的なアイテムの、定期的な予定のマスターに設定した値を確認します。 
  
この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 この例のメソッドでは、定期的なアイテムの定期的な予定のマスターの[アイテム ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) が返されます。 
  
```cs
public static ItemId CreateARecurringMeeting(ExchangeService service)
{        Appointment recurrMeeting = new Appointment(service);
        // Set the properties you need to create a meeting.
        recurrMeeting.Subject = "Weekly Update Meeting";
        recurrMeeting.Body = "Come hear about how the project is coming along!";
        recurrMeeting.Start = DateTime.Now.AddDays(1);
        recurrMeeting.End = recurrMeeting.Start.AddHours(1);
        recurrMeeting.Location = "Contoso Main Gallery";
        recurrMeeting.RequiredAttendees.Add("Mack@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Sadie@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Magdalena@contoso.com"); recurrMeeting.ReminderMinutesBeforeStart = 30;
             
        DayOfTheWeek[] dow = new DayOfTheWeek[] { (DayOfTheWeek)recurrMeeting.Start.DayOfWeek };
        // The following are the recurrence-specific properties for the meeting.
        recurrMeeting.Recurrence = new Recurrence.WeeklyPattern(recurrMeeting.Start.Date, 1, dow);
        recurrMeeting.Recurrence.StartDate = recurrMeeting.Start.Date;
        recurrMeeting.Recurrence.NumberOfOccurrences = 10;
        // This method results in in a CreateItem call to EWS.
        recurrMeeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
        // Retrieve the meeting subject and the properties that are set on a recurring master when a recurring series is created.
        recurrMeeting = Appointment.Bind(service, recurrMeeting.Id, new PropertySet(AppointmentSchema.Subject,
                                                                                    AppointmentSchema.AppointmentType, 
                                                                                    AppointmentSchema.Recurrence, 
                                                                                    AppointmentSchema.FirstOccurrence,
                                                                                    AppointmentSchema.LastOccurrence,
                                                                                    AppointmentSchema.ModifiedOccurrences,
                                                                                    AppointmentSchema.DeletedOccurrences));
        // Print out the recurring master properties.
        Console.WriteLine("\nAppointment created: " + recurrMeeting.Subject);
        Console.WriteLine("Appointment Type: {0}\n", recurrMeeting.AppointmentType);
        Console.WriteLine("These property values are always null unless the item is a recurring master:\n");
        Console.WriteLine("\tRecurrence pattern: {0}", recurrMeeting.Recurrence.ToString());
        Console.WriteLine("\tRecurring series start Date: {0}", recurrMeeting.Recurrence.StartDate.ToString());
        Console.WriteLine("\tRecurring series end Date: {0}", 
                        recurrMeeting.Recurrence.EndDate == null ? "Null" : recurrMeeting.Recurrence.EndDate.ToString());
        Console.WriteLine("\tHas end: {0}", recurrMeeting.Recurrence.HasEnd.ToString());
        Console.WriteLine("\tNumber of occurrances: {0}", recurrMeeting.Recurrence.NumberOfOccurrences);
        Console.WriteLine("\tLast 24 characters of the first occurrence's item ID:\t {0}", 
                        recurrMeeting.FirstOccurrence.ItemId.ToString().Substring(144));
        Console.WriteLine("\tLast 24 characters of the last occurrence's item ID:\t {0}", 
                        recurrMeeting.LastOccurrence.ItemId.ToString().Substring(144)); 
        Console.WriteLine("\tModified Occurrences: {0}", 
                        (recurrMeeting.ModifiedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString()));
        Console.WriteLine("\tDeleted Occurrences: {0}", 
                        recurrMeeting.DeletedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString());
        // Return the ID of the recurring master.
        return recurrMeeting.Id;
}

```

## <a name="create-a-recurring-meeting-by-using-ews"></a>EWS を使用して定期的な会議を作成する
<a name="bk_CreateMtgEWS"> </a>

次の例の要求と応答の XML は、[EWS マネージ API を使用して定期的な会議を作成する](#bk_CreateMtgEWSMA)呼び出しに対応します。[Recurrence](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) 要素の定期的な部分に関係する特定の値を設定することを除けば、要求は本質的に単独インスタンスの予定を作成する際に使用する要求と同じです。次の例は、[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用して、会議を作成する場合の要求 XML を表しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Weekly Update Meeting</t:Subject>
          <t:Body BodyType="HTML">Come hear about how the Organized Observational Paradigm SkyNet project is coming along!</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-08T13:21:32.868-08:00</t:Start>
          <t:End>2014-03-08T14:21:32.868-08:00</t:End>
          <t:Location>Contoso Main Gallery</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Saturday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-03-08-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

 次の例は、**CreateItem** 操作で返される応答 XML を表しています。 
  
**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

次の例は、[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) 操作を使用するときに生成される要求 XML、作成した定期的なアイテムの **ItemId**、定期的なアイテムを作成するときにサーバーによって返される **ItemId** が定期的な予定のマスターを対象にしたものであることを確認するために定期的な予定のマスターにのみ設定された要求プロパティを示しています。　　　　　　　　　　　　　　　　　 
  
**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Recurrence" />
          <t:FieldURI FieldURI="calendar:FirstOccurrence" />
          <t:FieldURI FieldURI="calendar:LastOccurrence" />
          <t:FieldURI FieldURI="calendar:ModifiedOccurrences" />
          <t:FieldURI FieldURI="calendar:DeletedOccurrences" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 次の例は、**GetItem** 操作で返される応答 XML を表しています。 
  
**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
              <t:Subject>Weekly Update Meeting</t:Subject>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              <t:Recurrence>
                <t:WeeklyRecurrence>
                  <t:Interval>1</t:Interval>
                  <t:DaysOfWeek>Saturday</t:DaysOfWeek>
                </t:WeeklyRecurrence>
                <t:NumberedRecurrence>
                  <t:StartDate>2014-03-08-08:00</t:StartDate>
                  <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
                </t:NumberedRecurrence>
              </t:Recurrence>
              <t:FirstOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-03-08T21:21:00Z</t:Start>
                <t:End>2014-03-08T22:21:00Z</t:End>
                <t:OriginalStart>2014-03-08T21:21:00Z</t:OriginalStart>
              </t:FirstOccurrence>
              <t:LastOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-05-10T20:21:00Z</t:Start>
                <t:End>2014-05-10T21:21:00Z</t:End>
                <t:OriginalStart>2014-05-10T20:21:00Z</t:OriginalStart>
              </t:LastOccurrence>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムにアクセスする](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

