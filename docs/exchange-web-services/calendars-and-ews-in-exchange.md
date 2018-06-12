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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758876"
---
# <a name="calendars-and-ews-in-exchange"></a><span data-ttu-id="a3c28-103">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="a3c28-103">Calendars and EWS in Exchange</span></span>

<span data-ttu-id="a3c28-104">Exchange の予定表、予定表フォルダーとアイテム、予定、会議について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-104">Learn about calendars, calendar folders and items, appointments, and meetings in Exchange.</span></span>
  
<span data-ttu-id="a3c28-105">Outlook などのメール クライアントの予定表機能の多くを既によくご存じでしょう。これにより、予定の追跡、会議のスケジュール設定、ユーザーの空き時間の確認、出席依頼、会議の変更、キャンセルができます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-105">You're probably familiar with many of the calendar features in email clients like Outlook, which enable you to track appointments, schedule meetings, check people's availability, invite attendees, and change or cancel meetings.</span></span>
  
<span data-ttu-id="a3c28-p101">Exchange の予定表関連の機能は、Outlook などのクライアントで表示される内容とは少し異なります。Exchange の EWS は、情報の表示ではなく、情報の作成、保存、送信、変更などを行うことができます。EWS を使用して予定表を操作するには、情報ストレージ、時間、繰り返し、メッセージ フローなどの概念を理解する必要があります。具体的には、以下について理解する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p101">Calendar-related features in Exchange are a little different than what you see in a client like Outlook. Instead of displaying information, EWS in Exchange enables you to do things like create, store, send, or change information. To use EWS to work with calendars, you'll need to be familiar with concepts such as information storage, time, recurrence, and message flow. More specifically, you'll need to be familiar with the following:</span></span>
  
- <span data-ttu-id="a3c28-110">予定表フォルダー、予定表アイテム、予定表ビュー</span><span class="sxs-lookup"><span data-stu-id="a3c28-110">Calendar folders, calendar items, and calendar views</span></span>
    
- <span data-ttu-id="a3c28-111">会議出席依頼、応答、スケジューリング、参加者、リソース、会議室、空き時間</span><span class="sxs-lookup"><span data-stu-id="a3c28-111">Meeting requests, responses, scheduling, attendees, resources, rooms, and availability</span></span>
    
- <span data-ttu-id="a3c28-112">時間の長さ、タイム ゾーン、会議や予定の開始時刻と終了時刻</span><span class="sxs-lookup"><span data-stu-id="a3c28-112">Time durations, time zones, and start and end times of meetings and appointments</span></span>
    
- <span data-ttu-id="a3c28-113">定期的なアイテム、定期的なパターン、例外、単一インスタンスの予定と会議</span><span class="sxs-lookup"><span data-stu-id="a3c28-113">Recurring series, recurrence patterns, exceptions, and single instance appointments and meetings</span></span>
    
<span data-ttu-id="a3c28-p102">EWS と EWS マネージ API には、さまざまな予定表関連タスクを実行できるようにする、充実した操作とメソッドのセットが用意されています。たとえば、次の例に示すとおり、EWS マネージ API を使用すれば、わずか数行のコードで会議を作成し、出席者に招待を送信できます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p102">Fortunately, EWS and the EWS Managed API provide a rich set of operations and methods that enable you to perform a wide range of calendar-related tasks. For example, using the EWS Managed API, you can create a meeting and send invitations to attendees with just a few lines of code, as shown in the following example.</span></span>
  
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

## <a name="calendar-folders-and-calendar-items"></a><span data-ttu-id="a3c28-116">予定表フォルダーと予定表アイテム</span><span class="sxs-lookup"><span data-stu-id="a3c28-116">Calendar folders and calendar items</span></span>
<span data-ttu-id="a3c28-117"><a name="bk_CalendarFolder"> </a></span><span class="sxs-lookup"><span data-stu-id="a3c28-117"></span></span>

<span data-ttu-id="a3c28-p103">予定表フォルダーには予定表アイテムが含まれています。予定表フォルダーには [IPF.Appointment](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) の **フォルダー クラス**があり、[ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS マネージ API プロパティで定義されているアイテムのみを含めることができます。このプロパティは、 [Appointment クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトか、EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) 要素と関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p103">Calendar folders contain calendar items. Calendar folders have a [folder class](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) of **IPF.Appointment**, and can include only the items defined by the [ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API property, which is associated with an [Appointment Class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, or the EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="a3c28-120">一連の定期的な一連の定期的な例外の発生が、メールボックス内の実際の項目ではないが、内部的には、定期的なアイテムの添付ファイルとして保存ではなく、予定表フォルダー内のアイテムはメールボックス内の他のフォルダー内のアイテムとは少し異なりますマスター シェイプです。</span><span class="sxs-lookup"><span data-stu-id="a3c28-120">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="a3c28-121">したがって、特定の日付範囲内のすべての予定を取得するために [カレンダー] ビューを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3c28-121">Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view.</span></span> <span data-ttu-id="a3c28-122">予定と予定表のビューを取得する方法の詳細については、[予定および Exchange EWS を使用して会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3c28-122">To learn more about retrieving appointments and calendar views, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="meetings-and-appointments"></a><span data-ttu-id="a3c28-123">会議と予定</span><span class="sxs-lookup"><span data-stu-id="a3c28-123">Meetings and appointments</span></span>
<span data-ttu-id="a3c28-124"><a name="bk_meetings"> </a></span><span class="sxs-lookup"><span data-stu-id="a3c28-124"></span></span>

<span data-ttu-id="a3c28-p105">会議と予定の根本的な違いは、会議には出席者がいますが、予定にはいない点です。内部的には、Exchange は会議と予定の両方に同じオブジェクトを使用します。EWS マネージ API [Appointment クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)か、EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 要素を使用して、会議や予定を操作します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="a3c28-128">予定も会議も単一のインスタンスや[定期的なアイテム](recurrence-patterns-and-ews.md)の一部ですが、予定は出席者、会議室、リソースを含まないため、メッセージの送信を必要としません。</span><span class="sxs-lookup"><span data-stu-id="a3c28-128">Both appointments and meetings can be single instances or part of a [recurring series](recurrence-patterns-and-ews.md), but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span>
  
<span data-ttu-id="a3c28-p106">会議には、要求と更新に対する送信と応答が含まれるため、予定表フォルダーのアイテムにアクセスするよりも多くのことが関係します。会議には関連するワークフローもあります。会議のスケジュールは出席者の空き時間に設定する必要があります。また、会議室、プロジェクターやその他の機器などのリソースを予約する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p106">Because meetings include sending and responding to requests and updates, they involve more than just accessing items in a Calendar folder. They also have an associated workflow. Meetings must be scheduled when attendees are available, and can also involve reserving a meeting room, or resources such as a projector or other equipment.</span></span>
  
<span data-ttu-id="a3c28-132">会議ワークフローには、通常、次の手順が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-132">The meeting workflow typically involves the following steps:</span></span>
  
1. <span data-ttu-id="a3c28-133">会議が作成され、開始時刻と終了時刻、場所、メッセージの本文などの情報が入力されます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-133">A meeting is created and populated with information such as start and end time, location, and a message body.</span></span>
    
2. <span data-ttu-id="a3c28-134">予想される出席者、リソース、会議室の一覧が作成されます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-134">A list of prospective attendees, resources, and rooms is created.</span></span>
    
3. <span data-ttu-id="a3c28-135">出席者の空き時間の状態がチェックされます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-135">The availability status of attendees is checked.</span></span> 
    
4. <span data-ttu-id="a3c28-136">会議出席依頼が出席者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-136">A meeting request is sent to attendees.</span></span>
    
5. <span data-ttu-id="a3c28-p107">出席者は、出席するかしないかの意向を会議出席依頼に返信します。出席者は、会議の新しい時間を提案する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p107">Attendees reply to the meeting with their intention to attend or not. Attendees may also propose a new time for the meeting.</span></span>
    
6. <span data-ttu-id="a3c28-139">会議がキャンセルまたは更新されることもあり、その場合は通常、出席者に新しいメッセージが送信されます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-139">Meetings can be canceled or updated, which typically trigger new messages to be sent to attendees.</span></span>
    
## <a name="calendars-and-time"></a><span data-ttu-id="a3c28-140">予定表と時間</span><span class="sxs-lookup"><span data-stu-id="a3c28-140">Calendars and time</span></span>
<span data-ttu-id="a3c28-141"><a name="bk_Time"> </a></span><span class="sxs-lookup"><span data-stu-id="a3c28-141"></span></span>

<span data-ttu-id="a3c28-p108">時間関連の機能は、予定表作成に不可欠です。予定と会議には、開始時刻、終了時刻、期間以外に、メッセージを作成、送信、受信した時刻などの時間関連のプロパティがあります。既存の予定と会議は、開始時刻と終了時刻に基づいて予定表フォルダーから取得できます。定期的なアイテムには始まりと終わりがあります。会議は指定されたタイムゾーン内で開始されます。これは、グローバル経済でますます重要になってきています。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p108">Time-related functionality is integral to calendaring. Appointments and meetings have start and end times, durations, and other time-related properties, such as the time at which a message is created, sent, and received. Existing appointments and meetings can be retrieved from a Calendar folder based on a start and end time. Recurring series have beginnings and ends. And meetings occur within a given time zone, which is increasingly important in a global economy.</span></span>
  
<span data-ttu-id="a3c28-p109">時刻の値は内部的に協定世界時 (UTC) で Exchange サーバーに保存されます。Exchange は、時刻の値をクライアント設定に基づいてローカル タイム ゾーンに変換します。[DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) プロパティはコンピューターのローカル タイム ゾーンに範囲指定されます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p109">Times are stored internally on an Exchange server in Coordinated Universal Time (UTC). Exchange converts them to local time zone based on client settings. [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) properties are scoped to the computer's local time zone.</span></span> 
  
## <a name="recurring-series"></a><span data-ttu-id="a3c28-150">定期的なアイテム</span><span class="sxs-lookup"><span data-stu-id="a3c28-150">Recurring series</span></span>
<span data-ttu-id="a3c28-151"><a name="bk_recurrence"> </a></span><span class="sxs-lookup"><span data-stu-id="a3c28-151"></span></span>

<span data-ttu-id="a3c28-p110">予定や会議の定期的なアイテムは、定期的なマスター、発生するアイテムのセット、オプションの例外アイテムのセットで構成されています。定期的なアイテムの情報は定期的なマスター アイテムに格納されます。[RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS 要素は一連のアイテムと例外に関連しています。または、 [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) EWS マネージ API メソッドを使用して、定期的なマスターを取得できます。一連のアイテムのインスタンスを使用すると、一連のアイテムに関連するすべての要素と情報を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p110">A recurring series of appointments or meetings is comprised of a recurring master, a set of occurrence items, and optionally, a set of exception items. Recurrence information is stored on the recurring master item. The [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS element is associated with occurrences and exceptions in a series, or you can use the [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API method to get the recurring master. Using an instance of a series, you can find all the elements and information associated with the series.</span></span> 
  
<span data-ttu-id="a3c28-p111">定期的なアイテムのプロパティはすべての予定表アイテムに存在しますが、定期的なマスター アイテムにのみ入力されます。一連のすべてのアイテムのインデックスに加えて、定期的なマスターには、変更されたアイテムや削除されたアイテム、一連のアイテムの定期的なパターン (たとえば、日単位、週単位、月単位、年単位) への参照があります。</span><span class="sxs-lookup"><span data-stu-id="a3c28-p111">Note that recurrence properties exist on all calendar items, but they are populated only on recurring master items. In addition to an index of all occurrences in a series, the recurring master has a reference to modified and deleted occurrences and the recurrence pattern of a series (for example, daily, weekly, monthly, or yearly).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="a3c28-158">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="a3c28-158">In this section</span></span>
<span data-ttu-id="a3c28-159"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="a3c28-159"></span></span>

- [<span data-ttu-id="a3c28-160">Exchange 2013 の EWS を使用して予定および会議を作成します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-160">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="a3c28-161">EWS を使用して Exchange、終日のイベントを作成します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-161">Create all-day events by using EWS in Exchange</span></span>](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-162">Exchange EWS を使用して予定および会議を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-163">Exchange EWS を使用して予定および会議を更新します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-164">予定を削除して、Exchange で EWS を使用して会議をキャンセル</span><span class="sxs-lookup"><span data-stu-id="a3c28-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-165">Exchange EWS を使用して、ルームの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-165">Get room lists by using EWS in Exchange</span></span>](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-166">Exchange EWS を使用して空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-166">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-167">Exchange EWS を使用して、会議の新しい日時を提案します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-167">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a3c28-168">Exchange 予定表のアイテムをまとめてを処理します。</span><span class="sxs-lookup"><span data-stu-id="a3c28-168">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="a3c28-169">定期的なパターンと EWS</span><span class="sxs-lookup"><span data-stu-id="a3c28-169">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="a3c28-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3c28-170">See also</span></span>


- [<span data-ttu-id="a3c28-171">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="a3c28-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="a3c28-172">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="a3c28-172">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="a3c28-173">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="a3c28-173">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

