---
title: FieldURI
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURI
api_type:
- schema
ms.assetid: 24af8e3b-3074-4c8c-8d0a-52446508d044
description: FieldURI 要素は、URI によって頻繁に参照されるプロパティを識別します。
ms.openlocfilehash: 82d1bd49819710fe54cfd9343bdd327798709954
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760518"
---
# <a name="fielduri"></a>FieldURI

**FieldURI**要素は、URI によって頻繁に参照されるプロパティを識別します。 
  
```XML
<FieldURI FieldURI="" />
```

 **PathToUnindexedFieldType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**FieldURI** <br/> |プロパティの URI を識別します。  <br/> |
   
#### <a name="fielduri-attribute"></a>FieldURI 属性

|**値**|**説明**|
|:-----|:-----|
|フォルダー: フォルダー Id  <br/> |**フォルダー Id**のプロパティを識別します。  <br/> |
|フォルダー: ParentFolderId  <br/> |**ParentFolderId**プロパティを識別します。  <br/> |
|フォルダー: 表示名  <br/> |**DisplayName**プロパティを識別します。  <br/> |
|フォルダー: UnreadCount  <br/> |**UnreadCount**プロパティを識別します。  <br/> |
|フォルダー: TotalCount  <br/> |**TotalCount**プロパティを識別します。  <br/> |
|フォルダー: ChildFolderCount  <br/> |**ChildFolderCount**プロパティを識別します。  <br/> |
|フォルダー: FolderClass  <br/> |**FolderClass**プロパティを識別します。  <br/> |
|フォルダー: SearchParameters  <br/> |**SearchParameters**プロパティを識別します。  <br/> |
|フォルダー: ManagedFolderInformation  <br/> |**ManagedFolderInformation**プロパティを識別します。  <br/> |
|フォルダー: PermissionSet  <br/> |**PermissionSet**プロパティを識別します。  <br/> |
|フォルダー: EffectiveRights  <br/> |**EffectiveRights**プロパティを識別します。  <br/> |
|フォルダー: SharingEffectiveRights  <br/> |**SharingEffectiveRights**プロパティを識別します。  <br/> |
|項目: アイテム Id  <br/> |**ItemId**プロパティを識別します。  <br/> |
|アイテム: ParentFolderId  <br/> |**ParentFolderId**プロパティを識別します。  <br/> |
|項目: ItemClass  <br/> |**ItemClass**プロパティを識別します。  <br/> |
|項目: MimeContent  <br/> |**MimeContent**プロパティを識別します。  <br/> |
|項目の添付ファイル:  <br/> |**添付ファイル**のプロパティを識別します。  <br/> |
|アイテムの件名。  <br/> |**サブタイトル**のプロパティを識別します。  <br/> |
|アイテム: DateTimeReceived  <br/> |**DateTimeReceived**プロパティを識別します。  <br/> |
|アイテムのサイズ。  <br/> |**Size**プロパティを識別します。  <br/> |
|項目のカテゴリ。  <br/> |**カテゴリ**のプロパティを識別します。  <br/> |
|: 添付ファイル付きのアイテム  <br/> |**添付ファイル付き**のプロパティを識別します。  <br/> |
|項目の重要性。  <br/> |**重要度**のプロパティを識別します。  <br/> |
|アイテム: InReplyTo  <br/> |**InReplyTo**プロパティを識別します。  <br/> |
|アイテム: InternetMessageHeaders  <br/> |**InternetMessageHeaders**プロパティを識別します。  <br/> |
|アイテム: IsAssociated  <br/> |**IsAssociated**プロパティを識別します。  <br/> |
|アイテム: IsDraft  <br/> |**IsDraft**プロパティを識別します。  <br/> |
|アイテム: IsFromMe  <br/> |**IsFromMe**プロパティを識別します。  <br/> |
|アイテム: IsResend  <br/> |**IsResend**プロパティを識別します。  <br/> |
|アイテム: IsSubmitted  <br/> |**IsSubmitted**プロパティを識別します。  <br/> |
|アイテム: IsUnmodified  <br/> |**IsUnmodified**プロパティを識別します。  <br/> |
|アイテム: DateTimeSent  <br/> |**DateTimeSent**プロパティを識別します。  <br/> |
|アイテム: DateTimeCreated  <br/> |**DateTimeCreated**プロパティを識別します。  <br/> |
|アイテムの本文:  <br/> |**Body**プロパティを識別します。  <br/> |
|アイテム: ResponseObjects  <br/> |**ResponseObjects**プロパティを識別します。  <br/> |
|項目: 感度解析  <br/> |**感度解析**プロパティを識別します。  <br/> |
|アイテム: ReminderDueBy  <br/> |**ReminderDueBy**プロパティを識別します。  <br/> |
|アイテム: ReminderIsSet  <br/> |**ReminderIsSet**プロパティを識別します。  <br/> |
|アイテム: ReminderNextTime  <br/> |**ReminderNextTime**プロパティを識別します。  <br/> |
|項目: ReminderMinutesBeforeStart  <br/> |**ReminderMinutesBeforeStart**プロパティを識別します。  <br/> |
|アイテム: DisplayTo  <br/> |**DisplayTo**プロパティを識別します。  <br/> |
|アイテム: DisplayCc  <br/> |**DisplayCc**プロパティを識別します。  <br/> |
|アイテムのカルチャ。  <br/> |**カルチャ**プロパティを識別します。  <br/> |
|アイテム: EffectiveRights  <br/> |**EffectiveRights**プロパティを識別します。  <br/> |
|アイテム: LastModifiedName  <br/> |**LastModifiedName**プロパティを識別します。  <br/> |
|アイテム: LastModifiedTime  <br/> |**LastModifiedTime**プロパティを識別します。  <br/> |
|アイテム: ConversationId  <br/> |**ConversationId**プロパティを識別します。  <br/> |
|アイテム: UniqueBody  <br/> |**UniqueBody**プロパティを識別します。  <br/> |
|項目: フラグ  <br/> |**フラグ**プロパティを識別します。  <br/> |
|アイテム: StoreEntryId  <br/> |**StoreEntryId**プロパティを識別します。  <br/> |
|項目: InstanceKey  <br/> |**InstanceKey**プロパティを識別します。  <br/> |
|アイテム: NormalizedBody  <br/> |**NormalizedBody**プロパティを識別します。  <br/> |
|アイテム: EntityExtractionResult  <br/> |**EntityExtractionResult**プロパティを識別します。  <br/> |
|itemPolicyTag  <br/> |Idnentifies **PolicyTag**プロパティ。  <br/> |
|アイテム: ArchiveTag  <br/> |**ArchiveTag**プロパティを識別します。  <br/> |
|アイテム: RetentionDate  <br/> |**RetentionDate**プロパティを識別します。  <br/> |
|アイテム: プレビュー  <br/> |**プレビュー**プロパティを識別します。  <br/> |
|アイテム: NextPredictedAction  <br/> |**NextPredictedAction**プロパティを識別します。  <br/> |
|アイテム: GroupingAction  <br/> |**GroupingAction**プロパティを識別します。  <br/> |
|アイテム: PredictedActionReasons  <br/> |**PredictedActionReasons**プロパティを識別します。  <br/> |
|アイテム: IsClutter  <br/> |内部使用のみを目的としています。  <br/> |
|アイテム: RightsManagementLicenseData  <br/> |**RightsManagementLicenseData**プロパティを識別します。  <br/> |
|アイテム: BlockStatus  <br/> |**BlockStatus**プロパティを識別します。  <br/> |
|アイテム: HasBlockedImages  <br/> |**HasBlockedImages**プロパティを識別します。  <br/> |
|アイテム: WebClientReadFormQueryString  <br/> |**WebClientReadFormQueryString**プロパティを識別します。  <br/> |
|アイテム: WebClientEditFormQueryString  <br/> |**WebClientEditFormQueryString**プロパティを識別します。  <br/> |
|TextBody の項目:  <br/> |**TextBody**プロパティを識別します。  <br/> |
|IconIndex の項目:  <br/> |**IconIndex**プロパティを識別します。  <br/> |
|アイテム: MimeContentUTF8  <br/> |**MimeContentUTF8**プロパティを識別します。  <br/> |
|メッセージ: ConversationIndex  <br/> |**ConversationIndex**プロパティを識別します。  <br/> |
|メッセージ: ConversationTopic  <br/> |**ConversationTopic**プロパティを識別します。  <br/> |
|メッセージ: InternetMessageId  <br/> |**InternetMessageId**プロパティを識別します。  <br/> |
|メッセージ: IsRead  <br/> |**IsRead**プロパティを識別します。  <br/> |
|メッセージ: IsResponseRequested  <br/> |**IsResponseRequested**プロパティを識別します。  <br/> |
|メッセージ: IsReadReceiptRequested  <br/> |**IsReadReceiptRequested**プロパティを識別します。  <br/> |
|メッセージ: IsDeliveryReceiptRequested  <br/> |**IsDeliveryReceiptRequested**プロパティを識別します。  <br/> |
|メッセージ: ReceivedBy  <br/> |**ReceivedBy**プロパティを識別します。  <br/> |
|メッセージ: ReceivedRepresenting  <br/> |**ReceivedRepresenting**プロパティを識別します。  <br/> |
|メッセージ: 参照  <br/> |**参照**のプロパティを識別します。  <br/> |
|メッセージ: ReplyTo  <br/> |**ReplyTo**プロパティを識別します。  <br/> |
|メッセージ: から  <br/> |**** プロパティを識別します。  <br/> |
|メッセージの送信者:  <br/> |**送信者**のプロパティを識別します。  <br/> |
|メッセージ: ToRecipients  <br/> |**ToRecipients**プロパティを識別します。  <br/> |
|メッセージ: CcRecipients  <br/> |**CcRecipients**プロパティを識別します。  <br/> |
|メッセージ: BccRecipients  <br/> |**BccRecipients**プロパティを識別します。  <br/> |
|メッセージ: ApprovalRequestData  <br/> |**ApprovalRequestData**プロパティを識別します。  <br/> |
|メッセージ: VotingInformation  <br/> |**VotingInformation**プロパティを識別します。  <br/> |
|メッセージ: ReminderMessageData  <br/> |**ReminderMessageData**プロパティを識別します。  <br/> |
|会議: AssociatedCalendarItemId  <br/> |**AssociatedCalendarItemId**プロパティを識別します。  <br/> |
|会議: IsDelegated  <br/> |**IsDelegated**プロパティを識別します。  <br/> |
|会議: IsOutOfDate  <br/> |**IsOutOfDate**プロパティを識別します。  <br/> |
|会議: HasBeenProcessed  <br/> |**HasBeenProcessed**プロパティを識別します。  <br/> |
|会議: ResponseType  <br/> |**ResponseType**プロパティを識別します。  <br/> |
|会議: ProposedStart  <br/> |**ProposedStart**プロパティを識別します。  <br/> |
|会議: PropsedEnd  <br/> |**ProposedEnd**プロパティを識別します。  <br/> |
|meetingRequest:MeetingRequestType  <br/> |**MeetingRequestType**プロパティを識別します。  <br/> |
|meetingRequest:IntendedFreeBusyStatus  <br/> |**IntendedFreeBusyStatus**プロパティを識別します。  <br/> |
|meetingRequest:ChangeHighlights  <br/> |**ChangeHighlights**プロパティを識別します。  <br/> |
|カレンダー開始します。  <br/> |**起動**プロパティを識別します。  <br/> |
|カレンダー: 終了  <br/> |**End**プロパティを識別します。  <br/> |
|カレンダー: OriginalStart  <br/> |**OriginalStart**プロパティを識別します。  <br/> |
|カレンダー: StartWallClock  <br/> |**StartWallClock**プロパティを識別します。  <br/> |
|カレンダー: EndWallClock  <br/> |**EndWallClock**プロパティを識別します。  <br/> |
|カレンダー: StartTimeZoneId  <br/> |**StartTimeZoneId**プロパティを識別します。  <br/> |
|カレンダー: EndTimeZoneId  <br/> |**EndTimeZoneId**プロパティを識別します。  <br/> |
|カレンダー: IsAllDayEvent  <br/> |**IsAllDayEvent**プロパティを識別します。  <br/> |
|カレンダー: LegacyFreeBusyStatus  <br/> |**LegacyFreeBusyStatus**プロパティを識別します。  <br/> |
|予定表の場所:  <br/> |**Location**プロパティを識別します。  <br/> |
|予定表にします。  <br/> |**** プロパティを識別します。  <br/> |
|カレンダー: IsMeeting  <br/> |**IsMeeting**プロパティを識別します。  <br/> |
|カレンダー: IsCancelled  <br/> |**IsCancelled**プロパティを識別します。  <br/> |
|カレンダー: IsRecurring  <br/> |**IsRecurring**プロパティを識別します。  <br/> |
|カレンダー: MeetingRequestWasSent  <br/> |**MeetingRequestWasSent**プロパティを識別します。  <br/> |
|カレンダー: IsResponseRequested  <br/> |**IsResponseRequested**プロパティを識別します。  <br/> |
|カレンダー: CalendarItemType  <br/> |**CalendarItemType**プロパティを識別します。  <br/> |
|カレンダー: MyResponseType  <br/> |**MyResponseType**プロパティを識別します。  <br/> |
|: 開催者の予定表  <br/> |**開催者**のプロパティを識別します。  <br/> |
|カレンダー: RequiredAttendees  <br/> |**RequiredAttendees**プロパティを識別します。  <br/> |
|カレンダー: OptionalAttendees  <br/> |**OptionalAttendees**プロパティを識別します。  <br/> |
|カレンダー: リソース  <br/> |**リソース**のプロパティを識別します。  <br/> |
|カレンダー: ConflictingMeetingCount  <br/> |**ConflictingMeetingCount**プロパティを識別します。  <br/> |
|カレンダー: AdjacentMeetingCount  <br/> |**AdjacentMeetingCount**プロパティを識別します。  <br/> |
|カレンダー: ConflictingMeetings  <br/> |**ConflictingMeetings**プロパティを識別します。  <br/> |
|カレンダー: AdjacentMeetings  <br/> |**AdjacentMeetings**プロパティを識別します。  <br/> |
|カレンダーの期間:  <br/> |**Duration**プロパティを識別します。  <br/> |
|: タイム ゾーンの予定表  <br/> |**タイム ゾーン**プロパティを識別します。  <br/> |
|カレンダー: AppointmentReplyTime  <br/> |**AppointmentReplyTime**プロパティを識別します。  <br/> |
|カレンダー: AppointmentSequenceNumber  <br/> |**AppointmentSequenceNumber**プロパティを識別します。  <br/> |
|カレンダー: AppointmentState  <br/> |**AppointmentState**プロパティを識別します。  <br/> |
|カレンダー: 定期的なアイテム  <br/> |**定期的なアイテム**のプロパティを識別します。  <br/> |
|カレンダー: FirstOccurrence  <br/> |**FirstOccurrence**プロパティを識別します。  <br/> |
|カレンダー: LastOccurrence  <br/> |**LastOccurrence**プロパティを識別します。  <br/> |
|カレンダー: ModifiedOccurrences  <br/> |**ModifiedOccurrences**プロパティを識別します。  <br/> |
|カレンダー: DeletedOccurrences  <br/> |**DeletedOccurrences**プロパティを識別します。  <br/> |
|カレンダー: MeetingTimeZone  <br/> |**MeetingTimeZone**プロパティを識別します。  <br/> |
|カレンダー: ConferenceType  <br/> |**ConferenceType**プロパティを識別します。  <br/> |
|カレンダー: AllowNewTimeProposal  <br/> |**AllowNewTimeProposal**プロパティを識別します。  <br/> |
|カレンダー: IsOnlineMeeting  <br/> |**IsOnlineMeeting**プロパティを識別します。  <br/> |
|カレンダー: MeetingWorkspaceUrl  <br/> |**MeetingWorkspaceUrl**プロパティを識別します。  <br/> |
|カレンダー: NetShowUrl  <br/> |**NetShowUrl**プロパティを識別します。  <br/> |
|カレンダー: UID  <br/> |**UID**プロパティを識別します。  <br/> |
|カレンダー: RecurrenceId  <br/> |**RecurrenceId**プロパティを識別します。  <br/> |
|カレンダー: DateTimeStamp  <br/> |**DateTimeStamp**プロパティを識別します。  <br/> |
|カレンダー: StartTimeZone  <br/> |**StartTimeZone**プロパティを識別します。  <br/> |
|カレンダー: EndTimeZone  <br/> |**EndTimeZone**プロパティを識別します。  <br/> |
|カレンダー: JoinOnlineMeetingUrl  <br/> |**JoinOnlineMeetingUrl**プロパティを識別します。  <br/> |
|カレンダー: OnlineMeetingSettings  <br/> |**OnlineMeetingSettings**プロパティを識別します。  <br/> |
|カレンダー: IsOrganizer  <br/> |**IsOrganizer**プロパティを識別します。  <br/> |
|タスク: ActualWork  <br/> |**ActualWork**プロパティを識別します。  <br/> |
|タスク: AssignedTime  <br/> |**AssignedTime**プロパティを識別します。  <br/> |
|タスク: BillingInformation  <br/> |**BillingInformation**プロパティを識別します。  <br/> |
|タスク: ChangeCount  <br/> |**ChangeCount**プロパティを識別します。  <br/> |
|タスク: 企業  <br/> |**企業**のプロパティを識別します。  <br/> |
|タスク: CompleteDate  <br/> |**CompleteDate**プロパティを識別します。  <br/> |
|タスクの連絡先:  <br/> |**連絡先**のプロパティを識別します。  <br/> |
|タスク: DelegationState  <br/> |**DelegationState**プロパティを識別します。  <br/> |
|タスク: 代理人  <br/> |**代理人**のプロパティを識別します。  <br/> |
|タスク: DueDate  <br/> |**DueDate**プロパティを識別します。  <br/> |
|タスク: IsAssignmentEditable  <br/> |**IsAssignmentEditable**プロパティを識別します。  <br/> |
|タスクの完了します。  <br/> |**完了**プロパティを識別します。  <br/> |
|タスク: IsRecurring  <br/> |**IsRecurring**プロパティを識別します。  <br/> |
|タスク: IsTeamTask  <br/> |**IsTeamTask**プロパティを識別します。  <br/> |
|タスク: マイレージ  <br/> |**経費情報**プロパティを識別します。  <br/> |
|タスクの所有者:  <br/> |**Owner**プロパティを識別します。  <br/> |
|タスク。 達成率  <br/> |**PercentComplete**プロパティを識別します。  <br/> |
|タスク: 定期的なアイテム  <br/> |**定期的なアイテム**のプロパティを識別します。  <br/> |
|タスク: 開始日  <br/> |**StartDate**プロパティを識別します。  <br/> |
|タスクの状態:  <br/> |**Status**プロパティを識別します。  <br/> |
|タスク: StatusDescription  <br/> |**StatusDescription**プロパティを識別します。  <br/> |
|タスク: TotalWork  <br/> |**TotalWork**プロパティを識別します。  <br/> |
|連絡先のエイリアス:  <br/> |**エイリアス**のプロパティを識別します。 このプロパティは、Exchange Server 2010 のサービス パック 2 (SP2) で導入されました。  <br/> |
|連絡先: AssistantName  <br/> |**AssistantName**プロパティを識別します。  <br/> |
|連絡先: 誕生日  <br/> |**誕生日**プロパティを識別します。  <br/> |
|連絡先: BusinessHomePage  <br/> |**BusinessHomePage**プロパティを識別します。  <br/> |
|連絡先: 子  <br/> |**Children**プロパティを識別します。  <br/> |
|連絡先の会社。  <br/> |**企業**のプロパティを識別します。  <br/> |
|連絡先: 会社名  <br/> |**CompanyName**プロパティを識別します。  <br/> |
|連絡先: CompleteName  <br/> |**CompleteName**プロパティを識別します。  <br/> |
|連絡先: ContactSource  <br/> |**ContactSource**プロパティを識別します。  <br/> |
|連絡先: カルチャ  <br/> |**カルチャ**プロパティを識別します。  <br/> |
|連絡先: 部門  <br/> |**部署**のプロパティを識別します。  <br/> |
|連絡先: 表示名  <br/> |**DisplayName**プロパティを識別します。  <br/> |
|連絡先: DirectoryId  <br/> |**DirectoryId**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: DirectReports  <br/> |**DirectReports**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: EmailAddresses  <br/> |**EmailAddresses**プロパティを識別します。  <br/> |
|連絡先: 表題  <br/> |**表題**のプロパティを識別します。  <br/> |
|連絡先: FileAsMapping  <br/> |**FileAsMapping**プロパティを識別します。  <br/> |
|連絡先: 生成  <br/> |**生成**プロパティを識別します。  <br/> |
|連絡先名:  <br/> |**GivenName**のプロパティを識別します。  <br/> |
|連絡先: ImAddresses  <br/> |**ImAddresses**プロパティを識別します。  <br/> |
|連絡先のイニシャル。  <br/> |**[頭文字]** プロパティを識別します。  <br/> |
|連絡先氏名:  <br/> |**役職**のプロパティを識別します。  <br/> |
|連絡先マネージャー。  <br/> |**マネージャー**のプロパティを識別します。  <br/> |
|連絡先: ManagerMailbox  <br/> |**ManagerMailbox**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: ミドル  <br/> |**ミドル ネーム**のプロパティを識別します。  <br/> |
|連絡先: マイレージ  <br/> |**経費情報**プロパティを識別します。  <br/> |
|連絡先: MSExchangeCertificate  <br/> |**MSExchangeCertificate**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先のニックネーム。  <br/> |**ニックネーム**のプロパティを識別します。  <br/> |
|連絡先のメモ:  <br/> |**「メモ**」プロパティをを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: 事業所  <br/> |**事業所**プロパティを識別します。  <br/> |
|連絡先: PhoneNumbers  <br/> |**PhoneNumbers**プロパティを識別します。  <br/> |
|連絡先: PhoneticFullName  <br/> |**PhoneticFullName**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: PhoneticFirstName  <br/> |**PhoneticFirstName**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: PhoneticLastName  <br/> |**PhoneticLastName**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先の写真。  <br/> |**写真**のプロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: PhysicalAddresses  <br/> |**PhysicalAddresses**プロパティを識別します。  <br/> |
|連絡先: PostalAddressIndex  <br/> |**PostalAddressIndex**プロパティを識別します。  <br/> |
|連絡先: 職業  <br/> |**職業**プロパティを識別します。  <br/> |
|連絡先: SpouseName  <br/> |**SpouseName**プロパティを識別します。  <br/> |
|連絡先: 姓  <br/> |**姓**のプロパティを識別します。  <br/> |
|連絡先: WeddingAnniversary  <br/> |**WeddingAnniversary**プロパティを識別します。  <br/> |
|連絡先: UserSMIMECertificate  <br/> |**UserSMIMECertificate**プロパティを識別します。 このプロパティは、Exchange 2010 SP2 で導入されました。  <br/> |
|連絡先: HasPicture  <br/> |**HasPicture**プロパティを識別します。  <br/> |
|distributionlist:Members  <br/> |**メンバー**プロパティを識別します。  <br/> |
|postitem: PostedTime  <br/> |**PostedTime**プロパティを識別します。  <br/> |
|会話: ConversationId  <br/> |**ConversationId**プロパティを識別します。  <br/> |
|会話: ConversationTopic  <br/> |**ConversationTopic**プロパティを識別します。  <br/> |
|会話: UniqueRecipients  <br/> |**UniqueRecipients**プロパティを識別します。  <br/> |
|会話: GlobalUniqueRecipients  <br/> |**GlobalUniqueRecipients**プロパティを識別します。  <br/> |
|会話: UniqueUnreadSenders  <br/> |**UniqueUnreadSenders**プロパティを識別します。  <br/> |
|会話: GlobalUniqueUnreadSenders  <br/> |**GlobalUniqueUnreadSenders**プロパティを識別します。  <br/> |
|会話: UniqueSenders  <br/> |**UniqueSenders**プロパティを識別します。  <br/> |
|会話: GlobalUniqueSenders  <br/> |**GlobalUniqueSenders**プロパティを識別します。  <br/> |
|会話: LastDeliveryTime  <br/> |**LastDeliveryTime**プロパティを識別します。  <br/> |
|会話: GlobalLastDeliveryTime  <br/> |**GlobalLastDeliveryTime**プロパティを識別します。  <br/> |
|会話のカテゴリ。  <br/> |**カテゴリ**のプロパティを識別します。  <br/> |
|会話: GlobalCategories  <br/> |**GlobalCategories**プロパティを識別します。  <br/> |
|会話フラグ:  <br/> |**フラグ**プロパティを識別します。  <br/> |
|会話: GlobalFlagStatus  <br/> |**GlobalFlagStatus**プロパティを識別します。  <br/> |
|会話: 添付ファイル付き  <br/> |**添付ファイル付き**のプロパティを識別します。  <br/> |
|会話: GlobalHasAttachments  <br/> |**GlobalHasAttachments**プロパティを識別します。  <br/> |
|会話: HasIrm  <br/> |**HasIrm**プロパティを識別します。  <br/> |
|会話: GlobalHasIrm  <br/> |**GlobalHasIrm**プロパティを識別します。  <br/> |
|会話: MessageCount  <br/> |**MessageCount**プロパティを識別します。  <br/> |
|会話: GlobalMessageCount  <br/> |**GlobalMessageCount**プロパティを識別します。  <br/> |
|会話: UnreadCount  <br/> |**UnreadCount**プロパティを識別します。  <br/> |
|会話: GlobalUnreadCount  <br/> |**GlobalUnreadCount**プロパティを識別します。  <br/> |
|会話: サイズ  <br/> |**Size**プロパティを識別します。  <br/> |
|会話: GlobalSize  <br/> |**GlobalSize**プロパティを識別します。  <br/> |
|会話: ItemClasses  <br/> |**ItemClasses**プロパティを識別します。  <br/> |
|会話: GlobalItemClasses  <br/> |**GlobalItemClasses**プロパティを識別します。  <br/> |
|会話の重要性。  <br/> |**重要度**のプロパティを識別します。  <br/> |
|会話: GlobalImportance  <br/> |**GlobalImportance**プロパティを識別します。  <br/> |
|Itemid の会話。  <br/> |**Itemid**プロパティを識別します。  <br/> |
|会話: GlobalItemIds  <br/> |**GlobalItemIds**プロパティを識別します。  <br/> |
|会話: LastModifiedTime  <br/> |**LastModifiedTime**プロパティを識別します。  <br/> |
|会話: InstanceKey  <br/> |**InstanceKey**プロパティを識別します。  <br/> |
|テーマ プレビュー:  <br/> |**プレビュー**プロパティを識別します。  <br/> |
|会話: GlobalParentFolderId  <br/> |**GlobalParentFolderId**プロパティを識別します。  <br/> |
|会話: NextPredictedAction  <br/> |**NextPredictedAction**プロパティを識別します。  <br/> |
|会話: GroupingAction  <br/> |**GroupingAction**プロパティを識別します。  <br/> |
|IconIndex の会話。  <br/> |**IconIndex**プロパティを識別します。  <br/> |
|会話: GlobalIconIndex  <br/> |**GlobalIconIndex**プロパティを識別します。  <br/> |
|会話: DraftItemIds  <br/> |**DraftItemIds**プロパティを識別します。  <br/> |
|会話: HasClutter  <br/> |内部使用のみを目的としています。  <br/> |
|ペルソナ: PersonaId  <br/> |**PersonaId**プロパティを識別します。  <br/> |
|ペルソナ: PersonaType  <br/> |**PersonaType**プロパティを識別します。  <br/> |
|GivenName のペルソナ。  <br/> |**GivenName**のプロパティを識別します。  <br/> |
|ペルソナ: 仕入先名  <br/> |**CompanyName**プロパティを識別します。  <br/> |
|ペルソナ: 姓  <br/> |**姓**のプロパティを識別します。  <br/> |
|ペルソナ: 表示名  <br/> |**DisplayName**プロパティを識別します。  <br/> |
|ペルソナ: EmailAddress  <br/> |**EmailAddress**プロパティを識別します。  <br/> |
|ペルソナ: 表題  <br/> |**表題**のプロパティを識別します。  <br/> |
|ペルソナ: HomeCity  <br/> |**HomeCity**プロパティを識別します。  <br/> |
|ペルソナ: CreationTime  <br/> |**CreationTime**プロパティを識別します。  <br/> |
|ペルソナ: RelevanceScore  <br/> |**RelevanceScore**プロパティを識別します。  <br/> |
|ペルソナ: WorkCity  <br/> |**WorkCity**プロパティを識別します。  <br/> |
|ペルソナ: PersonaObjectStatus  <br/> |**PersonaObjectStatus**プロパティを識別します。  <br/> |
|ペルソナ: FileAsId  <br/> |**FileAsId**プロパティを識別します。  <br/> |
|ペルソナ: DisplayNamePrefix  <br/> |**DisplayNamePrefix**プロパティを識別します。  <br/> |
|ペルソナ: YomiCompanyName  <br/> |**YomiCompanyName**プロパティを識別します。  <br/> |
|ペルソナ: YomiFirstName  <br/> |**YomiFirstName**プロパティを識別します。  <br/> |
|ペルソナ: YomiLastName  <br/> |**YomiLastName**プロパティを識別します。  <br/> |
|ペルソナ: タイトル  <br/> |**Title**プロパティを識別します。  <br/> |
|ペルソナ: EmailAddresses  <br/> |**EmailAddresses**プロパティを識別します。  <br/> |
|ペルソナ: 電話番号  <br/> |**PhoneNumber**プロパティを識別します。  <br/> |
|ペルソナ: ImAddress  <br/> |**ImAddress**プロパティを識別します。  <br/> |
|ペルソナ: ImAddresses  <br/> |**ImAddresses**プロパティを識別します。  <br/> |
|ペルソナ: ImAddresses2  <br/> |**ImAddresses2**プロパティを識別します。  <br/> |
|ペルソナ: ImAddresses3  <br/> |**ImAddresses3**プロパティを識別します。  <br/> |
|ペルソナ: FolderIds  <br/> |**FolderIds**プロパティを識別します。  <br/> |
|ペルソナ: 帰属  <br/> |**帰属**プロパティを識別します。  <br/> |
|ペルソナ: 表示名  <br/> |**表示名**のプロパティを識別します。  <br/> |
|ペルソナの頭文字。  <br/> |**[頭文字]** プロパティを識別します。  <br/> |
|ペルソナ: FileAses  <br/> |**FileAses**プロパティを識別します。  <br/> |
|ペルソナ: FileAsIds  <br/> |**FileAsIds**プロパティを識別します。  <br/> |
|ペルソナ: DisplayNamePrefixes  <br/> |**DisplayNamePrefixes**プロパティを識別します。  <br/> |
|ペルソナ: GivenNames  <br/> |**GivenNames**プロパティを識別します。  <br/> |
|ペルソナ: MiddleNames  <br/> |**MiddleNames**プロパティを識別します。  <br/> |
|ペルソナの姓:  <br/> |**姓**のプロパティを識別します。  <br/> |
|ペルソナ: ジェネレーション  <br/> |**世代**プロパティを識別します。  <br/> |
|ペルソナ: ニックネーム  <br/> |**ニックネーム**のプロパティを識別します。  <br/> |
|ペルソナ: YomiCompanyNames  <br/> |**YomiCompanyNames**プロパティを識別します。  <br/> |
|ペルソナ: YomiFirstNames  <br/> |**YomiFirstNames**プロパティを識別します。  <br/> |
|ペルソナ: YomiLastNames  <br/> |**YomiLastNames**プロパティを識別します。  <br/> |
|ペルソナ: BusinessPhoneNumbers  <br/> |**BusinessPhoneNumbers**プロパティを識別します。  <br/> |
|ペルソナ: BusinessPhoneNumbers2  <br/> |**BusinessPhoneNumbers2**プロパティを識別します。  <br/> |
|ペルソナ: HomePhones  <br/> |**HomePhones**プロパティを識別します。  <br/> |
|ペルソナ: HomePhones2  <br/> |**HomePhones2**プロパティを識別します。  <br/> |
|ペルソナ: MobilePhones  <br/> |**MobilePhones**プロパティを識別します。  <br/> |
|ペルソナ: MobilePhones2  <br/> |**MobilePhones2**プロパティを識別します。  <br/> |
|ペルソナ: AssistantPhoneNumbers  <br/> |**AssistantPhoneNumbers**プロパティを識別します。  <br/> |
|ペルソナ: CallbackPhones  <br/> |**CallbackPhones**プロパティを識別します。  <br/> |
|ペルソナ: CarPhones  <br/> |**CarPhones**プロパティを識別します。  <br/> |
|ペルソナ: HomeFaxes  <br/> |**HomeFaxes**プロパティを識別します。  <br/> |
|ペルソナ: OrganizationMainPhones  <br/> |**OrganizationMainPhones**プロパティを識別します。  <br/> |
|ペルソナ: OtherFaxes  <br/> |**OtherFaxes**プロパティを識別します。  <br/> |
|ペルソナ: OtherTelephones  <br/> |**OtherTelephones**プロパティを識別します。  <br/> |
|ペルソナ: OtherPhones2  <br/> |**OtherPhones2**プロパティを識別します。  <br/> |
|ペルソナ: ポケットベル  <br/> |**ポケットベルなど**のプロパティを識別します。  <br/> |
|ペルソナ: RadioPhones  <br/> |**RadioPhones**プロパティを識別します。  <br/> |
|ペルソナ: TelexNumbers  <br/> |**TelexNumbers**プロパティを識別します。  <br/> |
|ペルソナ: WorkFaxes  <br/> |**WorkFaxes**プロパティを識別します。  <br/> |
|ペルソナ: Emails1  <br/> |**Emails1**プロパティを識別します。  <br/> |
|ペルソナ: Emails2  <br/> |**Emails2**プロパティを識別します。  <br/> |
|ペルソナ: Emails3  <br/> |**Emails3**プロパティを識別します。  <br/> |
|ペルソナ: BusinessHomePages  <br/> |**BusinessHomePages**プロパティを識別します。  <br/> |
|ペルソナ: 学校  <br/> |**学校**のプロパティを識別します。  <br/> |
|ペルソナ: PersonalHomePages  <br/> |**PersonalHomePages**プロパティを識別します。  <br/> |
|ペルソナ: OfficeLocations  <br/> |**OfficeLocations**プロパティを識別します。  <br/> |
|ペルソナ: BusinessAddresses  <br/> |**BusinessAddresses**プロパティを識別します。  <br/> |
|ペルソナ: HomeAddresses  <br/> |**HomeAddresses**プロパティを識別します。  <br/> |
|ペルソナ: OtherAddresses  <br/> |**OtherAddresses**プロパティを識別します。  <br/> |
|ペルソナ: タイトル  <br/> |**タイトル**プロパティを識別します。  <br/> |
|ペルソナ: 部門  <br/> |**部門**のプロパティを識別します。  <br/> |
|ペルソナ: CompanyNames  <br/> |**CompanyNames**プロパティを識別します。  <br/> |
|ペルソナ: マネージャー  <br/> |**マネージャー**のプロパティを識別します。  <br/> |
|ペルソナ: AssistantNames  <br/> |**AssistantNames**プロパティを識別します。  <br/> |
|ペルソナ: 職業  <br/> |**職業**プロパティを識別します。  <br/> |
|ペルソナ: SpouseNames  <br/> |**SpouseNames**プロパティを識別します。  <br/> |
|ペルソナ: 趣味  <br/> |**趣味**プロパティを識別します。  <br/> |
|ペルソナ: WeddingAnniversaries  <br/> |**WeddingAnniversaries**プロパティを識別します。  <br/> |
|ペルソナ: 誕生日  <br/> |**誕生日**プロパティを識別します。  <br/> |
|ペルソナ: 子  <br/> |**Children**プロパティを識別します。  <br/> |
|ペルソナの場所:  <br/> |**場所**のプロパティを識別します。  <br/> |
|ペルソナ: ExtendedProperties  <br/> |**ExtendedProperties**プロパティを識別します。  <br/> |
|ペルソナ: 住所  <br/> |**住所**のプロパティを識別します。  <br/> |
|ペルソナ本文:  <br/> |**本文**のプロパティを識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> | 取得、設定、または作成する追加のプロパティを識別します。  <br/>  この要素への XPath 式は、次のように。  <br/>  `/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[AggregateOn](aggregateon.md) <br/> |グループ化された FindItem 結果セットをグループ化した項目の順序を決定するために使用されるプロパティを表します。  <br/> |
|[GroupBy](groupby.md) <br/> |FindItem クエリの任意のグループ化を指定します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |UpdateFolder 操作でフォルダーの 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |UpdateItem 呼び出し中にアイテムから特定のプロパティを削除する削除操作を表します。  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |UpdateFolder の呼び出し中にフォルダーから特定のプロパティを削除する削除操作を表します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。  <br/> |
|[存在します。](exists.md) <br/> |**True**を返す指定されたプロパティが存在する場合、アイテムの検索式を表します。  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティを比較し、これらが等しい場合**は true**に評価する検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |最初のプロパティ値が大きい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |最初のプロパティには、もう 1 つ以上の場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティが以下の場合に**true**を返す検索式を表す 2 番目の。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティが以下の場合に**true**を返す検索式を表す 2 番目の。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |値が同じではない場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[除外](excludes.md) <br/> |プロパティのビットごとのマスクを実行します。  <br/> |
|[内容](contains.md) <br/> |指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。  <br/> |
|[FieldOrder](fieldorder.md) <br/> |結果の並べ替えに使用する単一のフィールドを表し、並べ替えの方向を示します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素は、[パス](path.md)の代替グループの一部です。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

FieldURI 要素を使用する次の例を次に示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

