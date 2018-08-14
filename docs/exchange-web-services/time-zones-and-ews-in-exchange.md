---
title: Exchange のタイム ゾーンと EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Exchange において、タイム ゾーンが EWS マネージ API と EWS でどのように機能するかを確認します。
ms.openlocfilehash: fcc8b00acf2b63de04718e13b82191de95bbf2b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759195"
---
# <a name="time-zones-and-ews-in-exchange"></a>Exchange のタイム ゾーンと EWS

Exchange において、タイム ゾーンが EWS マネージ API と EWS でどのように機能するかを確認します。
  
タイム ゾーンは、重要視されることがあまりありません。しかし、EWS マネージ API または EWS を使用して日付と時刻を指定する場合には重要な概念です。EWS マネージ API や EWS アプリケーションでタイム ゾーンの処理を誤ると、予期しない結果が生じることがあります。知識があれば、タイム ゾーンは簡単に正しく処理できます。
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>EWS マネージ API でのタイム ゾーンの処理

EWS マネージ API を使用している場合、タイム ゾーンはほとんどの場合に自動的に処理されます。ユーザー側で明示的にアクションを実行しなくても、API がクライアント コンピューターのローカルのタイム ゾーンを使用し、必要な変換がバックグラウンドで処理されます。目的に沿っていればこれで十分ですが、その他のオプションもあります。
  
オプションの 1 つとして、[ExchangeService.TimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) プロパティの設定があります。 このプロパティは、EWS マネージ API で実行されるすべての要求のタイム ゾーンを制御します。 このプロパティは読み取り専用であり、クラスのコンストラクターを介してのみ設定できます。 [ExchangeService(System.TimeZoneInfo)](http://msdn.microsoft.com/ja-JP/library/dd635875%28v=exchg.80%29.aspx) または [ExchangeService(ExchangeVersion, System.TimeZoneInfo)](http://msdn.microsoft.com/ja-JP/library/dd636248%28v=exchg.80%29.aspx) コンストラクターのいずれかを使用する場合、[System.TimeZoneInfo](http://msdn.microsoft.com/ja-JP/library/system.timezoneinfo%28v=vs.110%29.aspx) オブジェクトとして特定のタイム ゾーンを指定できます。 パラメーターとして **TimeZoneInfo** オブジェクトを取らない他のコンストラクターのいずれかを使用する場合、**ExchangeService** クラスが **TimeZone** プロパティをクライアント コンピューターの現在のタイム ゾーンに設定します。 
  
特定のタイム ゾーンを設定した場合も、クライアント コンピューターのタイム ゾーンのままにした場合も、すべての日付と時刻は、**TimeZone** プロパティが示すタイム ゾーンで表示されます。 EWS マネージ API は、すべての日付/時刻のプロパティを [System.DateTime](http://msdn.microsoft.com/ja-JP/library/system.datetime%28v=vs.110%29.aspx) 構造体として公開します。 このため、日付/時刻のプロパティを設定する場合は、指定した時刻が **DateTime** オブジェクトの [DateTime.Kind](http://msdn.microsoft.com/ja-JP/library/system.datetime.kind%28v=vs.110%29.aspx) プロパティの値に応じて解釈されることに注意してください。 **Kind** プロパティの値が **Unspecified** に設定されると、**DateTime** の値は **TimeZone** プロパティで指定されたタイム ゾーンにあると解釈されます。 日付/時刻のプロパティを読み取る場合は、すべての **DateTime** プロパティがそのタイム ゾーンで表されます。 
  
[新しい予定や会議を作成する場合](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)、または[既存の予定や会議を更新する場合](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)は、新しい [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトに対して **TimeZone** で指定されたタイム ゾーンを上書きできます。 ただし、何を実際に上書きできるかは、目的としている [EWS スキーマ バージョン](ews-schema-versions-in-exchange.md) によって決まります。 [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) プロパティのすべての値に対して、予定や会議に固有のタイム ゾーンを使用できるように、[Appointment.StartTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) を設定できます。 **Exchange2007_SP1** を超える **ExchangeService.RequestedServerVersion** プロパティの値を使用している場合、[Appointment.EndTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) プロパティも設定して、[Appointment.End](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) プロパティのタイム ゾーンを指定することができます。 ただし、これらのプロパティは、作成要求の日付と時刻の解釈のみに反映される点に注意してください。 予定を取得した場合、開始時刻と終了時刻は **TimeZone** プロパティで指定したタイム ゾーンで表示されます。 
  
既存の予定または会議を更新する場合、**Appointment** オブジェクトのタイム ゾーンは **StartTimeZone** プロパティまたは **EndTimeZone** プロパティ、あるいはその両方を設定して変更できます。 これに応じて、時間が適切にシフトします。 **ExchangeService.RequestedServerVersion** を **Exchange2007_SP1** に設定している場合は、**EndTimeZone** プロパティを設定することはできません。代わりに **StartTimeZone** プロパティの値が使用されます。 
  
**表 1. EWS マネージ API でのタイム ゾーンのプロパティ**

|**タイム ゾーンのプロパティ**|**最小サーバーの要求バージョン**|**説明**|
|:-----|:-----|:-----|
|[TimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |**ExchangeService** クラスのコンストラクターを使用して設定していない場合、このプロパティはクライアント コンピューターのタイム ゾーンに設定されます。 アイテムを作成するとき、および既存のアイテムを取得するときのすべての **DateTime** プロパティは、このタイム ゾーンで表現されます。 このタイム ゾーンは、予定や会議の作成要求で **Appointment.StartTimeZone** または **Appointment.EndTimeZone** プロパティ、あるいはその両方の設定によって上書きされます。 **Appointment.StartTimeZone** プロパティで上書きされない場合は、このタイム ゾーンが予定や会議の作成タイム ゾーンとみなされます。  <br/> |
|[StartTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |新しい **Appointment** オブジェクトで設定した場合、このタイム ゾーンは [Appointment.Start](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) および [Appointment.ReminderDueBy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) プロパティの解釈に使用されます。 また、このタイム ゾーンは、**Appointment** オブジェクトの作成タイム ゾーンとみなされます。  <br/> 既存のアイテムを取得する場合、このプロパティは情報のみを提供します。 既存の予定の **DateTime** プロパティは常に、**ExchangeService.TimeZone** プロパティで指定したタイム ゾーンで表現されます。  <br/> |
|[EndTimeZone](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |新しい **Appointment** オブジェクトで設定した場合、このタイム ゾーンは [Appointment.End](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) プロパティの解釈に使用されます。  <br/> 既存のアイテムを取得する場合、このプロパティは情報のみを提供します。 既存の予定の **DateTime** プロパティは常に、**ExchangeService.TimeZone** プロパティで指定したタイム ゾーンで表現されます。  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>EWS でのタイム ゾーンの処理

EWS を使用している場合、タイム ゾーンは自動的に処理されず、処理はもう少し複雑になります。タイム ゾーンが EWS 要求と応答にどのように影響するかは、いくつかの要因によって異なります。
  
- [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 要素で指定されている Exchange のバージョン 
    
- [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) 要素 (ある場合) で指定されているタイム ゾーン 
    
- [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx)、[StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)、[EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) 要素 (予定または会議にある場合) で指定されているタイム ゾーン 
    
- XML **dateTime** 要素 (ある場合) に指定されているタイム ゾーン 
    
**dateTime** 要素の値で指定されるタイム ゾーンには、次の 3 つの形式があります。 詳しくは、「[XML Schema Part 2: Datatypes Second Edition](http://www.w3.org/TR/xmlschema-2/#dateTime)」をご参照ください。ただし、
  
- **協定世界時 (UTC):** 'Z' で指定される値に読み替えてください。 例: `2014-06-06T19:00:00.000Z`
    
- **特定のタイム ゾーン:** '+' または '-' で指定され、時間と分がそれに続きます。 例: `2014-06-06T19:00:00.000-08:00`
    
- **タイム ゾーンなし:** タイム ゾーンが存在しないものとして指定します。 例: `2014-06-06T19:00:00.000`
    
タイム ゾーンが **dateTime** 値 (UTC または特定のタイム ゾーン) として示される場合、値は常にそのタイム ゾーンとして解釈されます。 タイム ゾーンがない場合、この値はその他のタイム ゾーン関連の要素の特定の組み合わせに応じて解釈されます。 
  
**表 2. EWS でのタイム ゾーン要素とその影響**

|**RequestServerVersion**|**TimeZoneContext がありますか。**|**MeetingTimeZone、StartTimeZone、または EndTimeZone がありますか (CalendarItem と MeetingRequest のみですか)。**|**UTC の dateTime**|**特定のタイム ゾーンの dateTime**|**タイム ゾーンのない dateTime**|**予定や会議の作成タイム ゾーン**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |はい  <br/> |はい (**MeetingTimeZone**)  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**MeetingTimeZone** 要素を含む [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 内の要素または [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) 要素は、**MeetingTimeZone** 要素のタイム ゾーンとして解釈され、その他のものは UTC として解釈される  <br/> |**MeetingTimeZone** 要素のタイム ゾーン  <br/> |
|**Exchange2007_SP1** <br/> |はい  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |いいえ  <br/> |はい (**MeetingTimeZone**)  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**MeetingTimeZone** 要素を含む [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 内の要素または [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) 要素は、**MeetingTimeZone** 要素のタイム ゾーンとして解釈され、その他のものは UTC として解釈される  <br/> |**MeetingTimeZone** 要素のタイム ゾーン  <br/> |
|**Exchange2007_SP1** <br/> |いいえ  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
|**Exchange2010** 以降  <br/> |はい  <br/> |はい (**StartTimeZone** または **EndTimeZone**、あるいはその両方)  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**StartTimeZone** 要素がある場合、[Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) および [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) 要素の値は **StartTimeZone** 要素のタイム ゾーンとして解釈されます。 それ以外の場合、その要素の値は **TimeZoneContext** 要素のタイム ゾーンとして解釈されます。  <br/> **EndTimeZone** 要素がある場合、[Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) 要素の値は **EndTimeZone** 要素のタイム ゾーンとして解釈されます。 それ以外の場合、**End** 要素の値は **TimeZoneContext** 要素のタイム ゾーンとして解釈されます。  <br/> [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) または [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) 外の要素は、**TimeZoneContext** 要素のタイム ゾーンとして解釈されます。  <br/> |ある場合は **StartTimeZone** 要素のタイム ゾーン、ない場合は **TimeZoneContext** 要素のタイム ゾーン  <br/> |
|**Exchange2010** 以降  <br/> |はい  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**TimeZoneContext** 要素のタイム ゾーンとして解釈される  <br/> |**TimeZoneContext** 要素のタイム ゾーン  <br/> |
|**Exchange2010** 以降  <br/> |いいえ  <br/> |はい (**StartTimeZone** または **EndTimeZone**、あるいはその両方)  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**StartTimeZone** 要素がある場合、[Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) および [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) 要素の値は **StartTimeZone** 要素のタイム ゾーンとして解釈されます。 それ以外の場合、その要素の値は UTC として解釈されます。  <br/> **EndTimeZone** 要素がある場合、[Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) 要素の値は **EndTimeZone** 要素のタイム ゾーンとして解釈されます。 それ以外の場合、**End** 要素の値は UTC として解釈されます。  <br/> [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) または [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) 外の要素は UTC として解釈されます。  <br/> |ある場合は **StartTimeZone** 要素のタイムゾーン、ない場合は UTC  <br/> |
|**Exchange2010** 以降  <br/> |いいえ  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
   
サーバーからの応答を解釈するときは、常に各要素の値をチェックし、値を正しく解釈する必要があります。Exchange には常に値のタイム ゾーン (UTC または指定のタイム ゾーン) が含まれます。
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>予定や会議を作成する際のタイム ゾーンのその他の考慮事項

予定または会議を作成するとき、開始時刻に適用するタイム ゾーンは、予定の作成タイム ゾーンとみなされます。作成タイム ゾーンは、予定または会議を作成するときに日付/時刻がどのように解釈されるかを制御するほか、アイテムに次のように影響します。
  
- アイテムが終日イベントの場合、作成タイム ゾーンとは別のタイム ゾーンを使用しているクライアントから表示すると、表示が予期しない状態になることがあります。 これは[終日イベントが作成されたとき](how-to-create-all-day-events-by-using-ews-in-exchange.md)、終日イベントの開始時刻と終了時刻が作成タイム ゾーンの午前 0 時に調整されるためです。 その時刻は、別のタイム ゾーンの表示では午前 0 時ではないため、アイテムが別の日にも表示されることがあります。 このため、可能であれば、ユーザーの標準予定表管理クライアント用のタイム ゾーンを使用して、終日イベントを作成することをお勧めします。
    
- アイテムが会議であり、参加者のタイム ゾーンがクライアントのタイム ゾーンと異なる場合、作成タイム ゾーンは出席者が会議要求を受信すると Outlook の情報バーに表示されます。
    
## <a name="in-this-section"></a>このセクションの内容

- [Exchange の EWS を使用して、特定のタイム ゾーンで予定を作成する](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用して予定のタイム ゾーンを更新する](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS スキーマのバージョン](ews-schema-versions-in-exchange.md)
    
- [Exchange 2013 で EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Exchange で EWS を使用して予定と会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して終日イベントを作成する](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [DateTime 構造体](http://msdn.microsoft.com/ja-JP/library/system.datetime%28v=vs.110%29.aspx)
    
- [TimeZoneInfo クラス](http://msdn.microsoft.com/ja-JP/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

