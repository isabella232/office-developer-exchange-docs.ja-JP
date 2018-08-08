---
title: Exchange の EWS を使用して、定期的なアイテムにアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Exchange の EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスする方法を説明します。
ms.openlocfilehash: 9f78ef5b51766a69d23fce3f36c55fbb9422fb16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758900"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a>Exchange の EWS を使用して、定期的なアイテムにアクセスする

Exchange の EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスする方法を説明します。
  
定期的に連続で発生する予定または会議は、定期的マスター、決まったパターンに従って繰り返す一連の発生アイテム、および、オプションで、変更された発生アイテムと削除された発生アイテムのセットで構成されています。EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスできます。これにより次のことが可能です。
  
- アイテム ID に関連付けられた予定表アイテムが、定期的マスターか、一連の発生アイテムか、あるいは連続発生の例外であるかの確認。
    
- 予定表フォルダーでの定期的な予定の検索。
    
- 関連する定期的な予定表アイテムの取得。
    
- 一連の発生アイテム、発生例外、または発生削除の反復処理。
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a>EWS マネージ API を使用した、定期的な予定表アイテムのコレクションの取得

予定のコレクションを取得したい場合は、[ExchangeService.FindAppointments](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを使用して、特定の期間内に開始、終了する予定すべてを取得し、次の例に示すように、**Occurrence** または **Exception** の種類の予定表アイテムをすべてコレクションに追加することができます。 
  
この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 
  
```cs
public static Collection<Appointment> FindRecurringCalendarItems(ExchangeService service, 
                                                                    DateTime startSearchDate, 
                                                                    DateTime endSearchDate)
{
    // Instantiate a collection to hold occurrences and exception calendar items.
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a calendar view to search the calendar folder and specify the properties to return.
    CalendarView calView = new CalendarView(startSearchDate, endSearchDate);
    calView.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                            AppointmentSchema.Subject, 
                                            AppointmentSchema.Start, 
                                            AppointmentSchema.IsRecurring, 
                                            AppointmentSchema.AppointmentType);
    // Retrieve a collection of calendar items.
    FindItemsResults<Appointment> findResults = service.FindAppointments(WellKnownFolderName.Calendar, calView);
    // Add all calendar items in your view that are occurrences or exceptions to your collection.
    foreach (Appointment appt in findResults.Items)
    {
        if (appt.AppointmentType == AppointmentType.Occurrence || appt.AppointmentType == AppointmentType.Exception)
        {
            foundAppointments.Add(appt);
        }
        else
        {
            Console.WriteLine("Discarding calendar item of type {0}.", appt.AppointmentType);
        }
    }
    return foundAppointments;
}

```

定期的マスターの予定表アイテムは、**FindAppointments** の呼び出しでは戻されませんので、ご注意ください。 定期的マスターを取得したい場合、またはより一般的なアプローチで予定表アイテムを取得したい場合は、[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) を使用する必要があります。 そのうえで、検索フィルターを使用して、選択した日付以降に開始するアイテムのみを取得し、返すアイテムの数を制限するようにアイテム ビューを使用することができます。 この期間内に発生するものでも、検索対象の開始日よりも前に開始する定期的マスターは、検出されませんので、ご注意ください。
  
この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 
  
```cs
public static Collection<Appointment> FindCalendarItemsByAppointmentType(ExchangeService service, 
                                                                         AppointmentType myAppointmentType, 
                                                                         DateTime startSearchDate)
{
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a search filter based on the start search date.
    SearchFilter.SearchFilterCollection searchFilter = new SearchFilter.SearchFilterCollection();
    searchFilter.Add(new SearchFilter.IsGreaterThanOrEqualTo(AppointmentSchema.Start, startSearchDate));
    // Create an item view to specify which properties to return.
    ItemView view = new ItemView(20);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                       AppointmentSchema.Subject, 
                                       AppointmentSchema.Start, 
                                       AppointmentSchema.AppointmentType,
                                       AppointmentSchema.IsRecurring);
    // Get the appointment items from the server with the properties we specified.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Calendar, searchFilter, view);
    // Add each of the appointments of the type you want to the collection.
    foreach (Item item in findResults.Items)
    {
        Appointment appt = item as Appointment;
        if (appt.AppointmentType == myAppointmentType)
        {
            foundAppointments.Add(appt);
        }
    }
    return foundAppointments;
}

```

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して定期的な予定表アイテムを取得する

パズルの 1 ピースだけが手元にあっても、完成させるには、残りのピースが必要です。定期的な予定表アイテムのアイテム ID を持っている場合は、EWS マネージ API のプロパティまたはメソッドからいずれかを使用して、残りのピースを取得します。
  
**表 1. EWS マネージ API のプロパティまたはメソッドを使用して、関連する定期的な予定表アイテムを取得する**

|**次のアイテム ID を持っている場合**|**取得できるもの**|**使用する手段**|
|:-----|:-----|:-----|
|定期的マスターの予定表アイテム  <br/> | 一連のアイテムで最初に発生するもの  <br/>  一連のアイテムで最後に発生するもの  <br/>  連続発生アイテムの例外  <br/>  連続発生アイテムから削除された予定  <br/>  任意の発生アイテム (そのインデックスが指定される)  <br/> |[Appointment.FirstOccurrence](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) プロパティ  <br/> [Appointment.LastOccurrence](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) プロパティ  <br/> [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) プロパティ  <br/> [Appointment.DeletedOccurrences](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) プロパティ  <br/> [Appointment.BindToOccurrence](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) メソッド  <br/> |
|一連のアイテムで単発で発生するもの  <br/> |定期的マスター  <br/> |[Appointment.BindToRecurringMaster](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) メソッド  <br/> |
|予定表アイテム ([Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクト)  <br/> |[予定型](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)の列挙値  <br/> |[Appointment.AppointmentType](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) プロパティ  <br/> |
   
次のコード例では、定期的なマスター、一連のアイテムで最初または最後に発生するもの、またはインデックスが指定された発生アイテムを取得する方法を示しています。
  
この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。 
  
```cs
public static void GetRelatedRecurrenceCalendarItems(ExchangeService service, ItemId itemId)
{
    Appointment calendarItem = Appointment.Bind(service, itemId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    PropertySet props = new PropertySet(AppointmentSchema.AppointmentType,
                                        AppointmentSchema.Subject,
                                        AppointmentSchema.FirstOccurrence,
                                        AppointmentSchema.LastOccurrence,
                                        AppointmentSchema.ModifiedOccurrences,
                                        AppointmentSchema.DeletedOccurrences);
    // If the item ID is not for a recurring master, retrieve the recurring master for the series.
    switch (calendarItem.AppointmentType)
    {
        // Calendar item is a recurring master so use Appointment.Bind
        case AppointmentType.RecurringMaster:
            recurrMaster = Appointment.Bind(service, itemId, props);
            break;
        // The calendar item is a single instance meeting, so there are no instances to modify or delete.
        case AppointmentType.Single:
            Console.WriteLine("Item id must reference a calendar item that is part of a recurring series.");
            return;
        // The calendar item is an occurrence in the series, so use BindToRecurringMaster.
        case AppointmentType.Occurrence:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
        // The calendar item is an exception to the series, so use BindToRecurringMaster.                
        case AppointmentType.Exception:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
    }
    // View the first occurrence, last occurrence, and number of modified and deleted occurrences associated with the recurring master.
    Console.WriteLine("Information for the {0} recurring series:", recurrMaster.Subject);
    Console.WriteLine("The start time for the first appointment with id \t{0} was on \t{1}.", 
                        recurrMaster.FirstOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.FirstOccurrence.Start.ToString());
    Console.WriteLine("The start time for the last appointment with id \t{0} will be on \t{1}.", 
                        recurrMaster.LastOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.LastOccurrence.Start.ToString());
    Console.WriteLine("There are {0} modified occurrences and {1} deleted occurrences.", 
                        recurrMaster.ModifiedOccurrences == null ? "no" : recurrMaster.ModifiedOccurrences.Count.ToString(), 
                        recurrMaster.DeletedOccurrences == null ? "no" : recurrMaster.DeletedOccurrences.Count.ToString());
    // Bind to the first occurrence of a series by using its index.
    Appointment firstOccurrence = Appointment.BindToOccurrence(service, 
                                                                recurrMaster.Id, 
                                                                1, // Index of first item is 1, not 0.
                                                                new PropertySet(AppointmentSchema.AppointmentType,
                                                                                AppointmentSchema.Start));
    Console.WriteLine("Compare the start times for a recurring master's first occurrence " + 
                        "and the occurrence found at index 1 using the BindToOccurrence method:");
    Console.WriteLine("The appointment at index 1 has a start time of\t\t\t\t {0}\n" +
                        "Which matches that of the first occurrence on the recurring master: \t {1}",
                        firstOccurrence.Start.ToString(),
                        recurrMaster.FirstOccurrence.Start.ToString());
}

```

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a>EWS を使用して、繰り返し連続で発生する予定アイテムにアクセスする

繰り返し連続で発生する予定表アイテムへのアクセス方法は、予定表アイテムの単一インスタンスへのアクセス方法によく似ています。 [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 操作要求を使用して、必要な予定インスタンスの [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) で、求めているプロパティを指定します。 [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) は、発生アイテムの定期的マスターの**ItemID** と、一連のインデックス値を格納します。 
  
次の XML は、インデックスによって指定される一連のアイテムを返すために使用する [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 要求を示しています。 定期的マスターの **ItemID** の値は読みやすいよう短縮されていますので、ご注意ください。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Start" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkA" InstanceIndex="1" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで **GetItem** 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す **NoError** の [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
- [Exchange の EWS を使用して予定と会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

