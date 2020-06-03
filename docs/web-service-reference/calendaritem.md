---
title: CalendarItem
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
description: CalendarItem 要素は、Exchange 予定表アイテムを表します。
ms.openlocfilehash: b29141470d157ef5bd67be06a1e1fa1c9536b042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529484"
---
# <a name="calendaritem"></a>CalendarItem

**Calendaritem**要素は、Exchange 予定表アイテムを表します。 
  
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
|[MimeContent](mimecontent.md) <br/> |Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージクラスを表します。  <br/> |
|[件名](subject.md) <br/> |Exchange ストアアイテムおよび応答オブジェクトの件名を表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度レベルを示します。  <br/> |
|[Body](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムが受信された日付と時刻を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのサイズ (バイト単位) を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要度について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを示します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分にアイテムを送信したかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前に送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日付と時刻を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日付と時刻を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日付と時刻を表します。 これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の時間 (分単位) を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] 行の内容として使用される表示文字列を表します。 これは、すべての Cc 受信者表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |To 行の内容として使用される表示文字列を表します。 これは、すべての受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[UID](uid.md) <br/> |予定表アイテムを識別します。  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |ICalendar オブジェクトのインスタンスが作成された日付と時刻を示します。  <br/> |
|[開始](start.md) <br/> |予定表アイテムの開始を表します。 この要素は、予定表アイテムの1回だけに適用されます。  <br/> |
|[終わり](end-ex15websvcsotherref.md) <br/> |期間の最後の部分を表します。 この要素は、予定表アイテムの1回だけに適用されます。  <br/> |
|[OriginalStart](originalstart.md) <br/> |予定表アイテムの元の開始時刻を表します。  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |予定表アイテムまたは会議出席依頼が終日イベントを表しているかどうかを示します。  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |予定表アイテムの空き時間状態を表します。  <br/> |
|[場所](location.md) <br/> |会議または予定の場所を表します。  <br/> |
|[When](when.md) <br/> |予定表アイテムがいつ発生するかについての情報を提供します。  <br/> |
|[IsMeeting](ismeeting.md) <br/> |予定表アイテムが会議または予定であるかどうかを示します。  <br/> |
|[IsCancelled](iscancelled.md) <br/> |予定または会議がキャンセルされたかどうかを示します。  <br/> |
|[IsRecurring](isrecurring.md) <br/> |予定表アイテムが定期的なアイテムの一部であるかどうかを示します。 この要素は値の取得のみ可能です。  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |出席依頼が出席者に送信されたかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |アイテムへの応答が必要かどうかを示します。  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |予定表アイテムの発生の種類を表します。  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |予定表アイテムの状態または応答を含みます。  <br/> |
|[Organizer](organizer.md) <br/> |会議の開催者を表します。  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |会議に出席するために必要な出席者を表します。  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |会議に出席する必要がない出席者を表します。  <br/> |
|[リソース](resources.md) <br/> |会議のスケジュールされたリソースを表します。  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |予定表アイテムと競合する会議の数を表します。  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |会議の時間に隣接する予定表アイテムの合計数を表します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべてのアイテムを識別します。  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表アイテムを説明します。  <br/> |
|[期間 (アイテム)](duration-items.md) <br/> |予定表アイテムの期間を表します。  <br/> |
|[TimeZone (Item)](timezone-item.md) <br/> |タイムゾーンのテキストの説明を提供します。  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |出席者が会議出席依頼に返信した日時を表します。  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |予定のバージョンのシーケンス番号を指定します。  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |予定の状態を指定します。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンを含みます。  <br/> [Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムの最初の出現を表します。  <br/> [Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムの最後の発生を表します。  <br/> [Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |定期的な予定表アイテムの定期的なアイテムの配列が含まれています。  <br/> [Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |定期的な予定表アイテムの削除された出現の配列を格納します。  <br/> [Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |会議がホストされている場所のタイムゾーンを表します。  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |予定表アイテムの開始タイムゾーンを表します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |予定表アイテムの終了タイムゾーンを表します。  <br/> |
|[ConferenceType](conferencetype.md) <br/> |予定表アイテムで実行される会議の種類を示します。  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |出席者が会議に対して会議の新しい日時を提案できるかどうかを示します。  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |会議がオンラインかどうかを示します。  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |予定表アイテムにリンクされている会議ワークスペースの URL が含まれます。  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Microsoft NetShow online 会議の URL を指定します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを最後に変更したユーザーの表示名を含みます。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook Web App のアイテムを編集するために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表アイテムを説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムまたはフォルダーの1つのプロパティに追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべてのアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカルクライアントストアに作成する1つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別の Exchange アイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列を格納します。  <br/> |
|[アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカルクライアントストアで更新する単一のアイテムを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

1つの予定表アイテムを定期的な予定のマスター予定アイテムに更新する場合は、予定表アイテムの元のタイムゾーンを保持するために、[会議 timezone](meetingtimezone.md)要素を指定する必要があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

