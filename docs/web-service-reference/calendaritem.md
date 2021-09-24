---
title: CalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: CalendarItem 要素は、予定表アイテムExchange表します。
ms.openlocfilehash: b8493a54e42df2789be04b2a426c6aff414ec6f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518863"
---
# <a name="calendaritem"></a>CalendarItem

**CalendarItem 要素は**、予定表アイテムExchangeを表します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |base64Binary 形式で表されるオブジェクトのネイティブの Multipurpose Internet Mail Extensions (MIME) ストリームを含みます。  <br/> |
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[件名](subject.md) <br/> |アイテムと応答オブジェクトを格納Exchangeの件名を表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの感度レベルを示します。  <br/> |
|[Body](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテム ストア内のアイテムに添付されているアイテムまたはファイルExchangeします。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムが受信された日時を表します。  <br/> |
|[サイズ](size.md) <br/> |アイテムのサイズをバイト単位で表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要度について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが Outbox の既定のフォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを示します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分にアイテムを送信したかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前に送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日時を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日時を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションをExchangeします。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日時を表します。 これは [、ReminderMinutesBeforeStart](reminderminutesbeforestart.md) 要素によって使用され、アラームが表示される時間を決定します。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |ユーザー ストア内のアイテムに対してアラームが設定されているかどうかをExchangeします。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の分数を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |Cc 行の内容に使用される表示文字列を表します。 これは、すべての Cc 受信者の表示名の連結文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |To 行の内容に使用される表示文字列を表します。 これは、すべての宛先受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに表示される添付ファイルが 1 つ以上ある場合に **true** に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[UID](uid.md) <br/> |予定表アイテムを識別します。  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |定期的な予定表アイテムの特定のインスタンスを識別するために使用します。  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |iCalendar オブジェクトのインスタンスが作成された日時を示します。  <br/> |
|[Start](start.md) <br/> |予定表アイテムの開始を表します。 この要素は、予定表アイテムの 1 回の出現にのみ適用されます。  <br/> |
|[終わり ](end-ex15websvcsotherref.md) <br/> |期間の終了を表します。 この要素は、予定表アイテムの 1 回の出現にのみ適用されます。  <br/> |
|[OriginalStart](originalstart.md) <br/> |予定表アイテムの元の開始時刻を表します。  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |予定表アイテムまたは会議出席依頼が 1 日のイベントを表すかどうかを示します。  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |予定表アイテムの空き時間情報の状態を表します。  <br/> |
|[Location](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[When](when.md) <br/> |予定表アイテムが発生する時間に関する情報を提供します。  <br/> |
|[IsMeeting](ismeeting.md) <br/> |予定表アイテムが会議か予定かを示します。  <br/> |
|[IsCancelled](iscancelled.md) <br/> |予定または会議が取り消されたかどうかを示します。  <br/> |
|[IsRecurring](isrecurring.md) <br/> |予定表アイテムが定期的なアイテムの一部であるかどうかを示します。 この要素は読み取り専用です。  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |要求された出席者に会議出席依頼が送信されたかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |アイテムへの応答が必要かどうかを示します。  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |予定表アイテムの出現の種類を表します。  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |予定表アイテムの状態または応答を格納します。  <br/> |
|[開催者](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |会議に出席するために必要な出席者を表します。  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |会議に出席する必要がなされていない出席者を表します。  <br/> |
|[リソース](resources.md) <br/> |会議のスケジュールされたリソースを表します。  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |予定表アイテムと競合する会議の数を表します。  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |会議時間に隣接する予定表アイテムの総数を表します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議時間と競合するアイテムを識別します。  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議時間に隣接しているすべての予定表アイテムについて説明します。  <br/> |
|[Duration (Items)](duration-items.md) <br/> |予定表アイテムの期間を表します。  <br/> |
|[TimeZone (Item)](timezone-item.md) <br/> |タイム ゾーンのテキストの説明を提供します。  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |出席者が会議出席依頼に返信した日時を表します。  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |予定のバージョンのシーケンス番号を指定します。  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |予定の状態を指定します。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンが含まれます。  <br/> この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムの最初の出現を表します。  <br/> この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムの最後の出現を表します。  <br/> この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |定期的なマスター アイテムと異なって変更された定期的な予定表アイテムの出現の配列を格納します。  <br/> この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |定期的な予定表アイテムの削除済みアイテムの配列を格納します。  <br/> この要素は [、CalendarItemType に RecurringMaster](calendaritemtype.md) 値がある場合に有効です。  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイム ゾーンを表します。  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |予定表アイテムの開始タイム ゾーンを表します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |予定表アイテムの終了タイム ゾーンを表します。  <br/> |
|[ConferenceType](conferencetype.md) <br/> |予定表アイテムで実行される会議の種類について説明します。  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |出席者が会議に対して新しい会議時間を提案できるかどうかを示します。  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |会議がオンラインかどうかを示します。  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |予定表アイテムによってリンクされている会議ワークスペースの URL を格納します。  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Microsoft NetShow オンライン会議の URL を指定します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを変更する最後のユーザーの表示名を格納します。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Web App エンドポイントに連結する URL をMicrosoft Office Outlookし、Web App エンドポイントでアイテムを読み取Outlook Web App。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Web App エンドポイントに連結する URL Microsoft Office Outlookを表し、Web App エンドポイント内のアイテムをOutlook Web App。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子を含む。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーン テキストを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議時間に隣接しているすべての予定表アイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |UpdateItem 操作中にアイテムまたはフォルダーの 1 つのプロパティに追加する [データを識別します](updateitem-operation.md)。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議時間と競合するアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別のアイテムExchange付けられたアイテムを表Exchangeします。  <br/> |
|[Items](items.md) <br/> |アイテムの配列を含む。  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作内のアイテムの 1 つのプロパティへの更新 [を表します](updateitem-operation.md)。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つのアイテムを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

1 つの予定表アイテムが定期的なマスター 予定表アイテムに更新される場合は、予定表アイテムの元のタイム ゾーンを保持するために [MeetingTimeZone](meetingtimezone.md) 要素を指定する必要があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

