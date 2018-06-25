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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759195"
---
# <a name="time-zones-and-ews-in-exchange"></a>Exchange のタイム ゾーンと EWS

Exchange において、タイム ゾーンが EWS マネージ API と EWS でどのように機能するかを確認します。
  
タイム ゾーンは、重要視されることがあまりありません。しかし、EWS マネージ API または EWS を使用して日付と時刻を指定する場合には重要な概念です。EWS マネージ API や EWS アプリケーションでタイム ゾーンの処理を誤ると、予期しない結果が生じることがあります。知識があれば、タイム ゾーンは簡単に正しく処理できます。
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>EWS マネージ API でのタイム ゾーンの処理

EWS マネージ API を使用している場合、タイム ゾーンはほとんどの場合に自動的に処理されます。ユーザー側で明示的にアクションを実行しなくても、API がクライアント コンピューターのローカルのタイム ゾーンを使用し、必要な変換がバックグラウンドで処理されます。目的に沿っていればこれで十分ですが、その他のオプションもあります。
  
1 つのオプションは、 [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx)プロパティを設定しています。 このプロパティでは、EWS のマネージ API によって実行されるすべての要求のタイム ゾーンを制御します。 このプロパティは、読み取り専用です。クラスのコンス トラクターを使用して、それを設定する唯一の方法です。 [ExchangeService(System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd635875%28v=exchg.80%29.aspx)または[ExchangeService (ExchangeVersion, System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd636248%28v=exchg.80%29.aspx)のコンス トラクターのいずれかを使用する場合は、 [System.TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx)オブジェクトとして特定のタイム ゾーンを指定できます。 **TimeZoneInfo**オブジェクトをパラメーターとしては考慮していないその他のコンス トラクターのいずれかを使用する場合、 **ExchangeService**クラスは、クライアント コンピューターの現在のタイム ゾーンに**タイム ゾーン**プロパティを設定します。 
  
**タイム ゾーン**プロパティによって表されるタイム ゾーンでは、特定のタイム ゾーンを設定するか、コンピューターでは、すべての日付と時刻、クライアントのタイム ゾーンをそのままかどうかが表されます。 EWS のマネージ API では、 [System.DateTime](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx)構造体としてすべての日付と時刻のプロパティを公開します。 したがって、日付と時刻のプロパティを設定する場合は、指定した時間を**DateTime**オブジェクトに[DateTime.Kind](http://msdn.microsoft.com/en-us/library/system.datetime.kind%28v=vs.110%29.aspx)プロパティの値に従って解釈されることに注意のようになります。 **Kind**プロパティの値は**未指定**に設定されている場合は、 **DateTime**の値が**タイム ゾーン**のプロパティで指定されたタイム ゾーンであると解釈されます。 日付と時刻のプロパティを表示している場合は、そのタイム ゾーンのすべての**DateTime**プロパティが表されます。 
  
[新しい予定または会議を作成](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)または[既存の予定または会議を更新](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)する場合は、新しい[予定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)のオブジェクトの**タイム ゾーン**で指定されたタイム ゾーンを上書きする機能があります。 ただし、正確にどのようなことをオーバーライドするは、対象としている[EWS のスキーマのバージョン](ews-schema-versions-in-exchange.md)によって異なります。 [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)プロパティの値は、その予定または会議の特定のタイム ゾーンを使用する[Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx)を設定できます。 **Exchange2007_SP1**より大きい値の**ExchangeService.RequestedServerVersion**プロパティの値を使用する場合ことができますもプロパティを設定する、 [Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) [のタイム ゾーンを指定することAppointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx)プロパティ。 ただし、これらのプロパティは、作成要求の日付と時刻の解釈のみに影響する点に注意してください。 予定を取得する場合、開始時刻と終了時刻は**タイム ゾーン**のプロパティで指定されたタイム ゾーンでも表現されます。 
  
既存の予定または会議を更新する場合は、 **StartTimeZone**プロパティや、 **EndTimeZone**プロパティを設定することによって**予定**オブジェクトのタイム ゾーンを変更できます。 これを行うと、それに応じて移動するのには適用可能な時間が発生します。 **EndTimeZone**プロパティを設定することはできません**ExchangeService.RequestedServerVersion**を**Exchange2007_SP1**に設定した場合**StartTimeZone**プロパティの値は、代わりに使用されます。 
  
**表 1 です。EWS のマネージ API でのタイム ゾーンのプロパティ**

|**タイム ゾーン プロパティ**|**最小サーバー要求のバージョン**|**説明**|
|:-----|:-----|:-----|
|[タイム ゾーン](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |**ExchangeService**クラスのコンス トラクターを使用して設定されていない場合、このプロパティはクライアント コンピューターのタイム ゾーンに設定します。 アイテムとアイテムを既存の取得を作成するとき、すべての**DateTime**プロパティは、このタイム ゾーンで表されます。 ゾーン設定が可能で、この時点では、 **Appointment.StartTimeZone**および**Appointment.EndTimeZone**プロパティを設定することで予定や会議のための要求を作成します。 **Appointment.StartTimeZone**プロパティによってオーバーライドされていない場合、このタイム ゾーンは、予定と会議の作成のタイム ゾーンと見なされます。  <br/> |
|[StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |かどうか**予定**の新しいオブジェクトに設定すると、このタイム ゾーンを使用して、 [Appointment.Start](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx)と[Appointment.ReminderDueBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx)のプロパティを解釈します。 このタイム ゾーンは**予定**オブジェクトの作成のタイム ゾーンとも見なされます。  <br/> 既存のアイテムを取得するには、このプロパティは情報提供のみです。 既存の予定の**日付**プロパティの値は常に、 **ExchangeService.TimeZone**プロパティで指定されたタイム ゾーンで表されます。  <br/> |
|[EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |かどうか**予定**の新しいオブジェクトに設定すると、このタイム ゾーンを使用して[Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx)プロパティを解釈します。  <br/> 既存のアイテムを取得するには、このプロパティは情報提供のみです。 既存の予定の**日付**プロパティの値は常に、 **ExchangeService.TimeZone**プロパティで指定されたタイム ゾーンで表されます。  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>EWS でのタイム ゾーンの処理

EWS を使用している場合、タイム ゾーンは自動的に処理されず、処理はもう少し複雑になります。タイム ゾーンが EWS 要求と応答にどのように影響するかは、いくつかの要因によって異なります。
  
- [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)要素で指定されている Exchange のバージョン 
    
- (存在する場合) は、 [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx)要素で指定されたタイム ゾーン 
    
- タイム ゾーンに指定されている、 [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx)、 [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)、 [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx)の要素 (存在する場合に、予定または会議) 
    
- (存在する場合) は、 **dateTime**の XML 要素で指定されたタイム ゾーン 
    
**DateTime**の要素の値で指定されたタイム ゾーンには、次の 3 つのフォームを実行できます。 内のすべての詳細を読み取ることができます[XML スキーマのパート 2: データ型の第 2 版](http://www.w3.org/TR/xmlschema-2/#dateTime)、言い換えて説明していますが。
  
- **世界協定時刻 (UTC):**'Z' を指定します。 例えば`2014-06-06T19:00:00.000Z`
    
- **特定のタイム ゾーン:** 指定された '+' または '-' の時間と分の後にします。 例えば`2014-06-06T19:00:00.000-08:00`
    
- **タイム ゾーンなし:** 任意のタイム ゾーンがない場合で指定します。 例えば`2014-06-06T19:00:00.000`
    
タイム ゾーン (UTC、または特定のタイム ゾーン) は、 **dateTime**値である場合は、その値は常にそのタイム ゾーンとして解釈されます。 タイム ゾーンが存在しない場合、値の解釈は他のタイム ゾーンの関連する要素の特定の組み合わせに依存します。 
  
**表 2 になります。EWS とその影響でタイム ゾーン要素**

|**RequestServerVersion**|**TimeZoneContext が存在しますか。**|**MeetingTimeZone、StartTimeZone、または EndTimeZone (カレンダー項目および MeetingRequest のみ) に存在しますか。**|**UTC の日時**|**特定のタイム ゾーンの日時**|**日時とタイム ゾーンなし**|**予定および会議の作成のタイム ゾーン**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |はい  <br/> |[はい] ( **MeetingTimeZone** )  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**MeetingTimeZone**要素が含まれている[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)または[MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)要素内の要素は、 **MeetingTimeZone**要素は、UTC として解釈される他のすべてのタイム ゾーンとして解釈されます。  <br/> |**MeetingTimeZone**要素内のタイム ゾーン  <br/> |
|**Exchange2007_SP1** <br/> |はい  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |いいえ  <br/> |[はい] ( **MeetingTimeZone** )  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**MeetingTimeZone**要素が含まれている[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)または[MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)要素内の要素は、 **MeetingTimeZone**要素は、UTC として解釈される他のすべてのタイム ゾーンとして解釈されます。  <br/> |**MeetingTimeZone**要素内のタイム ゾーン  <br/> |
|**Exchange2007_SP1** <br/> |いいえ  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
|**Exchange2010**以降では  <br/> |はい  <br/> |( **StartTimeZone**または**EndTimeZone** ) は、[はい]  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**StartTimeZone**要素が存在する場合、[開始](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx)および[ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx)要素の値は、 **StartTimeZone**要素内のタイム ゾーンとして解釈されます。 それ以外の場合、それらの要素の値は、 **TimeZoneContext**要素内のタイム ゾーンとして解釈されます。  <br/> **EndTimeZone**要素が存在する場合は、[開始](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx)要素の値が**EndTimeZone**要素内のタイム ゾーンとして解釈されます。 それ以外の場合、**末尾**の要素の値は、 **TimeZoneContext**要素内のタイム ゾーンとして解釈されます。  <br/> [カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)または[MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)の外側にある要素は、 **TimeZoneContext**要素内のタイム ゾーンとして解釈されます。  <br/> |タイム ゾーンに存在する場合、 **StartTimeZone**要素でない場合は、 **TimeZoneContext**要素のタイム ゾーン  <br/> |
|**Exchange2010**以降では  <br/> |はい  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**TimeZoneContext**要素内のタイム ゾーンとして解釈されます。  <br/> |**TimeZoneContext**要素内のタイム ゾーン  <br/> |
|**Exchange2010**以降では  <br/> |いいえ  <br/> |( **StartTimeZone**または**EndTimeZone** ) は、[はい]  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |**StartTimeZone**要素が存在する場合、[開始](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx)および[ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx)要素の値は、 **StartTimeZone**要素内のタイム ゾーンとして解釈されます。 それ以外の場合、それらの要素の値は、UTC として解釈されます。  <br/> **EndTimeZone**要素が存在する場合は、[開始](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx)要素の値が**EndTimeZone**要素内のタイム ゾーンとして解釈されます。 それ以外の場合、**末尾**の要素の値は、UTC として解釈されます。  <br/> [カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx)または[MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx)の外側にある要素は、UTC として解釈されます。  <br/> |**StartTimeZone**要素を存在する場合、タイム ゾーン UTC の場合は  <br/> |
|**Exchange2010**以降では  <br/> |いいえ  <br/> |いいえ  <br/> |UTC として解釈される  <br/> |値に示されているタイム ゾーンとして解釈される  <br/> |UTC として解釈される  <br/> |UTC  <br/> |
   
サーバーからの応答を解釈するときは、常に各要素の値をチェックし、値を正しく解釈する必要があります。Exchange には常に値のタイム ゾーン (UTC または指定のタイム ゾーン) が含まれます。
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>予定や会議を作成する際のタイム ゾーンのその他の考慮事項

予定または会議を作成するとき、開始時刻に適用するタイム ゾーンは、予定の作成タイム ゾーンとみなされます。作成タイム ゾーンは、予定または会議を作成するときに日付/時刻がどのように解釈されるかを制御するほか、アイテムに次のように影響します。
  
- アイテムが終日イベントの場合は、作成のタイム ゾーンよりも、別のタイム ゾーンを使用しているクライアントから表示した場合、予期しない方法で表示可能性があります。 作成のタイム ゾーンの午前 0 時に終日のイベントの[終日のイベントが作成されたとき](how-to-create-all-day-events-by-using-ews-in-exchange.md)、最初と最後の時間を調整するためです。 その時間は、余分な日数を対象にする項目がありますので、別のタイム ゾーンで午前 0 時以外の時間として表示されます。 このため、可能な場合は、終日イベントを作成するのには、ユーザーのプライマリの予定表作成クライアントに対して構成されているタイム ゾーンを使用することをお勧めします。
    
- アイテムが会議であり、参加者のタイム ゾーンがクライアントのタイム ゾーンと異なる場合、作成タイム ゾーンは出席者が会議要求を受信すると Outlook の情報バーに表示されます。
    
## <a name="in-this-section"></a>このセクションの内容

- [Exchange EWS を使用して、特定のタイム ゾーンで予定を作成します。](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して予定のタイム ゾーンを更新します。](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange のスキーマ バージョンの EWS](ews-schema-versions-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Exchange EWS を使用して予定および会議を更新します。](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange、終日のイベントを作成します。](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [DateTime 構造体](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx)
    
- [TimeZoneInfo クラス](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

