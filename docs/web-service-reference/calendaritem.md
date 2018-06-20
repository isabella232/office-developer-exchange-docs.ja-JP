---
title: カレンダー項目
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: カレンダー項目要素は、Exchange 予定表アイテムを表します。
ms.openlocfilehash: c7b6d4930bc42fbe26d35264e2eae0c986cc8db7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759590"
---
# <a name="calendaritem"></a>カレンダー項目

**カレンダー項目**要素は、Exchange 予定表アイテムを表します。 
  
```XML
<CalendarItem>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 **CalendarItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[Subject](subject.md) <br/> |Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度レベルを示します。  <br/> |
|[Body/本文](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムを受信したときの日時を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのバイト単位のサイズを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要性をについて説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムの返信するアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |かどうかの項目がまだ送信されていないことを示します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日時を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日時を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生したときの日時を表します。 [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストアのアイテムのアラームが設定されたかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |分前にアラームが表示されるときに、イベントの数を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] 行の内容のために使用される表示文字列を表します。 これは、すべての Cc 受信者の表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |行の内容のために使用される表示文字列を表します。 これは、すべての受信者の表示名の連結された文字列です。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
|[カルチャ](culture.md) <br/> |メールボックス内の指定したアイテムのカルチャを表します。  <br/> |
|[UID](uid.md) <br/> |予定表アイテムを識別します。  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |定期的な予定表アイテムの特定のインスタンスを識別するために使用します。  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |ICalendar オブジェクトのインスタンスが作成された日時を示します。  <br/> |
|[Start](start.md) <br/> |予定表アイテムの開始を表します。 この要素は、予定表アイテムの 1 回のみに適用されます。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |期間の終了を表します。 この要素は、予定表アイテムの 1 回のみに適用されます。  <br/> |
|[OriginalStart](originalstart.md) <br/> |予定表アイテムの元の開始時刻を表します。  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |予定表アイテムまたは会議出席依頼が終日のイベントを表すかどうかを示します。  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |予定表アイテムの空き/予約済み状態を表します。  <br/> |
|[場所](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[When](when.md) <br/> |予定表アイテムが発生した場合についてを説明します。  <br/> |
|[IsMeeting](ismeeting.md) <br/> |予定表アイテムが会議または予定があるかどうかを示します。  <br/> |
|[IsCancelled](iscancelled.md) <br/> |予定または会議がキャンセルされたかどうかを示します。  <br/> |
|[IsRecurring](isrecurring.md) <br/> |予定表アイテムが定期的なアイテムの一部であるかどうかを示します。 この要素は、読み取り専用です。  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |要求された出席者に会議出席依頼が送信されたかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |項目への応答が必要かどうかを示します。  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |予定表アイテムのアイテムの種類を表します。  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |ステータス、または予定表アイテムへの応答が含まれています。  <br/> |
|[Organizer](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |会議に出席するために必要な出席者を表します。  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |出席者が会議に出席する必要がないことを表します。  <br/> |
|[リソース](resources.md) <br/> |会議のスケジュール設定されたリソースを表します。  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |予定表のアイテムと競合する会議の数を表します。  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |会議の時刻に隣接している予定表アイテムの合計数を表します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべての項目を識別します。  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表のアイテムについて説明します。  <br/> |
|[期間 (アイテム)](duration-items.md) <br/> |予定表アイテムの期間を表します。  <br/> |
|[タイムゾーン (アイテム)](timezone-item.md) <br/> |タイム ゾーンの説明を提供します。  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |会議出席依頼に出席者が返信したときの日時を表します。  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |予定のバージョンのシーケンス番号を指定します。  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |予定の状態を指定します。  <br/> |
|[定期的なアイテム (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。  <br/> この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムが最初に見つかった位置を表します。  <br/> この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムが最後に見つかった位置を表します。  <br/> この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |定期的な予定のマスター アイテムが異なるように変更された定期的な予定表アイテム アイテムの配列が含まれています。  <br/> この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |定期的な予定表アイテムの削除済みアイテムの配列が含まれています。  <br/> この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイム ゾーンを表します。  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |予定表アイテムの開始タイム ゾーンを表します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |予定表アイテムの終了タイム ゾーンを表します。  <br/> |
|[ConferenceType](conferencetype.md) <br/> |予定表アイテムで実行される会議の種類について説明します。  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |出席者によって会議の会議の新しい日時を提案ことができるかどうかを示します。  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |会議がオンラインかどうかを示します。  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |予定表アイテムにリンクされている会議ワークスペースの URL が含まれています。  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Microsoft NetShow オンライン会議の URL を指定します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |最後の項目を変更するのにはユーザーの表示名が含まれています。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に修正された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook Web App 内の項目を編集するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムや会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表のアイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムまたはフォルダーのプロパティを追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべての項目を識別します。  <br/> |
|[(ItemSync) を作成します。](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列が含まれています。  <br/> |
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[更新プログラム (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つの項目を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

マスターの予定表の定期的なアイテムを 1 つの予定表アイテムが更新されると、予定表アイテムの元のタイム ゾーンを保持するために[MeetingTimeZone](meetingtimezone.md)要素を指定してください。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
  

  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

