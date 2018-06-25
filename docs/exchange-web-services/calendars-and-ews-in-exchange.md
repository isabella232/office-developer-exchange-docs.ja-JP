---
title: Calendars and EWS in Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Exchange の予定表、予定表フォルダーとアイテム、予定、会議について説明します。
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758876"
---
# <a name="calendars-and-ews-in-exchange"></a>Calendars and EWS in Exchange

Exchange の予定表、予定表フォルダーとアイテム、予定、会議について説明します。
  
Outlook などのメール クライアントの予定表機能の多くを既によくご存じでしょう。これにより、予定の追跡、会議のスケジュール設定、ユーザーの空き時間の確認、出席依頼、会議の変更、キャンセルができます。
  
Exchange の予定表関連の機能は、Outlook などのクライアントで表示される内容とは少し異なります。Exchange の EWS は、情報の表示ではなく、情報の作成、保存、送信、変更などを行うことができます。EWS を使用して予定表を操作するには、情報ストレージ、時間、繰り返し、メッセージ フローなどの概念を理解する必要があります。具体的には、以下について理解する必要があります。
  
- 予定表フォルダー、予定表アイテム、予定表ビュー
    
- 会議出席依頼、応答、スケジューリング、参加者、リソース、会議室、空き時間
    
- 時間の長さ、タイム ゾーン、会議や予定の開始時刻と終了時刻
    
- 定期的なアイテム、定期的なパターン、例外、単一インスタンスの予定と会議
    
EWS と EWS マネージ API には、さまざまな予定表関連タスクを実行できるようにする、充実した操作とメソッドのセットが用意されています。たとえば、次の例に示すとおり、EWS マネージ API を使用すれば、わずか数行のコードで会議を作成し、出席者に招待を送信できます。
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a>予定表フォルダーと予定表アイテム
<a name="bk_CalendarFolder"> </a>

予定表フォルダーには予定表アイテムが含まれています。予定表フォルダーには [IPF.Appointment](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) の **フォルダー クラス**があり、[ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS マネージ API プロパティで定義されているアイテムのみを含めることができます。このプロパティは、 [Appointment クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトか、EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) 要素と関連付けられています。 
  
一連の定期的な一連の定期的な例外の発生が、メールボックス内の実際の項目ではないが、内部的には、定期的なアイテムの添付ファイルとして保存ではなく、予定表フォルダー内のアイテムはメールボックス内の他のフォルダー内のアイテムとは少し異なりますマスター シェイプです。 したがって、特定の日付範囲内のすべての予定を取得するために [カレンダー] ビューを使用する必要があります。 予定と予定表のビューを取得する方法の詳細については、[予定および Exchange EWS を使用して会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。
  
## <a name="meetings-and-appointments"></a>会議と予定
<a name="bk_meetings"> </a>

会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいない点です。内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)か、EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 要素を使用して、会議や予定を操作します。 
  
予定も会議も単一のインスタンスや[定期的なアイテム](recurrence-patterns-and-ews.md)の一部ですが、予定は出席者、会議室、リソースを含まないため、メッセージの送信を必要としません。
  
会議には、要求と更新に対する送信と応答が含まれるため、予定表フォルダーのアイテムにアクセスするよりも多くのことが関係します。会議には関連するワークフローもあります。会議のスケジュールは出席者の空き時間に設定する必要があります。また、会議室、プロジェクターやその他の機器などのリソースを予約する必要もあります。
  
会議ワークフローには、通常、次の手順が含まれます。
  
1. 会議が作成され、開始時刻と終了時刻、場所、メッセージの本文などの情報が入力されます。
    
2. 予想される出席者、リソース、会議室の一覧が作成されます。
    
3. 出席者の空き時間の状態がチェックされます。 
    
4. 会議出席依頼が出席者に送信されます。
    
5. 出席者は、出席するかしないかの意向を会議出席依頼に返信します。出席者は、会議の新しい時間を提案する場合もあります。
    
6. 会議がキャンセルまたは更新されることもあり、その場合は通常、出席者に新しいメッセージが送信されます。
    
## <a name="calendars-and-time"></a>予定表と時間
<a name="bk_Time"> </a>

時間関連の機能は、予定表作成に不可欠です。予定と会議には、開始時刻、終了時刻、期間以外に、メッセージを作成、送信、受信した時刻などの時間関連のプロパティがあります。既存の予定と会議は、開始時刻と終了時刻に基づいて予定表フォルダーから取得できます。定期的なアイテムには始まりと終わりがあります。会議は指定されたタイムゾーン内で開始されます。これは、グローバル経済でますます重要になってきています。
  
時刻の値は内部的に協定世界時 (UTC) で Exchange サーバーに保存されます。Exchange は、時刻の値をクライアント設定に基づいてローカル タイム ゾーンに変換します。[DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) プロパティはコンピューターのローカル タイム ゾーンに範囲指定されます。 
  
## <a name="recurring-series"></a>定期的なアイテム
<a name="bk_recurrence"> </a>

予定や会議の定期的なアイテムは、定期的なマスター、発生するアイテムのセット、オプションの例外アイテムのセットで構成されています。定期的なアイテムの情報は定期的なマスター アイテムに格納されます。[RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS 要素は一連のアイテムと例外に関連しています。または、 [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) EWS マネージ API メソッドを使用して、定期的なマスターを取得できます。一連のアイテムのインスタンスを使用すると、一連のアイテムに関連するすべての要素と情報を見つけることができます。 
  
定期的なアイテムのプロパティはすべての予定表アイテムに存在しますが、定期的なマスター アイテムにのみ入力されます。一連のすべてのアイテムのインデックスに加えて、定期的なマスターには、変更されたアイテムや削除されたアイテム、一連のアイテムの定期的なパターン (たとえば、日単位、週単位、月単位、年単位) への参照があります。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 の EWS を使用して予定および会議を作成します。](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [EWS を使用して Exchange、終日のイベントを作成します。](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して予定および会議を取得します。](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して予定および会議を更新します。](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [予定を削除して、Exchange で EWS を使用して会議をキャンセル](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して、ルームの一覧を取得します。](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して空き時間情報を取得します。](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して、会議の新しい日時を提案します。](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [Exchange 予定表のアイテムをまとめてを処理します。](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [定期的なパターンと EWS](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

