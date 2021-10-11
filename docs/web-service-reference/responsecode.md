---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: ResponseCode 要素は、要求に関する状態情報を提供します。
ms.openlocfilehash: fc328ffde3a21add77ce6870a87bc7092f3f46ab
ms.sourcegitcommit: f13a3a4a61fa23ca6414b7c96ddf087adbe3dc9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2021
ms.locfileid: "60262219"
---
# <a name="responsecode"></a>ResponseCode

**ResponseCode 要素は**、要求に関する状態情報を提供します。 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|要素|説明|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 応答の状態に関する説明情報を提供します。<br/><br/>  この要素で使用できる XPath 式を次に示します。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |単一の DeleteItem 操作要求の状態と [結果を格納](deleteitem-operation.md) します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |1 つの SendItem 操作要求の状態と [結果を格納](senditem-operation.md) します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |1 つの DeleteFolder 操作要求の状態と [結果を格納](deletefolder-operation.md) します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |単一の [DeleteAttachment](deleteattachment-operation.md) 操作要求の状態と結果を格納します。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |1 つの Unsubscribe 操作要求の状態と結果 [を格納](unsubscribe-operation.md) します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の CreateFolder 操作要求の状態と [結果を格納](createfolder-operation.md) します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1 つの GetFolder 操作要求の状態と [結果を格納](getfolder-operation.md) します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |単一の UpdateFolder 操作要求の状態と [結果を格納](updatefolder-operation.md) します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1 つの MoveFolder 操作要求の状態と [結果を格納](movefolder-operation.md) します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |単一の CopyFolder 操作要求の状態と [結果を格納](copyfolder-operation.md)します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |1 つの CreateManagedFolder 操作要求の状態 [と結果を格納](createmanagedfolder-operation.md) します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |1 つの FindFolder 操作要求の状態と [結果を格納](findfolder-operation.md) します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |1 つの CreateItem 操作要求の状態と [結果を格納](createitem-operation.md) します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |1 つの GetItem 操作要求の状態と [結果を格納](getitem-operation.md) します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |単一の UpdateItem 操作要求の状態と [結果を格納](updateitem-operation.md) します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1 つの MoveItem 操作要求の状態と [結果を格納](moveitem-operation.md) します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |単一の CopyItem 操作要求の状態と [結果を格納](copyitem-operation.md) します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |単一の [CreateAttachment](createattachment-operation.md) 操作要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1 つの [GetAttachment](getattachment-operation.md) 操作要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1 つの FindItem 操作要求の状態と [結果を格納](finditem-operation.md) します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 操作要求の状態 [と結果を格納](resolvenames-operation.md) します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1 つの ExpandDL 操作要求の状態と結果 [を格納](expanddl-operation.md) します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |単一の Subscribe 操作要求の状態と結果 [を格納](subscribe-operation.md) します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |1 つの GetEvents 操作要求の状態 [と結果を格納](getevents-operation.md) します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1 つの SendNotification 操作要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |[SyncFolderHierarchy 操作要求の状態と結果を格納](syncfolderhierarchy-operation.md)します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[SyncFolderItems](syncfolderitems-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |ConvertId 操作要求の状態と結果 [を格納](convertid-operation.md) します。  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |AddDelegate 操作要求の状態 [と結果を格納](adddelegate-operation.md) します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |GetDelegate 操作要求の状態 [と結果を格納](getdelegate-operation.md) します。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |[RemoveDelegate](removedelegate-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |UpdateDelegate 操作要求の状態 [と結果を格納](updatedelegate-operation.md) します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |[GetServerTimeZones](getservertimezones-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |[GetSharingFolder](getsharingfolder-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |[GetSharingFolder 操作要求への応答を定義](getsharingfolder-operation.md)します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |[GetSharingMetadata 操作要求の状態と結果を格納](getsharingmetadata-operation.md)します。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |[GetSharingMetadata 操作要求への応答を定義](getsharingmetadata-operation.md)します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |[RefreshSharingFolder](refreshsharingfolder-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |[RefreshSharingFolder 操作要求への応答を定義](refreshsharingfolder-operation.md)します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |[FindConversation](findconversation-operation.md)操作応答の状態と結果を格納します。  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |[ApplyConversationAction](applyconversationaction-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |単一の EmptyFolder 操作要求の状態と [結果を格納](emptyfolder-operation.md) します。  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |[UpdateInboxRules](updateinboxrules-operation.md)操作要求の状態と結果を格納します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |UploadItems 操作要求の状態 [と結果が含](uploaditems-operation.md) まれる。  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |[GetInboxRules 操作 **** 要求に対する応答](getinboxrules-operation.md)を含む。  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |[GetServiceConfiguration 操作要求に対する応答が含](getserviceconfiguration-operation.md)まれる。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成設定が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、テキスト値が必要です。 次の表に、この要素で返される値を示します。
  
|値|説明|
|:-----|:-----|
|NoError  <br/> |要求に対してエラーが発生しました。  <br/> |
|ErrorAccessDenied  <br/> |このエラーは、呼び出し元のアカウントに要求されたアクションを実行する権限が存在しない場合に発生します。  <br/> |
|ErrorAccessModeSpecified  <br/> |このエラーは内部でのみ使用されます。 このエラーは返されません。  <br/> |
|ErrorAccountDisabled  <br/> |このエラーは、問題のアカウントが無効になっている場合に発生します。  <br/> |
|ErrorAddDelegatesFailed  <br/> |このエラーは、代理人が追加されたリストを保存できない場合に発生します。  <br/> |
|ErrorAddressSpaceNotFound  <br/> |このエラーは、フォレスト間の可用性に関するアドレス 空間レコード (ドメイン ネーム システム (DNS) ドメイン名が Active Directory データベースに見つからない場合に発生します。  <br/> |
|ErrorADOperation  <br/> |このエラーは、Active Directory ドメイン サービス (DS) との通信の問題が原因で操作がADされます。  <br/> |
|ErrorADSessionFilter  <br/> |**ResolveNames** 操作要求で無効な名前を指定すると、このエラーが返されます。  <br/> |
|ErrorADUnavailable  <br/> |このエラーは、DS がAD場合に発生します。 後でもう一度要求を試してください。  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |このエラーは **、AffectedTaskOccurrences 属性** が指定されていないかどうかを示します。 [DeleteItem](deleteitem.md)要素を使用して、タスクである少なくとも 1 つのアイテムを削除する場合、そのタスクが繰り返されるかどうかに関係なく、現在の出現または系列全体を削除するかどうかを **DeleteItem** が判断できるよう **、AffectedTaskOccurrences** 属性を指定する必要があります。  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |アーカイブ フォルダー パスの作成中のエラーを示します。  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |アーカイブ メールボックスが有効になっていないかどうかを示します。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |アーカイブ メールボックス サービスの検出に失敗したと示します。  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |入れ子になった添付ファイルが 10 件を超えるアイテムの作成が試行されたと指定します。 この値は、Exchange Server 2010 Service Pack 2 (SP2) で導入されました。  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |[CreateAttachment 要素](createattachment.md)は、Int32.MaxValue を超えるサイズの添付ファイルをバイト単位で作成しようとすると、このエラーを返します。  <br/> [GetAttachment 要素](getattachment.md)は、Int32.MaxValue を超えるサイズの既存の添付ファイルをバイト単位で取得しようとすると、このエラーを返します。  <br/> |
|ErrorAutoDiscoverFailed  <br/> |このエラーは、Exchange Web Services が、自動検出サービスを使用してクライアント アクセス サーバーの役割がインストールされている Exchange 2010 を実行しているフォレスト間コンピューターの場所を特定しようとしましたが、自動検出サービスへの呼び出しが失敗しました。  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |このエラーは、ローカル フォレストの可用性構成情報が DS に存在ADします。  <br/> |
|ErrorBatchProcessingStopped  <br/> | このエラーは、アイテムの処理中に例外が発生し、その後のアイテムに対して例外が発生する可能性が高い場合を示します。 要求には複数のアイテムが含まれる場合があります。たとえば、GetItem 操作要求には複数の識別子が含まれる場合があります。 一般に、アイテムは一度に 1 つ処理されます。 アイテムの処理中に例外が発生し、その後のアイテムに対して例外が発生する可能性がある場合、その後のアイテムは処理されません。  <br/><br/>  次に、次のアイテムの処理を停止するエラーの例を示します。<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |このエラーは、定期的な予定表アイテムを移動またはコピーしようとすると発生します。  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | このエラーは、削除済みアイテム フォルダー内にある予定表アイテムの更新を試み、会議の更新または取り消しが **SendMeetingInvitationsOrCancellations** 属性の値に従って送信される場合に発生します。 <br/><br/>次に、この属性で使用できる値を示します。  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>ただし、このような更新は、この属性の値が SendToNone に設定されている場合にのみ許可されます。  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |このエラーは、UpdateItem、GetItem、DeleteItem、MoveItem、CopyItem、または SendItem 操作が呼び出され、指定された ID が定期的な予定表アイテムの出現 ID ではない場合に発生します。  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |このエラーは、UpdateItem、GetItem、DeleteItem、MoveItem、CopyItem、または **SendItem** 操作が呼び出され、指定された ID が定期的なマスター アイテムの ID ではない場合に発生します。      <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |このエラーは、予定表アイテムの期間が最大許容期間 (現在は 5 年) よりも長い場合に **、CreateItem** 操作または **UpdateItem** 操作中に発生します。  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |このエラーは、カレンダーの終了時刻が同じ時刻または開始時刻の後に設定されている場合に発生します。  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |このエラーは [、CalendarView](calendarview.md)要素を持つ **FindItem** 操作の指定したフォルダーが予定表フォルダーの種類ではない場合に発生します。  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |このエラーは、時刻の変更パターンを定義するために Day、WeekendDay、および Weekday の無効な値が使用されている場合に **、CreateItem** 操作または **UpdateItem** 操作中に発生します。  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |このエラーは、 **日、WeekDay、** および WeekendDay の無効な値を使用して週単位の繰り返しを指定すると **、CreateItem** 操作または UpdateItem 操作中に発生します。  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |このエラーは、予定表アイテムの定期的なバイナリ ラージ オブジェクト (BLOB) の状態が無効Exchange発生します。  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |このエラーは、指定した繰り返しを作成できない場合に発生します。  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |このエラーは、無効なタイム ゾーンが検出された場合に発生します。  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |このエラー 予定表アイテムが取り消されたかどうかを示します。  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |このエラーは、予定表アイテムが取り消されたかどうかを示します。  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |このエラーは、予定表アイテムが取り消されたかどうかを示します。  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |このエラーは、予定表アイテムが取り消されたかどうかを示します。  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |このエラーは、委任されたシナリオの予定表アイテムまたは会議出席依頼に対して [AcceptItem](acceptitem.md) 要素が無効です。  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |このエラーは、委任されたシナリオの予定表アイテムまたは会議出席依頼に対して [DeclineItem](declineitem.md) 要素が無効です。  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |このエラーは、委任されたシナリオでの会議の取り消しに対して [RemoveItem](removeitem.md) 要素が無効です。  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |このエラーは、代理シナリオの予定表アイテムまたは会議出席依頼に対して [TentativelyAcceptItem](tentativelyacceptitem.md) 要素が無効です。  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |このエラーは、予定表アイテムの操作 (現在は CancelItem) が出席者に対して無効です。 会議をキャンセルできるのは、会議の開催者のみです。  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |このエラーは、 [開催者の予定表](acceptitem.md) アイテムに対して AcceptItem が無効です。  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |このエラーは、 [開催者の予定表](declineitem.md) アイテムに対して DeclineItem が無効かどうかを示します。  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |このエラーは、 [開催者の予定表](removeitem.md) アイテムに対して RemoveItem が無効です。 予定表から会議を削除するには、開催者が CancelCalendarItem を使用する必要があります。  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |このエラーは、 [開催者の予定表アイテムに対して TentativelyAcceptItem](tentativelyacceptitem.md) が無効です。  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |このエラーは、会議出席依頼が古く、更新できないことを示します。  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |このエラーは、オカレンス インデックスが現在の繰り返し内のオカレンスを指していない状態を示します。 たとえば、定期的なパターンで 3 つの会議の発生のセットが定義され、5 番目のイベントにアクセスしようとすると、この応答コードが生成されます。  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |このエラーは、削除されたオカレンス (定期的なマスター ID とオカレンス インデックスを介してアドレス指定された) に対する操作が無効かどうかを示します。  <br/> |
|ErrorCalendarOutOfRange  <br/> |このエラーは、プロパティ値が範囲を外れた場合に、予定表アイテムまたはタスクの定期的なプロパティの CreateItem 操作と UpdateItem 操作で報告されます。 たとえば、月の 15 週目を指定すると、この応答コードが生成されます。  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |このエラーは [、CalendarView](calendarview.md) 要素の Start to End の範囲が、現在 2 年の最大許容値を超える場合に発生します。  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |このエラーは、要求するアカウントがディレクトリ データベース内の有効なアカウントではないと示します。  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |予定表連絡先タスク フォルダーをアーカイブしようとしたかどうかを示します。  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |パブリック フォルダー内のアイテムをアーカイブしようとしたかどうかを示します。  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |アーカイブ メールボックス内のアイテムをアーカイブしようとしたかどうかを示します。  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |このエラーは、予定表アイテムが作成され **、SavedItemFolderId** 属性が予定表以外のフォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |このエラーは、連絡先が作成され **、SavedItemFolderId** 属性が連絡先以外のフォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |このエラーは、予定表、連絡先、タスク、メモなどのメール フォルダー以外のフォルダーに投稿アイテムを作成できないことを示します。  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |このエラーは、タスクが作成され **、SavedItemFolderId** 属性がタスク以外のフォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotDeleteObject  <br/> |このエラーは、削除するアイテムまたはフォルダーを削除できない場合に発生します。  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |[DeleteItem 操作は、](deleteitem-operation.md)定期的なタスクの現在の発生を削除できない場合に、このエラーを返します。 これは **、AffectedTaskOccurrences** 属性が SpecifiedOccurrenceOnly に設定されている場合にのみ発生します。  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |必須の拡張機能を無効にしようとしたかどうかを示します。  <br/> |
|ErrorCannotEmptyFolder  <br/> |このエラーは、サーバーがフォルダーを空にできない場合に返す必要があります。  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |ソース フォルダー パスを取得できませんでした。  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |サーバーがオプションの外部 URL を取得Outlook Web Appします。  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |**GetAttachment 操作は**、添付ファイルの本文を取得できない場合に、このエラーを返します。  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |このエラーは、呼び出し元が予定表以外のフォルダーに対する予定表のアクセス許可を設定しようとしたかどうかを示します。  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |このエラーは、呼び出し元が予定表フォルダーに予定表以外のアクセス許可を設定しようとしたかどうかを示します。  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |このエラーは、アクセス許可セットで不明なアクセス許可を設定できないことを示します。  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |検索フォルダーをソース フォルダーとして指定しようとしたかどうかを示します。  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |このエラーは、アイテム識別子を必要とする要求にフォルダー識別子が与えられた場合に発生します。  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |このエラーは、フォルダー識別子を必要とする要求にアイテム識別子が与えられた場合に発生します。  <br/> |
|ErrorChangeKeyRequired  <br/> |この応答コードは **ErrorChangeKeyRequiredForWriteOperations に置き換えられた** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |このエラーは、アイテムの変更キーが見つからないか古い場合に返されます。 <br/><br/>SendItem、UpdateItem、および UpdateFolder 操作の場合、呼び出し元はアイテムの正しい現在の変更キーを渡す必要があります。 これは、競合の解決が常に上書きに設定されている場合でも、UpdateItem の場合です。  <br/> |
|ErrorClientDisconnected  <br/> |クライアントが切断されたと指定します。  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorClientIntentNotFound  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorConnectionFailed  <br/> |このエラーは、Web サービスExchangeに接続できない場合に発生します。  <br/> |
|ErrorConnectionFailedTransientError  <br/> |このエラーは、Web サービスExchangeに接続できない場合に発生します。 このエラー コードは、一時的なエラーを示します。 このエラーを受信すると、クライアントはサーバーへの接続を再試行できます。 <br/> |
|ErrorContainsFilterWrongType  <br/> |このエラーは、Contains フィルターで検査されたプロパティが文字列型ではないかどうかを示します。  <br/> |
|ErrorContentConversionFailed  <br/> |**GetItem 操作は**、Web サービスが要求Exchange MIME コンテンツを取得できない場合に、このエラーを返します。 <br/><br/>**CreateItem 操作は**、Web サービスがExchange MIME コンテンツからアイテムを作成できない場合に、このエラーを返します。 通常、これは item プロパティが破損または切り捨てられることを示しています。  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |このエラーは、QueryString オプションを使用して検索要求を行い、ターゲット メールボックスのコンテンツ インデックス作成が有効になっていない場合に発生します。  <br/> |
|ErrorCorruptData  <br/> |このエラーは、データが破損し、処理できない場合に発生します。  <br/> |
|ErrorCreateItemAccessDenied  <br/> |このエラーは、呼び出し元がアイテムを作成するアクセス許可を持ってない場合に発生します。  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |このエラーは、CreateManagedFolder 操作要求で指定された 1 つ以上の管理フォルダーを作成できなかった場合に発生します。 各フォルダーを検索して、作成されたフォルダーと存在しないフォルダーを特定します。  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |このエラーは、呼び出し元のアカウントにサブフォルダーの作成に必要なアクセス許可が付与されていない場合に発生します。  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |このエラーは、あるメールボックスから別のメールボックスにアイテムまたはフォルダーを移動しようとすると発生します。 移行元メールボックスと移行先メールボックスが異なる場合は、このエラーが発生します。  <br/> |
|ErrorCrossSiteRequest  <br/> |このエラーは、要求を処理する必要があるクライアント アクセス サーバーが別のサイトに含まれるため、要求が許可されないかどうかを示します。  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |このエラーは、次のシナリオで発生する可能性があります。<br/>  <br/>- アイテムのプロパティにアクセスまたは書き込もうとすると、プロパティ値が大きすぎます。<br/>- 要求 XML 内の base64 エンコードされた MIME コンテンツの長さが制限を超えています。<br/>- 既存のアイテム本文の本文のサイズが制限を超えています。<br/>- コンシューマは、長さ (または追加の場合は結合された長さ) が制限を超える HTML またはテキスト本文を設定します。 |
|ErrorDataSourceOperation  <br/> |このエラーは、基になるデータ プロバイダーが操作を完了できない場合に発生します。  <br/> |
|ErrorDelegateAlreadyExists  <br/> |このエラーは、指定したユーザーが代理人の一覧に既に存在する場合に **AddDelegate** 操作で発生します。  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |このエラーは、追加する指定されたユーザーがメールボックスの所有者である場合に **AddDelegate** 操作で発生します。  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |このエラーは **、GetDelegate** 操作で、ローカルの FreeBusy メッセージに代理人情報がない場合、または Active Directory パブリック デリゲートが存在しない場合 (AD DS で "パブリック 代理人" または "Send On Behalf" エントリがない場合に発生します。  <br/> |
|ErrorDelegateNoUser  <br/> |このエラーは、指定したユーザーを DS 内のユーザーにマップできない場合ADされます。  <br/> |
|ErrorDelegateValidationFailed  <br/> |このエラーは、追加された代理人ユーザーが無効な場合に **AddDelegate** 操作で発生します。  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |このエラーは、識別フォルダーの削除が試行された場合に発生します。  <br/> |
|ErrorDeleteItemsFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |このエラーは、識別されたユーザー ID が操作に対して無効です。 **DistinguishedUserType** は、要求に存在しない必要があります。  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |このエラーは、要求配布リスト のメンバーが配布リストに存在しないかどうかを示します。  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |このエラーは **、CreateManagedFolder** 操作要求の [FolderNames](foldernames.md)要素内で重複するフォルダー名が指定されている場合に発生します。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |このエラーは、重複する SOAP ヘッダーが含まれるかどうかを示します。  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |このエラーは、アクセス許可セットで重複するユーザー ID が見つかったか、Default または Anonymous が 2 回以上設定されている、または重複する ID または受信者が含まれるかどうかを示します。  <br/> |
|ErrorEmailAddressMismatch  <br/> |このエラーは、要求が検索フォルダーの検索パラメーターを作成または更新しようとするときに発生します。 たとえば、検索フォルダーがメールボックス内に作成されているが、検索フォルダーが別のメールボックスを検索する場合に発生することがあります。  <br/> |
|ErrorEventNotFound  <br/> |このエラーは、透かしに関連付けられているイベントがイベントが返される前に削除された場合に発生します。 このエラーが返された場合、サブスクリプションも削除されます。  <br/> |
|ErrorExceededConnectionCount  <br/> |このエラー -iIndicates は、ユーザーのポリシーで許可されているよりも、サーバーに対する同時要求の数が多いという問題を示します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |このエラーは、ユーザーの調整ポリシーのサブスクリプションの最大数を超えたかどうかを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |このエラーは、検索操作呼び出しが返されるアイテムの総数を超えたと示します。  <br/> |
|ErrorExpiredSubscription  <br/> |このエラーは、サブスクリプションが期限切れになった [ため、GetEvents](getevents-operation.md) 操作が削除中として呼び出された場合に発生します。  <br/> |
|ErrorExtensionNotFound  <br/> |拡張機能が見つからなかったかどうかを示します。  <br/> |
|ErrorFolderCorrupt  <br/> |このエラーは、フォルダーが破損して保存できない場合に発生します。  <br/> |
|ErrorFolderExists  <br/> |このエラーは、同じ親の別のフォルダーと同じ名前のフォルダーを作成しようとすると発生します。 重複するフォルダー名は使用できません。  <br/> |
|ErrorFolderNotFound  <br/> |このエラーは、指定されたフォルダー ID が有効なフォルダーに対応していないか、代理人がフォルダーにアクセスするアクセス許可を持たなかどうかを示します。  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |このエラーは、要求されたプロパティを取得できませんでした。 これは、プロパティが存在しないが、プロパティが何らかの方法で破損して取得が失敗したという意味ではありません。  <br/> |
|ErrorFolderSave  <br/> |このエラーは、無効な状態が原因でフォルダーを作成または更新できない可能性を示します。  <br/> |
|ErrorFolderSaveFailed  <br/> |このエラーは、無効な状態が原因でフォルダーを作成または更新できない可能性を示します。  <br/> |
|ErrorFolderSavePropertyError  <br/> |このエラーは、無効なプロパティ値が原因でフォルダーを作成または更新できない可能性を示します。 応答コードには、問題の原因となるプロパティが一覧表示されます。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |このエラーは、配布リストの空き時間情報を取得するために、最大グループ メンバー数に達しました。  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |このエラーは、エラーが発生して空き時間情報を取得できない場合に返されます。  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorImContactLimitReached  <br/> |このエラーは、連絡先の最大数に達したため、新しいインスタント メッセージング (IM) 連絡先を追加できない場合に返されます。 このエラーは、2013 Exchange Serverで導入されました。  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |既存のグループに既に同じ表示名がある場合に、グループ表示名を追加しようとすると、このエラーが返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorImGroupLimitReached  <br/> |このエラーは、グループの最大数に達したため、新しい IM グループを追加できない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorImpersonateUserDenied  <br/> |呼び出し元が問題の特定のユーザーを偽装するための適切な権限を持ってない場合、Exchange 偽装のサーバー間承認ケースでエラーが返されます。 このエラーは、拡張 Active Directory 権限の ms-Exch-EPI-May-Impersonate にマップされます。  <br/> |
|ErrorImpersonationDenied  <br/> |このエラーは、Exchange 偽装に対するサーバー間認証で、発信者が要求を行っているクライアント アクセス サーバーを通じて偽装する適切な権限を持ってない場合に返されます。 これは、ms-Exch-EPI-Impersonation 拡張 Active Directory 権限にマップされます。  <br/> |
|ErrorImpersonationFailed  <br/> |このエラーは、サーバー間認証の実行が試行された際に予期しないエラーが発生しました。 通常、この応答コードは、Exchange Web Services アプリケーション プールを実行しているサービス アカウントが正しく構成されていないか、Exchange Web Services がディレクトリと通信できないか、フォレスト間の信頼が正しく構成されていないかどうかを示します。  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |このエラーは、要求が現在のバージョンのバージョンで有効Exchange Serverが、指定された要求サーバーのバージョンに対して無効だったかどうかを示します。  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |このエラーは [、UpdateItem](updateitem.md) 要素または [UpdateFolder](updatefolder.md) 要素の各変更の説明で、更新するプロパティを 1 つのみリストする必要があります。  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |このエラーは、要求に含まれる出席者が多すぎて解決できない場合に発生します。 既定では、解決する出席者の最大数は 100 です。  <br/> |
|ErrorInsufficientResources  <br/> |このエラーは、メールボックス サーバーがオーバーロードされている場合に発生します。 後でもう一度要求を試してください。  <br/> |
|ErrorInternalServerError  <br/> |このエラーは、Exchange Web サービスが回復できないというエラーが発生し、発生したエラーに関連付けられているより具体的な応答コードが存在しない場合を示します。  <br/> |
|ErrorInternalServerTransientError  <br/> |このエラーは、内部サーバー エラーが発生し、後で要求を再試行する必要があります。  <br/> |
|ErrorInvalidAccessLevel  <br/> |このエラーは、発信者が空き時間情報データに対して持つアクセスのレベルが無効です。  <br/> |
|ErrorInvalidArgument  <br/> |このエラーは [、GetMessageTrackingReport](getmessagetrackingreport-operation.md)操作に渡された無効なすべての引数によって発生したエラーを示します。<br/><br/> このエラーは、次のシナリオで返されます。 <br/><br/>-  _sending-as パラメーターで指定された_ ユーザーがディレクトリに存在しません。 <br/>-  _sending-as パラメーターで指定された_ ユーザーは、ディレクトリ内で一意ではありません。 <br/>-  _送信先アドレスが_ 空です。<br/>-  _送信アドレスが_ 有効な電子メール アドレスではありません。  <br/> |
|ErrorInvalidAttachmentId  <br/> |このエラーは、指定した ID に対応する添付ファイルが見つからない場合に [、GetAttachment](getattachment-operation.md) 操作または [DeleteAttachment](deleteattachment-operation.md) 操作によって返されます。  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |このエラーは、複雑な添付ファイル テーブルの制限を使用して既存の検索フォルダーにバインドしようとするときに発生します。 ExchangeWeb サービスは、添付ファイル テーブルに対する単純な含みフィルターのみをサポートします。 より複雑な添付ファイル テーブル制限 (サブフィルター) を持つ既存の検索フォルダーにバインドしようとする場合、Exchange Web Services は、そのフィルターの XML をレンダリングできません。この応答コードを返します。 <br/><br/>フォルダーで GetFolder 操作を呼び出すが [、SearchParameters](searchparameters.md) 要素を要求しない点に注意してください。  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |このエラーは、複雑な添付ファイル テーブルの制限を使用して既存の検索フォルダーにバインドしようとするときに発生します。 ExchangeWeb サービスは、添付ファイル テーブルに対する単純な含みフィルターのみをサポートします。 <br/><br/>より複雑な添付ファイル テーブル制限を持つ既存の検索フォルダーにバインドしようとする場合、Exchange Web サービスは、そのフィルターの XML をレンダリングできません。 この場合、添付ファイル サブフィルターにはテキスト フィルターが含まれているが、添付ファイルの表示名は表示されません。<br/><br/> フォルダーで GetFolder 操作を呼び出すが [、SearchParameters](searchparameters.md) 要素を要求しない点に注意してください。  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | このエラーは、要求者の承認手順が失敗しました。  <br/> |
|ErrorInvalidChangeKey  <br/> |このエラーは、コンシューマーが、解析できない変更キーを持つフォルダーまたはアイテム識別子を渡した場合に発生します。 たとえば、これは無効な base64 コンテンツまたは空の文字列である可能性があります。  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |このエラーは、呼び出し元の ID を解決しようとして内部エラーが発生したと示します。  <br/> |
|ErrorInvalidCompleteDate  <br/> |このエラーは、タスクの [CompleteDate](completedate.md) 要素の値を将来の時刻に設定しようとすると返されます。 クライアント アクセス サーバーのローカル時刻に変換すると、タスクの [CompleteDate](completedate.md) をクライアント アクセス サーバーのローカル時刻より後の値に設定することはできません。  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |このエラーは、連絡先に対して無効な電子メール アドレスが提供されたかどうかを示します。  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |このエラーは、電子メール エントリに無効な電子メール インデックス値が指定されたかどうかを示します。  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |このエラーは、要求を別のディレクトリ サービス フォレストにプロキシするために使用される資格情報が認証に失敗した場合に発生します。  <br/> |
|ErrorInvalidDelegatePermission  <br/> |このエラーは、指定したフォルダーのアクセス許可が無効です。  <br/> |
|ErrorInvalidDelegateUserId  <br/> |このエラーは、指定された代理人ユーザー ID が無効です。  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |このエラーは、Exchangeが UPN、電子メール アドレス、またはユーザー SID を指定しない場合に、偽装中に発生します。 これは、呼び出し元が 1 つ以上を指定し、値が空の場合にも発生します。  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |このエラーは [、Excludes](excludes.md) 要素の制限に渡されたビットマスクを解析できない場合に発生します。  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidExtendedProperty  <br/> | このエラーは、次のイベントが発生すると発生します。 <br/> <br/>- 呼び出し元は、Web サービスでサポートされていない拡張プロパティをExchangeします。  <br/>- 呼び出し元は、拡張プロパティの属性値の無効な組み合わせを渡します。 これは、属性が渡された場合にも発生します。 特定の組み合わせだけが許可されます。  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |このエラーは、拡張プロパティの value セクションがプロパティの種類と一致しない場合に発生します。 <br/><br/>たとえば、PropertyType="String" を持つ拡張プロパティを整数の配列に設定すると、このエラーが発生します。 拡張プロパティに対して指定された型に対して適用できない文字列表現では、このエラーが発生します。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |このエラーは、共有招待の送信者が共有招待メタデータを作成しなかったことを示します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |このエラーは、共有メッセージが呼び出し元を対象としていないと示します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |このエラーは、要求者の組織フェデレーション オブジェクトが正しく構成されていないかどうかを示します。  <br/> |
|ErrorInvalidFolderId  <br/> |このエラーは、フォルダー ID が破損している場合に発生します。  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |このエラーは、指定したフォルダーの種類が現在の操作に対して無効です。 たとえば、パブリック フォルダーに検索フォルダーを作成することはできません。  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | このエラーは、ユーザーが次のいずれかを指定した場合に、分数ページングで発生します。 <br/> <br/>- 分母より大きい分子  <br/>- 0 未満の分子  <br/>- 0 以下の分母  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |このエラーは [、DataType](datatype.md) 要素と ShareFolderId 要素の両方が要求に存在することを示します。  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |このエラーは [、GetUserAvailability 操作](getuseravailability-operation.md) が [FreeBusyViewType の None で呼び出された場合に](freebusyviewtype.md) 発生します。  <br/> |
|ErrorInvalidId  <br/> |このエラーは、ID キーまたは変更キーの形式が正しいかどうかを示します。  <br/> |
|ErrorInvalidIdEmpty  <br/> |このエラーは、呼び出し元が空の Id 属性 **を** 指定すると発生します。  <br/> |
|ErrorInvalidLikeRequest  <br/> |このエラーは、アイテムが気に入らない場合に発生します。 ビルド番号 15.00.0913.09 から始まるバージョンExchangeには、この値が含まれます。  <br/> |
|ErrorInvalidIdMalformed  <br/> |このエラーは、呼び出し元が形式が正しい **Id** 属性を指定すると発生します。  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |このエラーは、Exchange 2007 形式を使用しているフォルダーまたはアイテム ID が、Exchange 2007 SP1 以降のバージョンの要求に対して指定されたかどうかを示します。 Exchange 2007 の ID を Exchange 2007 SP1 以降の要求で使用することはできません。 最初に [ConvertId 操作を使用して](convertid-operation.md) 変換する必要があります。  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |このエラーは、呼び出し元が長すぎる **Id** 属性を指定すると発生します。  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |このエラーは、アイテムの添付ファイル ID ではない ID が、添付ファイル ID を必要とする Web サービス メソッドに渡されるたびに返されます。  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |このエラーは、メールボックス内の連絡先が破損している場合に発生します。  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |このエラーは、呼び出し元が長すぎる **Id** 属性を指定すると発生します。  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |アイテムの添付ファイル階層が最大 255 レベルを超えると、このエラーが返されます。  <br/> |
|ErrorInvalidIdXml  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidImContactId  <br/> |このエラーは、指定された IM 連絡先識別子が有効な識別子を表していない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |このエラーは、指定された IM 配布グループ SMTP アドレス識別子が有効な識別子を表していない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidImGroupId  <br/> |このエラーは、指定された IM グループ識別子が有効な識別子を表していない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |このエラーは、インデックス付きページングのオフセットが負の場合に発生します。  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |アイテムが ArchiveItem 操作に対して無効 **だったかどうかを示** します。  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |このエラーは、会議出席依頼や予定表アイテム以外のアイテムの種類に AcceptItem 応答オブジェクトを使用しようとした場合、または [削除済みアイテム] フォルダーにある予定表アイテムの出現を受け入れしようとすると発生します。  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |このエラーは、予定表アイテム以外のアイテムの種類で CancelItem 応答オブジェクトを使用しようとした場合に発生します。  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | サポートされていない種類のアイテム添付ファイルを作成しようとすると、このエラーが返されます。  <br/><br/>  アイテム添付ファイルでサポートされているアイテムの種類には、次のオブジェクトが含まれます。  <br/><br/>- [アイテム](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [タスク](task.md) <br/>- [連絡先](contact.md) <br/> <br/> たとえば [、MeetingMessage](meetingmessage.md) 添付ファイルを作成しようとすると、この応答コードが表示されます。  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | 要求にサポートされていないアイテムの種類が含まれている場合、このエラーは [CreateItem](createitem-operation.md) 操作から返されます。 <br/><br/>サポートされているアイテムには、次のオブジェクトが含まれます。<br/>  <br/>- [アイテム](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [タスク](task.md) <br/>- [連絡先](contact.md) <br/><br/>  特定の種類は、他の何かを行う副作用として作成されます。 たとえば、会議メッセージは、出席者に予定表アイテムを送信するときに作成されます。明示的には作成されません。  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |このエラーは、会議出席依頼や予定表アイテム以外のアイテムの種類に対して DeclineItem 応答オブジェクトを使用しようとした場合、または削除済みアイテム フォルダーにある予定表アイテムの出現を拒否しようとした場合に発生します。  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |このエラーは [、ExpandDL 操作がプライベート](expanddl-operation.md) 配布リストにのみ有効な状態を示します。  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |要求で会議の取り消しアイテムではないアイテムが指定されている場合、このエラーは RemoveItem 応答オブジェクトから返されます。  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |要求がメッセージ アイテムではないアイテムを指定した場合、このエラーは [SendItem](senditem-operation.md) 操作から返されます。  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |このエラーは、会議出席依頼や予定表アイテム以外のアイテムの種類に対して [TentativelyAcceptItem](tentativelyacceptitem.md) を使用しようとした場合、または削除済みアイテム フォルダー内にある予定表アイテムの出現を暫定的に受け入れしようとすると発生します。  <br/> |
|ErrorInvalidLogonType  <br/> |このエラーは内部でのみ使用されます。 このエラーは返されません。  <br/> |
|ErrorInvalidMailbox  <br/> |このエラーは、個人用配布リストの作成または更新中に [CreateItem](createitem-operation.md) 操作または [UpdateItem](updateitem-operation.md) 操作が失敗しました。  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |このエラーは、管理フォルダーの構造が破損し、レンダリングできない場合に発生します。  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |このエラーは、管理フォルダーに設定されているクォータが 0 未満の場合に発生します。これは、破損した管理フォルダーを示します。  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |このエラーは、管理フォルダーに設定されているサイズが 0 未満の場合に発生します。これは、破損した管理フォルダーを示します。  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |このエラーは、指定されたマージされた空き時間情報の内部値が無効な場合に発生します。 既定値は 5 分です。 既定値は 1440 分です。  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |このエラーは、ResolveNames 操作の名前が無効 [な場合に発生します](resolvenames-operation.md)。 たとえば、長さ 0 の文字列、1 つのスペース、コンマ、およびダッシュは、すべて無効な名前です。  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |このエラーは、クライアント アクセス サーバー上のネットワーク サービス アカウントのエラーを示します。  <br/> |
|ErrorInvalidOofParameter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidOperation  <br/> | これは、要求された操作が無効な場合に使用される一般的なエラーです。 <br/><br/>たとえば、次の操作は実行できません。 <br/> <br/>- パブリック フォルダーで FindFolder 操作を使用して ["Deep"](findfolder-operation.md) トラバーサルを実行します。  <br/>- パブリック フォルダールートを移動またはコピーします。  <br/>- "Hard" delete 以外のモードを使用して、関連付けられたアイテムを削除します。  <br/>- 関連付けられたアイテムを移動またはコピーします。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |このエラーは、発信者が別の組織のユーザーに空き時間情報を要求したが、組織の関係で空き時間情報が有効になっていない場合を示します。  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |このエラーは、コンシューマーが返される最大行の 0 または負の値を渡した場合に発生します。  <br/> |
|ErrorInvalidParentFolder  <br/> |このエラーは、コンシューマーが操作の無効な親フォルダーを渡した場合に発生します。 たとえば、検索フォルダー内にフォルダーを作成しようとすると、このエラーが返されます。  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |タスクの完了率を無効な値に設定しようとすると、このエラーが返されます。 値は 0 ~ 100 (含む) である必要があります。  <br/> |
|ErrorInvalidPermissionSettings  <br/> |このエラーは、アクセス許可レベルがアクセス許可設定と矛盾している場合に発生します。  <br/> |
|ErrorInvalidPhoneCallId  <br/> |このエラーは、呼び出し元の識別子が無効です。  <br/> |
|ErrorInvalidPhoneNumber  <br/> |このエラーは、電話番号が正しく設定されていないか、ダイヤル プランルールに適合しないかどうかを示します。  <br/> |
|ErrorInvalidPropertyAppend  <br/> | このエラーは、追加しようとしているプロパティが追加をサポートしていない場合に発生します。 <br/><br/>追加をサポートする唯一のプロパティを次に示します。 <br/> <br/>- 受信者コレクション (ToRecipients、CcRecipients、BccRecipients)  <br/>- Attendee コレクション (RequiredAttendees、OptionalAttendees、Resources)  <br/>- Body  <br/>- ReplyTo  <br/><br/>  さらに、要求で指定された形式がストア内のアイテムの形式と一致しない場合、メッセージ本文が追加された場合に、このエラーが発生します。  <br/> |
|ErrorInvalidPropertyDelete  <br/> |このエラーは、削除操作をサポートしていないプロパティの [UpdateItem](updateitem-operation.md) 操作または [UpdateFolder](updatefolder-operation.md) 操作呼び出しで削除操作が指定されている場合に発生します。 たとえば[、Item](item.md)オブジェクトの[ItemId](itemid.md)要素を削除することはできません。  <br/> |
|ErrorInvalidPropertyForExists  <br/> |このエラーは、コンシューマーが Exists フィルターのフラグ プロパティの 1 つを渡した場合 [に発生](exists.md) します。 たとえば [、IsRead](isread.md) フラグまたは [IsFromMe](isfromme.md) フラグが Exists 要素で指定されている場合、このエラー [が発生](exists.md) します。 要求はフラグであるため、単一のプロパティの一部であるため [、IsEqualTo](isequalto.md) 要素を代わりに使用する必要があります。  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |このエラーは、操作しようとしているプロパティが、操作中の操作をサポートしていない場合に発生します。  <br/> |
|ErrorInvalidPropertyRequest  <br/> | このエラーは、要求で指定されたプロパティがアイテムの種類で使用できない場合に発生します。 たとえば、予定表アイテムでのみ使用できるプロパティが、メッセージの [GetItem](getitem-operation.md) 操作呼び出しで要求された場合、またはメッセージの [UpdateItem](updateitem-operation.md) 操作呼び出しで更新された場合に、このエラーが返されます。 <br/> <br/>  これは、次の操作で発生します。 <br/> <br/>- [GetItem 操作](getitem-operation.md) <br/>- [GetFolder 操作](getfolder-operation.md) <br/>- [UpdateItem 操作](updateitem-operation.md) <br/>- [UpdateFolder 操作](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |このエラーは、操作しようとしているプロパティが、操作中の操作をサポートしていないことを示します。 たとえば、設定しようとしているプロパティが読み取り専用の場合、このエラーが返されます。  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | このエラーは、クライアントが既に送信されたメッセージの特定のプロパティを更新しようとするときに [、UpdateItem](updateitem-operation.md) 操作中に発生します。<br/><br/> たとえば、送信されたメッセージで次のプロパティを更新できません。 <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |このエラーは、プッシュ サブスクリプション ID を使用して [GetEvents 操作](getevents-operation.md) または [Unsubscribe](unsubscribe-operation.md) 操作を呼び出した場合に発生します。 プッシュ サブスクリプションの登録を解除するには、購読解除応答を使用してプッシュ要求に応答するか、Web サービスを切断してプッシュ通知がタイム アウトするのを待つ必要があります。  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | このエラーは、"プッシュ"[](subscribe-operation.md)サブスクリプションを作成し、要求に含まれる URL が無効である場合に、Subscribe 操作によって返されます。<br/><br/>Web サービスが URL を受け入れるにはExchange条件を満たしている必要があります。 <br/> <br/>- 文字列の長 \> さ 0 \< 2083.  <br/> と - プロトコルは http または https です。  <br/>- URL は、Microsoft の URI クラスで解析.NET Frameworkできます。  <br/> |
|ErrorInvalidRecipients  <br/> |このエラーは、メッセージの受信者コレクションまたは予定表アイテムの出席者コレクションが無効です。 たとえば、受信者が含まれるアイテムを送信しようとすると、このエラーが返されます。  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |このエラーは、検索フォルダーに Web サービスで表Exchange受信者テーブル フィルターが含まれるかどうかを示します。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |このエラーは、検索フォルダーに Web サービスで表Exchange受信者テーブル フィルターが含まれるかどうかを示します。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |このエラーは、検索フォルダーに Web サービスで表Exchange受信者テーブル フィルターが含まれるかどうかを示します。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |このエラーは、検索フォルダーに Web サービスで表Exchange受信者テーブル フィルターが含まれるかどうかを示します。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|ErrorInvalidReferenceItem  <br/> | このエラーは、次のシナリオで Forward 応答オブジェクトと Reply 応答オブジェクトの [CreateItem](createitem-operation.md) 操作から返されます。<br/>  <br/>- 参照されるアイテム識別子は [、Message、CalendarItem、](message-ex15websvcsotherref.md)または **Message** または [CalendarItem](calendaritem.md)の子孫 **ではありません**。  <br/>- 参照アイテム識別子は **CalendarItem** 用で、オーガナイザーは自分自身に返信または ReplyAll を試みている。  <br/>- メッセージが下書きで、Reply または ReplyAll が選択されています。  <br/>- [SuppressReadReceipt](suppressreadreceipt.md)の参照項目は **、メッセージ** または Message の子孫 **ではありません**。  <br/> |
|ErrorInvalidRequest  <br/> |このエラーは、SOAP 要求に SOAP アクション ヘッダーがあるが、SOAP 本文には何も含めなかった場合に発生します。 Web サービスが SOAP 本文のルート要素のローカル名から呼び出すメソッドをExchange、SOAP Action ヘッダーは必要ありません。  <br/> |
|ErrorInvalidRestriction  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |このエラーは、指定した保持タグに関連付けられているアクションが正しくない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |**PolicyTag** プロパティに存在しないタグまたは非表示のタグを設定しようとすると、このエラーが返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |PolicyTag プロパティに暗黙的なタグを設定しようとすると、このエラー **が返** されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |保持タグ GUID が無効だったかどうかを示します。  <br/> |
|ErrorInvalidRoutingType  <br/> |このエラーは [、RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) 要素に渡されるルーティングの種類が無効な場合に発生します。 通常、ルーティングの種類は簡易メール転送プロトコル (SMTP) に設定されます。  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |このエラーは、指定した期間の終了時刻が開始時刻より長くなか、将来終了時刻が発生しない場合に発生します。  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |このエラーは、別のサーバーに送信されたプロキシ要求がバージョン管理の不一致のために要求にサービスを提供できない状態を示します。  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |このエラーは、ストアExchange予定表フォルダーのセキュリティ記述子が破損している可能性を示します。  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |このエラーは、要求で [SavedItemFolderId](saveditemfolderid.md) が指定されているが **SaveItemToFolder** プロパティが false に設定されているアイテムを送信しようとして発生 **します**。  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |このエラーは、ヘッダーで渡されたトークンの形式が正しくありませんか、ディレクトリ内の有効なアカウントを参照していないか、プライマリ グループ **ConnectingSID** が存在しないかどうかを示します。  <br/> |
|ErrorInvalidSharingData  <br/> |このエラーは、共有メタデータが無効な状態を示します。 これは、XML が無効な場合に発生する可能性があります。  <br/> |
|ErrorInvalidSharingMessage  <br/> |このエラーは、共有メッセージが無効かどうかを示します。 これは、プロパティが見つからない場合に発生する可能性があります。  <br/> |
|ErrorInvalidSid  <br/> |このエラーは、要求で無効な SID が渡された場合に発生します。  <br/> |
|ErrorInvalidSIPUri  <br/> |このエラーは、SIP 名、ダイヤル プラン、または電話番号が無効な SIP URI を示します。  <br/> |
|ErrorInvalidServerVersion  <br/> |このエラーは、要求で無効な要求サーバーのバージョンが指定されたかどうかを示します。  <br/> |
|ErrorInvalidSmtpAddress  <br/> |このエラーは、SMTP アドレスを解析できない場合に発生します。  <br/> |
|ErrorInvalidSubfilterType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubscription  <br/> |このエラーは、サブスクリプションが無効になったかどうかを示します。 これは、クライアント アクセス サーバーが再起動中か、サブスクリプションの有効期限が切れているためです。  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |このエラーは、サブスクライブ要求に複数のパブリック フォルダーの ID が含まれているかどうかを示します。 サブスクリプションには、同じメールボックスまたは 1 つのパブリック フォルダー ID から複数のフォルダーを含めできます。  <br/> |
|ErrorInvalidSyncStateData  <br/> |渡された SyncState データが無効な場合、このエラーは[SyncFolderItems](syncfolderitems.md)または[SyncFolderHierarchy](syncfolderhierarchy.md)によって返されます。 [](syncstate-ex15websvcsotherref.md) このエラーを修正するには、同期状態なしで再同期する必要があります。 同期状態 BLOB を永続化する場合は、誤って BLOB を切り捨てないかどうかを確認します。  <br/> |
|ErrorInvalidTimeInterval  <br/> |このエラーは、指定された時間間隔が無効です。 開始時刻は終了時刻以上である必要があります。  <br/> |
|ErrorInvalidUserInfo  <br/> |このエラーは、アクセス許可操作に対して内部的に矛盾した [UserId](userid.md) が指定されたかどうかを示します。 たとえば、識別されたユーザー ID が指定されている場合 (Default または Anonymous)、このユーザーの SID またはプライマリ SMTP アドレスまたは表示名も指定しようとすると、このエラーが返されます。  <br/> |
|ErrorInvalidUserOofSettings  <br/> |このエラーは、内部または外部の返信がOffice(OOF) 設定が無効なユーザーを示します。  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |このエラーは、偽装のExchange発生します。 呼び出し元は、ディレクトリ内でアクセスできない SOAP ヘッダー内の無効な UPN で渡されました。  <br/> |
|ErrorInvalidUserSid  <br/> |このエラーは、要求で無効な SID が渡された場合に発生します。  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidValueForProperty  <br/> |このエラーは、比較対象のプロパティの制限の比較値が無効です。<br/><br/> たとえば [、DateTimeCreated](datetimecreated.md)true の比較値  >  **は、** この応答コードを返します。 <br/><br/>比較で列挙プロパティを指定した場合も、この応答コードが返されますが、比較する値は、その列挙体の有効な値ではありません。  <br/> |
|ErrorInvalidWatermark  <br/> |このエラーは、無効な透かしが原因です。  <br/> |
|ErrorIPGatewayNotFound  <br/> |このエラーは、有効な VoIP ゲートウェイが使用できない状態を示します。  <br/> |
|ErrorIrresolvableConflict  <br/> |このエラーは、競合解決でプロパティの変更を解決できなかった場合に発生します。 ストア内のアイテムが変更され、更新する必要がある場合があります。 更新された変更キーを取得し、もう一度やり直してください。  <br/> |
|ErrorItemCorrupt  <br/> |このエラーは、オブジェクトの状態が破損し、取得できないことを示します。 アイテムを取得する場合、Body や[MimeContent](mimecontent.md)など、特定の[](body.md)要素だけがこの状態になります。 これらの要素を省略し、操作を再試行します。  <br/> |
|ErrorItemNotFound  <br/> |このエラーは、アイテムが見つからないか、アイテムにアクセスする権限を持っていない場合に発生します。  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |このエラーは、アイテムのプロパティ要求が失敗した場合に発生します。 プロパティが存在する可能性がありますが、取得できませんでした。  <br/> |
|ErrorItemSave  <br/> |このエラーは、アイテムまたはフォルダーの保存が失敗した場合に発生します。  <br/> |
|ErrorItemSavePropertyError  <br/> |このエラーは、無効なプロパティ値が原因でアイテムまたはフォルダーの保存が失敗した場合に発生します。 応答コードには、無効なプロパティのパスが含まれています。  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotmerged  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |このエラーは、可用性サービスがネットワーク サービスとしてログオンして、適切なサイトまたはフォレストに要求をプロキシできなかったかどうかを示します。 通常、この応答は構成エラーを示します。  <br/> |
|ErrorMailboxConfiguration  <br/> |このエラーは、DS 内のメールボックス情報AD正しく構成されていることを示します。  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |このエラーは、要求内の [MailboxDataArray](mailboxdataarray.md) 要素が空です。 少なくとも 1 つのメールボックス識別子を指定する必要があります。  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |このエラーは [、MailboxDataArray](mailboxdataarray.md) 要素に 100 を超えるエントリが指定されている場合に発生します。  <br/> |
|ErrorMailboxFailover  <br/> |このエラーは、メールボックスがフェールオーバー プロセス中のため、メールボックスにアクセスしようとして失敗したと示します。  <br/> |
|ErrorMailboxHoldNotFound  <br/> |メールボックスの保持が見つからなかったかどうかを示します。  <br/> |
|ErrorMailboxLogonFailed  <br/> |このエラーは、予定表ビュー情報を取得するメールボックスへの接続が失敗した場合に発生します。  <br/> |
|ErrorMailboxMoveInProgress  <br/> | このエラーは、メールボックスが別のメールボックス ストアまたはサーバーに移動中であること示します。 このエラーは、メールボックスが別のサーバーまたはメールボックス データベース上に含まれる可能性があります。  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | このエラーは、次のいずれかのエラー状態が発生したと示します。  <br/><br/>- メールボックス ストアが壊れています。  <br/>- メールボックス ストアが停止中です。  <br/>- メールボックス ストアがオフラインです。  <br/>- メールボックス ストアへのアクセスが試行された際にネットワーク エラーが発生しました。  <br/>- メールボックス ストアがオーバーロードされ、それ以上の接続を受け入れできません。  <br/>- メールボックス ストアが一時停止されました。  <br/> |
|ErrorMailRecipientNotFound  <br/> |このエラーは [、MailboxData](mailboxdata.md) 要素情報を有効なメールボックス アカウントにマップできない場合に発生します。  <br/> |
|ErrorMailTipsDisabled  <br/> |このエラーは、メール ヒントが無効になっているかどうかを示します。  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |このエラーは、作成しようとしている管理フォルダーがメールボックスに既に存在する場合に発生します。  <br/> |
|ErrorManagedFolderNotFound  <br/> |このエラーは、要求で指定されたフォルダー名が DS の管理フォルダー定義にマップされない場合ADされます。 DS で定義されているフォルダーの管理フォルダーのインスタンスADできます。 名前を確認し、もう一度やり直してください。  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |このエラーは、管理フォルダーのルートがメールボックスから削除されたか、管理フォルダー ルートの名前を持つ同じ親フォルダーにフォルダーが存在することを示します。 これは、ルート管理フォルダーの作成が失敗した場合にも発生します。  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |このエラーは、提案エンジンが提案を生成しようとするときに問題が発生したことを示します。  <br/> |
|ErrorMessageDispositionRequired  <br/> | このエラーは **、MessageDisposition 属性が設定** されていない場合に発生します。<br/><br/> この属性は、次の場合に必要です。 <br/> <br/>- [CreateItem 操作と](createitem-operation.md) 、作成または更新されるアイテムが Message の場合の [UpdateItem](updateitem-operation.md) [操作](message-ex15websvcsotherref.md)。  <br/>- [CancelCalendarItem、AcceptItem、DeclineItem、](cancelcalendaritem.md)[または仮のAcceptItem 応答](tentativelyacceptitem.md)オブジェクト。 [](acceptitem.md) [](declineitem.md)  <br/> |
|ErrorMessageSizeExceeded  <br/> |このエラーは、送信しようとしているメッセージが許可されている制限を超えていることを示します。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |このエラーは、指定されたドメインが見つからないかどうかを示します。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |このエラーは、メッセージ追跡サービスがメッセージを追跡できないことを示します。  <br/> |
| ErrorMessageTrackingTransientError  <br/> |このエラーは、メッセージ追跡サービスがダウンまたはビジー状態を示します。 このエラー コードは、一時的なエラーを示します。 このエラーを受信すると、クライアントはサーバーへの接続を再試行できます。  <br/> |
|ErrorMimeContentConversionFailed  <br/> |このエラーは、MIME コンテンツが CreateItem 操作の有効な iCal でない [場合に発生します](createitem-operation.md)。 [GetItem 操作の場合、](getitem-operation.md)この応答は MIME コンテンツを生成できないと示します。  <br/> |
|ErrorMimeContentInvalid  <br/> |このエラーは、MIME コンテンツが無効な場合に発生します。  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |このエラーは、要求内の MIME コンテンツが有効な基本 64 文字列でない場合に発生します。  <br/> |
|ErrorMissingArgument  <br/> |このエラーは、要求に必要な引数が見つからないかどうかを示します。 応答メッセージ のテキストは、チェックする引数を示します。  <br/> |
|ErrorMissingEmailAddress  <br/> |このエラーは、要求に識別フォルダー ID を指定したが、要求を行ったアカウントにシステム上にメールボックスが存在しない場合を示します。 その場合は、[DistinguishedFolderId] の下に Mailbox サブ要素[を指定する必要があります](distinguishedfolderid.md)。 [](mailbox.md)  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |このエラーは、要求に識別フォルダー ID を指定したが、要求を行ったアカウントにシステム上にメールボックスが存在しない場合を示します。 その場合は、[DistinguishedFolderId] の下に Mailbox サブ要素[を指定する必要があります](distinguishedfolderid.md)。 [](mailbox.md) この応答は [CreateManagedFolder 操作から返されます](createmanagedfolder-operation.md)。  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |このエラーは [、EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) 要素が見つからない場合に発生します。  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |このエラーは [、ReferenceItemId が見つからない](referenceitemid.md) 場合に発生します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラー コードは返されません。  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |このエラーは [、CreateAttachment](createattachment-operation.md)操作要求の **ItemAttachment** 要素に item 要素を含めない試みがある場合に返されます。  <br/> |
|ErrorMissingManagedFolderId  <br/> |このエラーは、フォルダーのポリシー IDs プロパティ、プロパティ 0x6732が存在しない場合に発生します。 これは破損したフォルダーと見なす必要があります。  <br/> |
|ErrorMissingRecipients  <br/> |このエラーは、受信者を含めずにアイテムを送信しようとしたかどうかを示します。 メッセージの送信を引き起こすメッセージ処理を使用して [CreateItem](createitem-operation.md) 操作を呼び出す場合は、次の応答コード **ErrorInvalidRecipients** を取得します。  <br/> |
|ErrorMissingUserIdInformation  <br/> |このエラーは [、UserId](userid.md) がアクセス許可セットで完全に指定されていないかどうかを示します。  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |このエラーは、要求内で複数の [ExchangeImpersonation](exchangeimpersonation.md) 要素の値を指定したと示します。  <br/> |
|ErrorMoveCopyFailed  <br/> |このエラーは、移動操作またはコピー操作が失敗したかどうかを示します。 移動は、削除済みアイテム フォルダーにある会議出席依頼を受け入れるときに [CreateItem](createitem-operation.md) 操作で行われます。 また、会議出席依頼を拒否したり、予定表アイテムをキャンセルしたり、予定表から会議を削除したりすると、その会議は [削除済みアイテム] フォルダーに移動されます。  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |このエラーは、識別フォルダーを移動しようとして発生します。  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |このエラーは、要求が複数のメールボックス サーバーにアクセスしようとするときに発生します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |このエラーは [、ResolveNames](resolvenames-operation.md) 操作が複数の結果を返す場合、または指定したあいまいな名前がディレクトリ内の複数のオブジェクトと一致する場合に発生します。 応答コードには、応答データに一致する名前が含まれます。  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |このエラーは、呼び出し元がシステムにメールボックスを持たなかっているかどうかを示します。 [ResolveNames 操作または](resolvenames-operation.md) [ExpandDL 操作は](expanddl-operation.md)、メールボックスのないユーザーを接続する場合は無効です。  <br/> |
|ErrorNameResolutionNoResults  <br/> |このエラーは [、ResolveNames 操作が結果](resolvenames-operation.md) を返すかどうかを示します。  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |要求を処理するサーバーが Web サービスで見つからない場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorNoCalendar  <br/> |このエラーは、メールボックスの予定表フォルダーがない場合に発生します。  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |このエラーは、要求が別の Active Directory サイトのメールボックスを参照したが、移行先サイト内のクライアント アクセス サーバーが Windows 認証用に構成されていないので、要求をプロキシで処理できないという結果を示します。  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照したが、移行先サイトのクライアント アクセス サーバーが SSL 接続用に構成されていないので、要求をプロキシで処理できないという結果を示します。  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照したが、移行先サイト内のクライアント アクセス サーバーが要求を受け取る許容可能な製品バージョンで、要求をプロキシで処理できない場合を示します。  <br/> |
|ErrorNoFolderClassOverride  <br/> |このエラーは、汎用フォルダー以外のアイテムを作成するときに [FolderClass](folderclass.md) 要素を設定した場合に発生します。 [CalendarFolder](calendarfolder.md)や[TasksFolder](tasksfolder.md)などの型指定されたフォルダーの場合、フォルダー クラスは暗黙的に指定されます。 [UpdateFolder](updatefolder-operation.md)操作を使用してフォルダー クラスを別のフォルダーの種類に設定すると **、ErrorObjectTypeChanged** 応答が返されます。 代わりに、汎用フォルダーの種類を使用しますが、フォルダー クラスを必要な値に設定します。 ExchangeWeb サービスは、正しい強く型指定されたフォルダーを作成します。  <br/> |
|ErrorNoFreeBusyAccess  <br/> |このエラーは、呼び出し元が問題の予定表フォルダーに空き時間情報表示権限を持たないかどうかを示します。  <br/> |
|ErrorNonExistentMailbox  <br/> | このエラーは、次のシナリオで発生します。 <br/> <br/>- [CreateManagedFolder](createmanagedfolder.md)の電子メール アドレスが空です。  <br/>- 電子メール アドレスは、本文または SOAP ヘッダー内の電子メール アドレスを受け取る要求 (Exchange 偽装呼び出しなど) の有効なアカウントを参照していない。  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |このエラーは、発信者がプライマリ以外の SMTP アドレスを渡した場合に発生します。 応答には、使用する正しい SMTP アドレスが含まれています。  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |このエラーは、カスタム範囲の MAPI プロパティを、0x8000タグで参照できないことを示します。 PropertySetId 属性を持つ EWS マネージ API [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)プロパティまたは EWS [ExtendedFieldURI](extendedfielduri.md) 要素を使用する必要があります。  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |この応答コードは使用されません。  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |パブリック フォルダー サーバーが使用できない場合、または呼び出し元にホーム パブリック サーバーがない場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照したが、そのサイト内のクライアント アクセス サーバーのいずれも応答し、要求をプロキシで処理できないという結果を示します。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |このエラーは、呼び出し元が予定表フォルダーまたは連絡先フォルダー内のアクセス許可を別の組織のユーザーに付与しようとして、試行が失敗したことを示します。  <br/> |
|ErrorNotDelegate  <br/> |このエラーは、ユーザーがメールボックスの代理人ではないかどうかを示します。 [GetDelegate 操作、RemoveDelegate](getdelegate-operation.md)操作、[および UpdateDelegate](updatedelegate-operation.md)操作によって、指定された代理人ユーザーが代理人の一覧に見つからない場合に返されます。 [](removedelegate-operation.md)  <br/> |
|ErrorNotEnoughMemory  <br/> |このエラーは、メモリ不足のため、操作を完了できないと示します。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |このエラーは、共有メッセージがサポートされていない状態を示します。  <br/> |
|ErrorObjectTypeChanged  <br/> |このエラーは、オブジェクトの種類が変更された場合に発生します。  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |このエラーは、オカレンスの[](end-ex15websvcsotherref.md)[開始](start.md)時刻または終了時刻が更新され、対応する以前または次の発生よりも前または後で発生する予定が発生する場合に発生します。  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |このエラーは、指定された出現回数の時間の指定が、同じ定期的なアイテムの別の出現と重なって表示されます。 この応答は、指定された出現の長さ (分) が Int32.MaxValue よりも大きい場合にも発生します。  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |このエラーは、現在の操作がパブリック フォルダー ルートに対して無効な状態を示します。  <br/> |
|ErrorOrganizationNotFederated  <br/> |このエラーは、要求者の組織がフェデレーションされていないので、要求者は外部ユーザーに送信する共有メッセージを作成できないか、外部ユーザーから受信した共有メッセージを受け入れできないことを示します。  <br/> |
|ErrorParentFolderIdRequired  <br/> |この応答コードは使用されません。  <br/> |
|ErrorParentFolderNotFound  <br/> |このエラーは、親フォルダーが見つからない場合に [CreateFolder](createfolder-operation.md) 操作で発生します。  <br/> |
|ErrorPasswordChangeRequired  <br/> |このエラーは、このメールボックスにアクセスする前にパスワードを変更する必要があります。 これは、新しいアカウントが作成され、管理者がユーザーが最初のログオン時にパスワードを変更する必要があるというメッセージが表示された場合に発生します。 Web サービスを使用してパスワードExchangeすることはできません。 パスワードを変更するには、Web アプリMicrosoft Office Outlookツールを使用する必要があります。  <br/> |
|ErrorPasswordExpired  <br/> |このエラーは、パスワードの有効期限が切れたかどうかを示します。 Web サービスを使用してパスワードをExchangeすることはできません。 パスワードを変更するには、Outlook Web Appツールを使用する必要があります。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |このエラーは、要求者が予定表または連絡先フォルダー内のアクセス許可を外部ユーザーに付与しようとしましたが、要求者に割り当てられた共有ポリシーは、要求されたアクセス許可レベルが共有ポリシーで許可される権限よりも高いことを示します。  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |このエラーは、電話番号が正しい形式で表示されていないかどうかを示します。  <br/> |
|ErrorPropertyUpdate  <br/> |このエラーは、無効なプロパティ値が原因で更新が失敗しました。 応答メッセージには、無効なプロパティ パスが含まれています。  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorPropertyValidationFailure  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |このエラーは、要求が別のクライアント アクセス サーバーに存在するサブスクリプションを参照したが、そのクライアント アクセス サーバーに要求をプロキシしようとしたが失敗したと示します。  <br/> |
|ErrorProxyCallFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照し、元の呼び出し元が 3,000 グループを超えるメンバーを示します。  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |このエラーは[、GetUserAvailabilityRequest](getuseravailabilityrequest.md)要求Exchange実行しようとするときに別のクライアント アクセス サーバーに送信された Web サービスに対する要求が無効だったことを示します。 通常、この応答コードは、構成エラーまたは権限エラーが発生したこと、または可用性プロキシ要求の模倣に失敗したユーザーを示します。  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |このエラーは、Web サービスExchange要求をフルフィルメントのために別のクライアント アクセス サーバーにプロキシしようとしたが、要求が失敗したことを示します。 この応答は、ネットワーク接続の問題や要求のタイムアウトの問題によって発生する可能性があります。  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |このエラー コードは、要求がターゲット サーバーで実行されるのか、別のサーバーにプロキシされるのかを Web サービスが判断できない場合に返す必要があります。  <br/> |
|ErrorProxyTokenExpired  <br/> |この応答コードは使用されません。  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |このエラーは、パブリック フォルダー メールボックスの URL が見つからない場合に発生します。 このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |このエラーは、パブリック フォルダーへのアクセスが試行され、試行が失敗した場合に発生します。 このエラーは、2013Exchange Server 2013 Exchangeで導入されました。  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |このエラーは[、GetUserAvailability](getuseravailability-operation.md)操作に渡された受信者が、Exchange 2007 より前のバージョンの Exchange Server を実行しているコンピューター上にあり、パブリック フォルダー サーバーから受信者の空き時間情報を取得する要求が失敗した場合に発生します。  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |このエラーは[、GetUserAvailability](getuseravailability-operation.md)操作に渡された受信者が、Exchange 2007 より前のバージョンの Exchange Server を実行しているコンピューター上にあり、組織単位にパブリック フォルダー サーバーが関連付けなかったため、パブリック フォルダー サーバーから受信者の空き時間情報を取得する要求が失敗した場合に発生します。  <br/> |
|ErrorPublicFolderSyncException  <br/> |このエラーは、プライマリ パブリック フォルダー メールボックスに対して同期操作が成功したが、セカンダリ パブリック フォルダー メールボックスに対して成功しない場合に発生します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorQueryFilterTooLong  <br/> |このエラーは、検索フォルダーの制限が有効な可能性がありますが、EWS ではサポートされていません。 ExchangeWeb サービスは、制限を最大 255 のフィルター式に制限します。 255 を超える既存の検索フォルダーにバインドしようとすると、この応答コードが返されます。  <br/> |
|ErrorQuotaExceeded  <br/> |このエラーは、メールボックス のクォータを超えたときに発生します。  <br/> |
|ErrorReadEventsFailed  <br/> |このエラーは、イベント情報の取得中にエラーが発生すると [、GetEvents](getevents-operation.md) 操作またはプッシュ通知によって返されます。 このエラーが返された場合、サブスクリプションは削除されます。 最後に既知の透かしに基づいてイベント同期を再作成します。  <br/> |
|ErrorReadReceiptNotPending  <br/> |このエラーは、メッセージ送信者がメッセージの読み取り確認を要求しなかった場合、またはメッセージが迷惑メール フォルダーにある場合に、読み取り受信を抑制しようとした場合に [、CreateItem](createitem-operation.md) 操作によって返されます。  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |このエラーは、定期的な終了日が 9/1/4500 以降の場合に発生します。  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |このエラーは、指定された繰り返しに指定された範囲に出現インスタンスが存在しない場合に発生します。  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |このエラーは、代理人が削除された後、代理人リストの保存に失敗しました。  <br/> |
|ErrorRequestAborted  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRequestStreamTooBig  <br/> | このエラーは、要求ストリームが 400 KB を超える場合に発生します。  <br/> |
|ErrorRequiredPropertyMissing  <br/> |CreateAttachment 操作要求で必要なプロパティが見つからない場合、この [エラーが返](createattachment-operation.md) されます。 見つからないプロパティ URI が応答に含まれます。  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |このエラーは、呼び出し元が ResolveNames 操作に連絡先フォルダーではないフォルダー [を指定したと示します](resolvenames-operation.md)。  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |このエラーは、呼び出し元が ResolveNames 操作に複数の連絡先フォルダー [を指定したと示します](resolvenames-operation.md)。  <br/> |
|ErrorResponseSchemaValidation  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRestrictionTooLong  <br/> |このエラーは、制限に 255 ノードを超えるノードが含まれている場合に発生します。  <br/> |
|ErrorRestrictionTooComplex  <br/> |このエラーは、Web サービスで制限を評価できない場合Exchange発生します。  <br/> |
|ErrorResultSetTooBig  <br/> |このエラーは、特定の受信者の予定表エントリの数が 1000 の制限を超えていると示します。 ウィンドウを減らして、もう一度やり直してください。  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |このエラーは [、SavedItemFolderId が](saveditemfolderid.md) 見つからない場合に発生します。  <br/> |
|ErrorSchemaValidation  <br/> | このエラーは、要求をスキーマに対して検証できない場合に発生します。  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |このエラーは、検索フォルダーが作成されたが、検索条件がフォルダーに設定されたことがないことを示します。 これは、別の API またはクライアントを使用して作成された破損した検索フォルダーにアクセスした場合にのみ発生します。 このエラーを修正するには [、UpdateFolder](updatefolder-operation.md) 操作を使用して、フォルダーに含める必要がある制限を含める [SearchParameters](searchparameters.md) 要素を設定します。  <br/> |
|ErrorSendAsDenied  <br/> | このエラーは、次の両方の条件が発生した場合に発生します。 <br/> <br/>- ユーザーに CanActAsOwner アクセス許可が付与されているが、プリンシパルのメールボックスに対する委任権限は付与されていない。  <br/>- 同じユーザーが SendAndSaveCopy オプションを使用して、プリンシパルのメールボックスに電子メール メッセージを作成して送信します。<br/>  <br/>  その結果、ErrorSendAsDenied エラーが発生し、プリンシパルの下書きフォルダーに電子メール メッセージが作成されます。  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |**SendMeetingCancellations** 属性が要求に存在し、削除するアイテムが予定表アイテムである場合、このエラーは [DeleteItem](deleteitem-operation.md)操作によって返されます。  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |**SendMeetingInvitationsOrCancellations** 属性が要求に存在し、更新するアイテムが予定表アイテムである場合 [、UpdateItem](updateitem-operation.md)操作によってこのエラーが返されます。  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |**SendMeetingInvitations** 属性が要求に存在し、作成するアイテムが予定表アイテムである場合 [、CreateItem](createitem-operation.md)操作によってこのエラーが返されます。  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |このエラーは、開催者が会議出席依頼を送信した後、要求を更新できないことを示します。 会議を変更するには、会議出席依頼ではなく予定表アイテムを変更します。  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |このエラーは、タスクの開始者がタスク要求を送信した後、その要求を更新できないことを示します。  <br/> |
|ErrorServerBusy  <br/> |このエラーは、サーバーがビジー状態のときに発生します。  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |このエラーは、Exchange Web Services が受信者の適切なフォレストにユーザーの可用性要求をプロキシしようとしたが、サービスの検出エラーが原因で要求を送信する場所を特定できない場合を示します。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |このエラーは、Active Directory データベースで外部 URL プロパティが設定されていない場合に発生します。  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |このエラーは、共有フォルダーの同期が失敗しました。 <br/><br/>このエラー コードは、次の場合に返されます。<br/><br/>- 共有フォルダーのサブスクリプションが見つかりません。<br/>- 共有フォルダーが見つかりません。<br/>- 対応するディレクトリ ユーザーが見つかりません。<br/>- ユーザーが存在しなくなりました。<br/>- 予定が無効です。<br/>- 連絡先アイテムが無効です。<br/>- リモート サーバーとの通信に失敗しました。  <br/> |
|ErrorStaleObject  <br/> |このエラーは [、UpdateItem](updateitem-operation.md) 操作または [SendItem](senditem-operation.md) 操作で、変更キーが最新ではないか、または指定されていないときに発生します。 [GetItem 操作を呼び出して](getitem-operation.md)、更新された変更キーを取得してから、もう一度操作を実行します。  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |このエラー: 申請クォータに達したため、ユーザーが直ちに追加の要求を送信できないことを示します。  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |このエラーは、そのサブスクリプションを作成しなかったアカウントを使用してサブスクリプションにアクセスしようとするときに発生します。 各サブスクリプションにアクセスできるのは、サブスクリプションの作成者のみです。  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |このエラーは、所有者ではない場合、またはメールボックスへの所有者アクセス権を持ってない場合は、サブスクリプションを作成できないことを示します。  <br/> |
|ErrorSubscriptionNotFound  <br/> |このエラーは、指定した [SubscriptionId (GetEvents)](subscriptionid-getevents.md) に対応するサブスクリプションが見つからない場合に発生します。 サブスクリプションの有効期限が切れている可能性Exchange Web サービス プロセスが再起動されたか、無効なサブスクリプションが渡された可能性があります。 サブスクリプションが有効な場合は、最新の透かしを使用してサブスクリプションを再作成します。 これは、Unsubscribe[操作または](unsubscribe-operation.md)[GetEvents 操作の応答によって](getevents-operation.md)返されます。  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |このエラー コードは、購読が解除されたサブスクリプションに対して要求が行われたときに返す必要があります。  <br/> |
|ErrorSyncFolderNotFound  <br/> |指定された親フォルダーが見つからない場合 [は、SyncFolderItems](syncfolderitems-operation.md) 操作によってこのエラーが返されます。  <br/> |
|ErrorTeamMailboxNotFound  <br/> |このエラーは、チーム メールボックスが見つからなかったかどうかを示します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |このエラーは、チーム メールボックスが見つかったが、チーム メールボックスがサーバーにリンクSharePointします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |このエラーは、チーム メールボックスが見つかったが、サーバーへのリンクが無効SharePoint示します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |このエラー コードは使用されません。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |このエラー コードは使用されません。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |このエラーは、チーム メールボックスの所有者に通知を送信しようとして失敗したと示します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |このエラーは、チーム メールボックスにアクセスしようとするときに発生する可能性がある一般的なエラーを示します。 後で要求を送信してみてください。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorTimeIntervalTooBig  <br/> |このエラーは、指定されたタイム ウィンドウが許可されている制限より大きいと示します。 既定では、許可される制限は 42 です。  <br/> |
|ErrorTimeoutExpired  <br/> | このエラーは、要求の処理を完了するのに十分な時間が足りない場合に発生します。  <br/> |
|ErrorTimeZone  <br/> |このエラーは、タイム ゾーン エラーが発生した場合に発生します。  <br/> |
|ErrorToFolderNotFound  <br/> |このエラーは、移動先フォルダーが存在しないかどうかを示します。  <br/> |
|ErrorTokenSerializationDenied  <br/> |このエラーは、呼び出し元がトークンのシリアル化要求を実行しようとしても、クライアント アクセス サーバーに ms-Exch-EPI-TokenSerialization 権限がない場合に発生します。  <br/> |
|ErrorTooManyObjectsOpened  <br/> |このエラーは、開いているオブジェクトの内部制限を超えた場合に発生します。  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |このエラーは、ユーザーのダイヤル プランが使用できない状態を示します。  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |このエラーは、ユーザーが見つからなかったかどうかを示します。  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |このエラーは、要求を処理するためにダイヤル プランの有効なサーバーが見つかる可能性を示します。  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |このエラーは、グループから IM 連絡先を削除しようとして失敗した場合に発生します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorUnsupportedCulture  <br/> |このエラーは、Culture プロパティを **System.Globalization.CultureInfo** クラスで解析できない値に設定しようとするときに発生します。   <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |このエラーは、呼び出し元がオブジェクト、オブジェクト配列、エラー、または null の拡張プロパティを使用しようとすると発生します。  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |このエラーは[、PostItem、Message、または CalendarItem](postitem.md)オブジェクト以外のアイテムの MIME コンテンツ[](message-ex15websvcsotherref.md)を取得または設定しようとしている場合[に発生](calendaritem.md)します。  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |このエラーは、呼び出し元がクエリに対して無効なプロパティを渡した場合に発生します。 これは、計算されたプロパティが使用されている場合に発生する可能性があります。  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |このエラーは、呼び出し元が並べ替えまたはグループ化プロパティに対して無効なプロパティを渡した場合に発生します。 これは、計算されたプロパティが使用されている場合に発生する可能性があります。  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |このエラーは、検索フォルダーの制限が有効な可能性がありますが、EWS ではサポートされていません。  <br/> |
|ErrorUnsupportedRecurrence  <br/> |このエラーは、指定された繰り返しがタスクでサポートされていない状態を示します。  <br/> |
|ErrorUnsupportedSubFilter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |このエラーは、Web Services Exchangeがストア内でプロパティの種類を検出したが、プロパティの種類に対して XML を生成できないことを示します。  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |このエラーは、代理人の更新後に代理人リストの保存に失敗しました。  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |このエラーは、変更の説明に記載されている単一のプロパティ パスが、実際の Item オブジェクトまたは [Folder](item.md) オブジェクト内で設定されている 1 つのプロパティと一致しない場合に [発生](folder.md) します。  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |このエラーは、要求者が有効になっていないかどうかを示します。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |このエラーは、要求者が予定表または連絡先フォルダー内のアクセス許可を外部ユーザーに付与しようとしましたが、要求者に割り当てられた共有ポリシーは、外部ユーザーのドメインがポリシーに一覧表示されていない状態を示しています。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |要求者の組織に一連のフェデレーション ドメインが存在するが、要求者の組織に、フェデレーション ドメインの 1 つを持つ SMTP プロキシ アドレスが存在しないかどうかを示します。  <br/> |
|ErrorValueOutOfRange  <br/> |このエラーは、予定表ビューの開始日または終了日が 1/1/0001 12:00:00 AM または 12/31/9999 11:59:59 PM に設定されたかどうかを示します。  <br/> |
|ErrorVirusDetected  <br/> |このエラーは、メッセージ内Exchangeウイルスが検出されたかどうかを示します。  <br/> |
|ErrorVirusMessageDeleted  <br/> |このエラーは、メッセージ内Exchangeウイルスが検出され、削除されたかどうかを示します。  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWebRequestInInvalidState  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWin32InteropError  <br/> |このエラーは、アンマネージ コードとの通信中に内部エラーが発生しました。  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWrongServerVersion  <br/> |このエラーは、メールボックス サーバーと同じバージョンのサーバーにのみ要求を行えることを示します。  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |このエラーは、プリンシパルのメールボックス サーバーとは異なるサーバー バージョンを持つ代理人が要求を行ったかどうかを示します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラー コードは返されません。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |重複する SOAP ヘッダーが含まれます。  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | 共有フォルダーの同期が失敗したと指定します。<br/><br/> このエラー コードは、次の場合に返す必要があります。<br/><br/>- 共有フォルダーのサブスクリプションが見つかりません。  <br/>- 共有フォルダーが見つかりませんでした。  <br/>- 対応するディレクトリ ユーザーが見つかりませんでした。  <br/>- ユーザーが存在しなくなりました。  <br/>- 予定が無効です。  <br/>- 連絡先アイテムが無効です。  <br/>- リモート サーバーとの通信エラーが発生しました。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Active Directory データベースで外部 URL プロパティが設定されていないと指定します。 Active Directory データベースで外部 URL プロパティが設定されていない場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |配布リストの空き時間情報を取得するために、最大グループ メンバー数に達したと指定します。 配布リストの空き時間情報を取得するために最大グループ メンバー数に達した場合は、このエラーを返す必要があります。  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |DataType 要素と ShareFolderId 要素の両方が要求に存在することを指定します。 DataType 要素と ShareFolderId 要素の両方が要求に存在する場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |呼び出し元が予定表フォルダーまたは連絡先フォルダー内のアクセス許可を別の組織のユーザーに付与しようとして失敗した場合に指定します。 このエラー コードは、発信者の共有ポリシーが無効になっている場合、または呼び出し元に割り当てられた共有ポリシーが要求されたレベルまたは要求されたフォルダーの種類に対する共有を禁止する場合に返す必要があります。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |要求者が予定表または連絡先フォルダー内のアクセス許可を外部ユーザーに付与しようとしたが、要求者に割り当てられた共有ポリシーは、外部ユーザーのドメインがポリシーに一覧表示されないと指定します。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |要求者が予定表または連絡先フォルダー内のアクセス許可を外部ユーザーに付与しようとしたが、要求者に割り当てられた共有ポリシーは、要求されたアクセス許可レベルが共有ポリシーで許可されるレベルよりも高いことを指定します。  <br/> |
|ErrorOrganizationNotFederated  <br/> |要求者の組織がフェデレーションされていないので、要求者は外部ユーザーに送信する共有メッセージを作成できないか、外部ユーザーから受信した共有メッセージを受け入れれないので指定します。 要求元の組織がフェデレーションされていない場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorMailboxFailover  <br/> |メールボックスがフェールオーバー プロセス中のため、メールボックスにアクセスしようとして失敗したと指定します。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |共有招待の送信者が共有招待メタデータを作成しなかったことを指定します。 共有招待の送信者が共有招待メタデータを作成しなかった場合は、このエラー コードを返す必要があります。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |メッセージ追跡サービスがメッセージを追跡できないことを指定します。  <br/> |
|ErrorMessageTrackingTransientError  <br/> |メッセージ追跡サービスがダウンまたはビジー状態を指定します。 このエラー コードは、一時的なエラーを指定します。 このエラーを受信すると、クライアントはサーバーへの接続を再試行できます。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |指定したドメインが見つからないと指定します。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |要求者の組織に一連のフェデレーション ドメインが含まれますが、要求者の組織には、フェデレーション ドメインの 1 つを持つ SMTP プロキシ アドレスが含まれます。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |呼び出し元が別の組織のユーザーに空き時間情報を要求したが、組織の関係で空き時間情報が有効になっていないと指定します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |要求者の組織のフェデレーション オブジェクトが正しく構成されていないと指定します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |共有メッセージが呼び出し元を対象としていないと指定します。  <br/> |
|ErrorInvalidSharingData  <br/> |共有メタデータが無効な場合を指定します。 これは、XML が無効な場合に発生する可能性があります。  <br/> |
|ErrorInvalidSharingMessage  <br/> |共有メッセージが無効な場合を指定します。 これは、プロパティが見つからない場合に発生する可能性があります。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |共有メッセージがサポートされていないと指定します。  <br/> |
|ErrorApplyConversationActionFailed  <br/> |会話内の 1 つ以上のアイテムにアクションを適用できない場合は、このエラーを返す必要があります。  <br/> |
|ErrorInboxRulesValidationError  <br/> |ルールが検証されない場合は、このエラーを返す必要があります。  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |別のクライアントが受信トレイ ルールにアクセスした後に受信トレイ ルールを管理しようとすると、このエラーが返される必要があります。  <br/> |
|ErrorRulesOverQuota  <br/> |このエラーは、ユーザーのルール クォータを超えた場合に返す必要があります。  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |このエラーは、2 つ目のサブスクリプション接続が開いている場合は、最初のサブスクリプション接続に返す必要があります。  <br/> |
|ErrorMissedNotificationEvents  <br/> |イベント通知が見つからない場合は、このエラーを返す必要があります。  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |このエラーは、Active Directory ドメイン サービス (DS) にレガシ識別名が重複ADされます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |このエラーは、クライアント アクセス トークンを取得する要求が無効でした。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorNoSpeechDetected  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorUMServerUnavailable  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorRecipientNotFound  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorRecognizerNotInstalled  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorSpeechGrammarError  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |SOAP ヘッダーの [ManagementRole](managementrole.md) ヘッダーが正しくない場合、このエラーが返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorLocationServicesDisabled  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |このエラーは、内部での使用のみを目的とします。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorWeatherServiceDisabled  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |このエラーは、コンテンツ インデックス検索に [QueryString (String)](querystring-string.md) 要素を使用せずにスコープ検索を実行すると返されます。 これは **、SearchMailboxes** および **FindConversation 操作に適用** されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |このエラーは、アーカイブ メールボックスの検索が失敗した場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |このエラーは、アーカイブ メールボックスの URL が検出できない場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |このエラーは、リモート アーカイブ メールボックス フォルダーを取得する操作が失敗した場合に発生します。  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |このエラーは、リモート アーカイブ メールボックス フォルダーを検索する操作が失敗した場合に発生します。  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |このエラーは、リモート アーカイブ メールボックス アイテムを取得する操作が失敗した場合に発生します。  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |このエラーは、リモート アーカイブ メールボックス アイテムをエクスポートする操作が失敗した場合に発生します。  <br/> |
|ErrorInvalidPhotoSize  <br/> |このエラーは、無効な写真サイズがサーバーから要求された場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |このエラーは **、GetUserPhoto** 操作要求で予期しない写真サイズが要求された場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |このエラーは **、SearchMailboxes** 操作要求に検索するメールボックスが多すぎる場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |このエラーは、このユーザーの保持タグが見つからなかったかどうかを示します。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |このエラーは、テナントまたはサーバーで探索検索が無効になっている場合に返されます。 このエラーは、2013 年Exchangeされました。  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |このエラーは、サポートされていない予定表アイテムをフェッチするために[SeekToConditionPageItemView](seektoconditionpageitemview.md)を使用して[FindItem](finditem-operation.md)操作を呼び出す際に発生します。  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |このエラーは、内部での使用のみを目的とします。  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |テナントは削除のマークが付いている。  <br/> |
|ErrorInvalidLicense  <br/> |ユーザーが有効なライセンスを持ってない。  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |フォルダーごとのメッセージ受信クォータを超えました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は必須ではなく、すべての応答に含まれるとは言えありません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

