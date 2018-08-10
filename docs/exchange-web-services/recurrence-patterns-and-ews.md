---
title: 定期的なパターンと EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Exchange の定期的なパターンと定期的なアイテムについて説明します。
ms.openlocfilehash: ac10e9b9a347abb5907b77f0e0e7315e4e86d97a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759186"
---
# <a name="recurrence-patterns-and-ews"></a>定期的なパターンと EWS

Exchange の定期的なパターンと定期的なアイテムについて説明します。
  
定期的なアイテムは、定義済みのパターンに従って繰り返す予定または会議です。定期的なアイテムは、特定のアイテム数にすることも、無制限で繰り返すこともできます。さらに、定期的なアイテムには、アイテムの残りのパターンに従わない例外もあります。また、パターンから削除されたアイテムを持つこともできます。EWS マネージ API と EWS を使用すると、定期的なアイテムと、それらの関連付けられた予定表アイテムを操作できます。
  
## <a name="recurring-calendar-items"></a>定期的な予定表アイテム

すべての予定表アイテムは、次に示す 4 つのカテゴリのいずれか 1 つに分類されます。
  
- 非定期的な予定表アイテム
    
- 定期的マスター
    
- 定期的なアイテム内のアイテム
    
- 定期的なアイテム内の変更されたアイテム (例外)
    
この記事では、定期的なアイテムの一部である予定表アイテムの 3 つの種類について説明します。
  
これは、定期的なアイテム を Exchange Server 上に実装する方法を理解するために役立ちます。定期的なアイテム内の各アイテムに、個別に異なるアイテムを作成するかわりに、サーバーは予定表で、定期的マスターと呼ばれる実際のアイテムを 1 つだけ作成します。定期的マスターの書式は非定期的な予定とよく似ていますが、定期的なパターンの情報が追加されています。サーバーは予定の情報に関するクライアントの要求に応じて、定期的なパターンを基に展開と呼ばれるプロセスを使用してアイテムを生成します。これらの生成されたアイテムは、永続的にサーバーで保存されるわけではありません。これを理解することは重要です。予定表アイテムを検索する方法が、受け取る情報と、展開を行うかどうかを決定するからです。
  
## <a name="recurrence-patterns"></a>定期的なパターン

展開を可能にする重要な定期的なアイテムは、定期的なパターンです。定期的なパターンは、定期的マスターにあります。定期的なパターンは、定期的マスターの日付および時間に基づいたアイテムの計算に関する条件のセットを記述します。
  
**表 1. 使用可能な定期的なパターン**

|**EWS マネージ API クラス**|**EWS の要素**|**例**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](http://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |毎日繰り返します。  <br/> 隔日で繰り返します。  <br/> |
|[Recurrence.MonthlyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](http://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |毎月 10 日に繰り返します。  <br/> 隔月の 21 日に繰り返します。  <br/> |
|[Recurrence.RelativeMonthlyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](http://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |毎月第 2 火曜日に繰り返します。  <br/> 3 か月ごとの第 3 木曜日に繰り返します。  <br/> |
|[Recurrence.RelativeYearlyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](http://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |毎年 8 月の第 1 月曜日に繰り返します。  <br/> |
|[Recurrence.WeeklyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](http://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |毎週月曜日に繰り返します。  <br/> 隔週の火曜日と木曜日に繰り返します。  <br/> |
|[Recurrence.YearlyPattern](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](http://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |毎年 9 月 1 日に繰り返します。  <br/> |
   
定期的なパターンについての別の重要な情報は、定期的なアイテムが終了するのはいつかということです。これは、アイテムのセット数、終了日、または終了日なしとして表すことができます。
  
**表 2. 定期的なアイテムの終了オプション**

|**EWS マネージ API メソッド/プロパティ**|**EWS の要素**|**説明**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](http://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |このプロパティまたは要素の値は、アイテムの数を指定します。  <br/> |
|[Recurrence.EndDate](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](http://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |定期的なアイテムの最後のアイテムは、このプロパティまたは要素で指定された日付の当日またはそれ以前になります。  <br/> |
|[Recurrence.HasEnd](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](http://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |定期的なアイテムには終わりがありません。  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>展開ビューと非展開ビュー

EWS マネージ API で **FindAppointments** メソッド (または EWS で **CalendarView** 要素を設定した **FindItem** 操作) を使用して、展開プロセスを呼び出します。これは結果セットからの定期的マスターの予定を非表示にし、その代わりに、その定期的なアイテムの展開ビューを表示します。予定表ビューのパラメーターに入る定期的マスターのアイテムと例外は、結果セットに含まれます。これとは逆に、EWS マネージ API で **FindItems** メソッド (または EWS で **IndexedPageItemView** または **FractionalPageItemView** 要素を設定した **FindItem** 操作) を使用しても、展開プロセスは呼び出されません。また、アイテムと例外も含まれません。2 つのメソッドを比較した例を紹介します。 
  
**表 3. 予定を検索するメソッドと操作**

|**EWS マネージ API メソッド**|**EWS 操作**|**定期的なアイテムの展開**|**結果に含まれるアイテム**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[CalendarView](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |あり  <br/> |非定期的な予定、定期的なアイテムの 1 つのアイテム、および定期的なアイテムに対する例外  <br/> |
|[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[IndexedPageItemView](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素または [FractionalPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) 要素を設定した [FindItem 操作](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |なし  <br/> |非定期的な予定と定期的マスターの予定  <br/> |
   
Sadie は最近、自分の息子を水泳チームに参加させました。チームは毎週水曜日の午前 8 時 30 分に練習を行います。7 月 2 日から練習が始まり、最後の練習は 8 月 6 日に行われます。練習を忘れてはいけないので、Sadie は自分の予定表に定期的な予定を追加して、忘れないようにしました。
  
**表 4. Sadie の定期的な予定**

|**予定フィールド**|**値**|
|:-----|:-----|
|件名  <br/> |水泳チームの練習  <br/> |
|開始  <br/> |2014 年 7 月 2 日午前 8 時 30 分  <br/> |
|終了  <br/> |2014 年 7 月 2 日午前 10 時 00 分  <br/> |
|繰り返し  <br/> |毎週水曜日  <br/> |
|最後のアイテム  <br/> |2014 年 8 月 6 日午前 8 時 30 分  <br/> |
   
予定表を一瞥すると、チームは合計 6 回の練習を行うと示されています。しかし予定表には、6 つの個別の予定アイテムはありません。その代わりに、定期的なアイテムを代表する定期的マスターの予定が 1 つだけあります。
  
ここで、Sadie の予定表の、7 月中に発生する予定を見つけることについて説明します。次のコード例では、Exchange マネージ API の **FindItems** メソッドを使用して、Sadie の予定表の非展開ビューを作成します。 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

このコードの結果は、次に示す [IndexedPageItemView](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx)要求になります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

サーバーの応答には、 [RecurringMaster](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) の **CalendarItemType** 要素の値を示す 1 つのアイテム (定期的マスター) のみが含まれます。 [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

では、展開ビューと比較してみましょう。次のコード例では、EWS マネージ API の **FindAppointments** メソッドを使用して、Sadie の予定表の展開ビューを作成します。 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

このコードの結果は、次に示す [CalendarView](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 要素を設定した [FindItem 操作](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)要求になります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

今度は、サーバーの応答に 5 つのアイテム (7 月の各水曜日につき 1 つ) が含まれます。これらのアイテムの [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) 要素は、すべて **Occurrence** の値を持っています。定期的マスターはこの応答に存在しない点に注意してください。 [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は、読みやすいよう短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

定期的マスター、アイテム、または例外があれば、いつでも[別の関連アイテムを取得](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)できます。アイテムまたは例外を指定すると定期的マスターを取得できます。この逆も可能です。
  
## <a name="working-with-recurring-calendar-items"></a>定期的な予定表アイテムの操作

非定期的な予定表アイテムを操作するために使用するメソッドおよび操作と同じものを、定期的なアイテムを操作するために使用します。相違点は、実行するアクションが定期的なアイテム全体に適用されるか、1 つのアイテムのみに適用されるかが、それらのメソッドまたは操作を呼び出すために使用するアイテムによって決まることです。[定期的マスターに実行したアクション](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)は、定期的なアイテム内のすべてのアイテムに適用されますが、[1 つのアイテムまたは例外に実行したアクション](how-to-update-a-recurring-series-by-using-ews.md)は、そのアイテムまたは例外にのみ適用されます。 
  
## <a name="in-this-section"></a>このセクションの内容

- [Exchange の EWS を使用して定期的なアイテムにアクセスする](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを作成する](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して定期的なアイテムを削除する](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Exchange の EWS を使用して定期的なアイテムを更新する](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    
- [Exchange 用の Web サービス クライアントの開発](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS を使用して予定と会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

