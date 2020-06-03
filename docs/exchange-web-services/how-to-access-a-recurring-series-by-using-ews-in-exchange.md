---
title: Exchange の EWS を使用して、定期的なアイテムにアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Exchange の EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスする方法を説明します。
ms.openlocfilehash: dca41472b3b2f775f420b6654d7e43ef456b0583
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456893"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="2c598-103">Exchange の EWS を使用して、定期的なアイテムにアクセスする</span><span class="sxs-lookup"><span data-stu-id="2c598-103">Access a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="2c598-104">Exchange の EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="2c598-104">Learn how to access calendar items in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2c598-p101">定期的に連続で発生する予定または会議は、定期的マスター、決まったパターンに従って繰り返す一連の発生アイテム、および、オプションで、変更された発生アイテムと削除された発生アイテムのセットで構成されています。EWS マネージ API または EWS を使用して、定期的に連続で発生する予定表アイテムにアクセスできます。これにより次のことが可能です。</span><span class="sxs-lookup"><span data-stu-id="2c598-p101">A recurring series of appointments or meetings is made up of a recurring master, a number of occurrences in a series that repeat according to a set pattern, and, optionally, sets of occurrences that were changed and that were deleted. You can use the EWS Managed API or EWS to access calendar items in a recurring series. This enables you to:</span></span>
  
- <span data-ttu-id="2c598-108">アイテム ID に関連付けられた予定表アイテムが、定期的マスターか、一連の発生アイテムか、あるいは連続発生の例外であるかの確認。</span><span class="sxs-lookup"><span data-stu-id="2c598-108">Check to see if a calendar item associated with an item ID is a recurring master, an occurrence in a series, or an exception to a series.</span></span>
    
- <span data-ttu-id="2c598-109">予定表フォルダーでの定期的な予定の検索。</span><span class="sxs-lookup"><span data-stu-id="2c598-109">Search your calendar folder for recurrence appointments.</span></span>
    
- <span data-ttu-id="2c598-110">関連する定期的な予定表アイテムの取得。</span><span class="sxs-lookup"><span data-stu-id="2c598-110">Get related recurrence calendar items</span></span>
    
- <span data-ttu-id="2c598-111">一連の発生アイテム、発生例外、または発生削除の反復処理。</span><span class="sxs-lookup"><span data-stu-id="2c598-111">Iterate through occurrences in a series, occurrence exceptions, or occurrence deletions.</span></span>
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="2c598-112">EWS マネージ API を使用した、定期的な予定表アイテムのコレクションの取得</span><span class="sxs-lookup"><span data-stu-id="2c598-112">Get a collection of recurring calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="2c598-113">予定のコレクションを取得したい場合は、[ExchangeService.FindAppointments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを使用して、特定の期間内に開始、終了する予定すべてを取得し、次の例に示すように、**Occurrence** または **Exception** の種類の予定表アイテムをすべてコレクションに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="2c598-113">If you want to retrieve a collection of appointments, you can use the [ExchangeService.FindAppointments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve all appointments between a given start and end date, and then add all calendar items with an appointment type of **Occurrence** or **Exception** to a collection, as shown in the following example.</span></span> 
  
<span data-ttu-id="2c598-114">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2c598-114">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

<span data-ttu-id="2c598-115">定期的マスターの予定表アイテムは、**FindAppointments** の呼び出しでは戻されませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2c598-115">Note that recurring master calendar items aren't returned in a call to **FindAppointments**.</span></span> <span data-ttu-id="2c598-116">定期的マスターを取得したい場合、またはより一般的なアプローチで予定表アイテムを取得したい場合は、[ExchangeService.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c598-116">If you want to retrieve recurring masters, or you want a more general approach to retrieving calendar items, you need to use [ExchangeService.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="2c598-117">そのうえで、検索フィルターを使用して、選択した日付以降に開始するアイテムのみを取得し、返すアイテムの数を制限するようにアイテム ビューを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="2c598-117">You can then use a search filter to retrieve only items with a start date greater than or equal to a date you choose, and an item view to limit the number of items to return.</span></span> <span data-ttu-id="2c598-118">この期間内に発生するものでも、検索対象の開始日よりも前に開始する定期的マスターは、検出されませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2c598-118">Note that a recurring master with a start date earlier than the start date in your search will not be found, even if occurrences occur in this range.</span></span>
  
<span data-ttu-id="2c598-119">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2c598-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="2c598-120">EWS マネージ API を使用して定期的な予定表アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="2c598-120">Get related recurrence calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="2c598-p103">パズルの 1 ピースだけが手元にあっても、完成させるには、残りのピースが必要です。定期的な予定表アイテムのアイテム ID を持っている場合は、EWS マネージ API のプロパティまたはメソッドからいずれかを使用して、残りのピースを取得します。</span><span class="sxs-lookup"><span data-stu-id="2c598-p103">Sometimes you have one piece of the puzzle, but to solve it you need the rest of the pieces. If you have the item ID for a recurrence calendar item, you can get the other pieces you need by using one of several EWS Managed API properties or methods.</span></span>
  
<span data-ttu-id="2c598-123">**表 1. EWS マネージ API のプロパティまたはメソッドを使用して、関連する定期的な予定表アイテムを取得する**</span><span class="sxs-lookup"><span data-stu-id="2c598-123">**Table 1. EWS Managed API property or method to use to get related recurrence calendar items**</span></span>

|<span data-ttu-id="2c598-124">**次のアイテム ID を持っている場合**</span><span class="sxs-lookup"><span data-stu-id="2c598-124">**If you have the item ID for…**</span></span>|<span data-ttu-id="2c598-125">**取得できるもの**</span><span class="sxs-lookup"><span data-stu-id="2c598-125">**You can get…**</span></span>|<span data-ttu-id="2c598-126">**使用する手段**</span><span class="sxs-lookup"><span data-stu-id="2c598-126">**By using the…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2c598-127">定期的マスターの予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="2c598-127">The recurring master calendar item</span></span>  <br/> | <span data-ttu-id="2c598-128">一連のアイテムで最初に発生するもの</span><span class="sxs-lookup"><span data-stu-id="2c598-128">The first occurrence in a series</span></span>  <br/>  <span data-ttu-id="2c598-129">一連のアイテムで最後に発生するもの</span><span class="sxs-lookup"><span data-stu-id="2c598-129">The last occurrence in a series</span></span>  <br/>  <span data-ttu-id="2c598-130">連続発生アイテムの例外</span><span class="sxs-lookup"><span data-stu-id="2c598-130">The exceptions to a series</span></span>  <br/>  <span data-ttu-id="2c598-131">連続発生アイテムから削除された予定</span><span class="sxs-lookup"><span data-stu-id="2c598-131">The deleted appointments in a series</span></span>  <br/>  <span data-ttu-id="2c598-132">任意の発生アイテム (そのインデックスが指定される)</span><span class="sxs-lookup"><span data-stu-id="2c598-132">Any occurrence (given its index)</span></span>  <br/> |<span data-ttu-id="2c598-133">[Appointment.FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c598-133">[Appointment.FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="2c598-134">[Appointment.LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c598-134">[Appointment.LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="2c598-135">[Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c598-135">[Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="2c598-136">[Appointment.DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c598-136">[Appointment.DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="2c598-137">[Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) メソッド</span><span class="sxs-lookup"><span data-stu-id="2c598-137">[Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="2c598-138">一連のアイテムで単発で発生するもの</span><span class="sxs-lookup"><span data-stu-id="2c598-138">A single occurrence in a series</span></span>  <br/> |<span data-ttu-id="2c598-139">定期的マスター</span><span class="sxs-lookup"><span data-stu-id="2c598-139">The recurring master</span></span>  <br/> |<span data-ttu-id="2c598-140">[Appointment.BindToRecurringMaster](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) メソッド</span><span class="sxs-lookup"><span data-stu-id="2c598-140">[Appointment.BindToRecurringMaster](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="2c598-141">予定表アイテム ([Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクト)</span><span class="sxs-lookup"><span data-stu-id="2c598-141">Any calendar item (an [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object)</span></span>  <br/> |<span data-ttu-id="2c598-142">[予定型](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)の列挙値</span><span class="sxs-lookup"><span data-stu-id="2c598-142">The [appointment type](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) enumeration value</span></span>  <br/> |<span data-ttu-id="2c598-143">[Appointment.AppointmentType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c598-143">[Appointment.AppointmentType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) property</span></span>  <br/> |
   
<span data-ttu-id="2c598-144">次のコード例では、定期的なマスター、一連のアイテムで最初または最後に発生するもの、またはインデックスが指定された発生アイテムを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2c598-144">The following code example shows how to get a recurring master, the first or last occurrence in a series, or an occurrence given its index.</span></span>
  
<span data-ttu-id="2c598-145">この例では、ユーザーが Exchange サーバーから認証されていて、**service** という名前の [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトを取得済みであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2c598-145">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a><span data-ttu-id="2c598-146">EWS を使用して、繰り返し連続で発生する予定アイテムにアクセスする</span><span class="sxs-lookup"><span data-stu-id="2c598-146">Access calendar items in a recurring series by using EWS</span></span>

<span data-ttu-id="2c598-p104">繰り返し連続で発生する予定表アイテムへのアクセス方法は、予定表アイテムの単一インスタンスへのアクセス方法によく似ています。[GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 操作要求を使用して、必要な予定インスタンスの [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) で、求めているプロパティを指定します。[OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) は、発生アイテムの定期的マスターの**ItemId** と、一連のインデックス値を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="2c598-p104">Accessing calendar items in a recurring series is very similar to accessing single instances of calendar items. You use a [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request, specifying the properties you want, with the [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) of the appointment instance you need. The [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contains the **ItemID** of the occurrence's recurring master, as well as its index value in the series.</span></span> 
  
<span data-ttu-id="2c598-p105">次の XML は、インデックスによって指定される一連のアイテムを返すために使用する [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) 要求を示しています。定期的マスターの **ItemID** の値は読みやすいよう短縮されていますので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="2c598-p105">The following XML shows the [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) request used to return an occurrence in a series specified by its index. Note that the **ItemID** of the recurring master has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="2c598-152">サーバーは、[GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで **GetItem** 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す **NoError** の [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) 値、および新しく作成されたメッセージの [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2c598-152">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2c598-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="2c598-153">See also</span></span>


- [<span data-ttu-id="2c598-154">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="2c598-154">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
- [<span data-ttu-id="2c598-155">Exchange の EWS を使用して予定と会議を取得する</span><span class="sxs-lookup"><span data-stu-id="2c598-155">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

