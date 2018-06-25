---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: ResponseCode 要素は、要求の状態に関する情報を提供します。
ms.openlocfilehash: 7baeb0ab87ffb43ba9d6b4016477888aa4ed613e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833294"
---
# <a name="responsecode"></a>ResponseCode

**ResponseCode**要素は、要求の状態に関する情報を提供します。 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|要素|説明|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 応答ステータスに関する説明情報を提供します。<br/><br/>  この要素に使用可能な XPath 式は、次のように。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[DeleteItem の操作](deleteitem-operation.md)を要求します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[SendItem 操作](senditem-operation.md)を要求します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[DeleteFolder の操作](deletefolder-operation.md)を要求します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[DeleteAttachment 操作](deleteattachment-operation.md)を要求します。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |状態および 1 つの結果が含まれています[購読の取り消し操作](unsubscribe-operation.md)を要求します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateFolder 操作](createfolder-operation.md)を要求します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetFolder の操作](getfolder-operation.md)を要求します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[UpdateFolder 操作](updatefolder-operation.md)を要求します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[MoveFolder 操作](movefolder-operation.md)を要求します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CopyFolder 操作](copyfolder-operation.md)を要求します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateManagedFolder 操作](createmanagedfolder-operation.md)を要求します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[FindFolder 操作](findfolder-operation.md)を要求します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateItem 操作](createitem-operation.md)を要求します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetItem 操作](getitem-operation.md)を要求します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[UpdateItem 操作](updateitem-operation.md)を要求します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[MoveItem 操作](moveitem-operation.md)を要求します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CopyItem 操作](copyitem-operation.md)を要求します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateAttachment 操作](createattachment-operation.md)を要求します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetAttachment 操作](getattachment-operation.md)を要求します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[FindItem 操作](finditem-operation.md)を要求します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |[ResolveNames 操作](resolvenames-operation.md)要求の結果ステータスを格納します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[ExpandDL の操作](expanddl-operation.md)を要求します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |状態および 1 つの結果が含まれています[購読の操作](subscribe-operation.md)を要求します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetEvents 操作](getevents-operation.md)を要求します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |状態および 1 つの SendNotification 操作要求の結果が含まれています。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)要求の結果ステータスを格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[SyncFolderItems 操作](syncfolderitems-operation.md)要求の結果ステータスを格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |状態と[ConvertId の操作](convertid-operation.md)要求の結果が含まれています。  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |[AddDelegate 操作](adddelegate-operation.md)要求の結果ステータスを格納します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |状態と[GetDelegate の操作](getdelegate-operation.md)要求の結果が含まれています。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |状態と[RemoveDelegate の操作](removedelegate-operation.md)要求の結果が含まれています。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |状態と[UpdateDelegate の操作](updatedelegate-operation.md)要求の結果が含まれています。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |状態と[GetServerTimeZones の操作](getservertimezones-operation.md)要求の結果が含まれています。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |状態と[GetSharingFolder の操作](getsharingfolder-operation.md)要求の結果が含まれています。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |[GetSharingFolder 操作](getsharingfolder-operation.md)要求に対する応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |状態と[GetSharingMetadata の操作](getsharingmetadata-operation.md)要求の結果が含まれています。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |[GetSharingMetadata 操作](getsharingmetadata-operation.md)要求に対する応答を定義します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |状態と[RefreshSharingFolder の操作](refreshsharingfolder-operation.md)要求の結果が含まれています。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |[RefreshSharingFolder 操作](refreshsharingfolder-operation.md)要求に対する応答を定義します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |状態および[FindConversation 操作](findconversation-operation.md)の応答の結果が含まれています。  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |状態と[ApplyConversationAction の操作](applyconversationaction-operation.md)要求の結果が含まれています。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[EmptyFolder 操作](emptyfolder-operation.md)を要求します。  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |状態と[UpdateInboxRules の操作](updateinboxrules-operation.md)要求の結果が含まれています。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |状態と[UploadItems の操作](uploaditems-operation.md)要求の結果が含まれています。  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |[GetInboxRules 操作](getinboxrules-operation.md)への応答が含まれています。 要求します。  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)の要求への応答が含まれています。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素が使用される場合に必要です。 次の表では、この要素に返される値について説明します。
  
|値|説明|
|:-----|:-----|
|NoError  <br/> |要求に対してエラーが発生しなかった。  <br/> |
|ErrorAccessDenied  <br/> |このエラーは、要求されたアクションを実行する権限が呼び出し元のアカウントにない場合に発生します。  <br/> |
|ErrorAccessModeSpecified  <br/> |このエラーは、内部でのみ使用します。 このエラーは返されません。  <br/> |
|ErrorAccountDisabled  <br/> |このエラーは、問題のアカウントが無効になっている場合に発生します。  <br/> |
|ErrorAddDelegatesFailed  <br/> |このエラーは、追加のデリゲートのリストを保存できない場合に発生します。  <br/> |
|ErrorAddressSpaceNotFound  <br/> |アドレス スペースのレコード、またはフォレスト間の可用性を実現する、ドメイン ネーム システム (DNS) ドメイン名で見つかりませんでした、Active Directory データベースでこのエラーが発生します。  <br/> |
|ErrorADOperation  <br/> |このエラーは、Active Directory ドメイン サービス (AD DS) との通信問題が発生したため、操作が失敗したときに発生します。  <br/> |
|ErrorADSessionFilter  <br/> |**ResolveNames**操作要求の名前を指定するときにこのエラーが返されることは有効ではありません。  <br/> |
|ErrorADUnavailable  <br/> |このエラーは、AD DS が使用できない場合に発生します。 後でもう一度やり直してください。  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |このエラーは、 **AffectedTaskOccurrences**属性の有効期限がされていないことを示します。 [DeleteItem](deleteitem.md)要素を使用して、タスクは、少なくとも 1 つの項目を削除してかどうかは、そのタスクが定期的に、 **AffectedTaskOccurrences**属性が**DeleteItem**を決定できるように指定するかどうか現在の回またはシリーズを全体削除します。  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |アーカイブ フォルダーのパスの作成時にエラーを示します。  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |アーカイブ先のメールボックスが無効になっていることを示します。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |そのアーカイブ メールボックスのサービスの検索が失敗したことを示します。  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |10 個以上の入れ子になった添付ファイル付きのアイテムを作成しようとするかを指定します。 この値は、Exchange Server 2010 のサービス パック 2 (SP2) で導入されました。  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |[CreateAttachment](createattachment.md)要素は、バイト単位で Int32.MaxValue を超えるサイズの添付ファイルを作成しようとしましたが場合にこのエラーを返します。  <br/> [GetAttachment](getattachment.md)要素は、サイズがバイト単位で Int32.MaxValue を超える既存の添付ファイルを取得するとした場合にこのエラーを返します。  <br/> |
|ErrorAutoDiscoverFailed  <br/> |このエラーは、Exchange Web サービスが Exchange 2010 を実行してフォレスト間のコンピューターの場所には、自動検出サービスが自動検出サービスへの呼び出しを使用して、インストールされているクライアント アクセス サーバーの役割を決定しようとしたことを示します失敗しました。  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |このエラーは、ローカル フォレストの構成情報が AD DS に表示されないことを示します。  <br/> |
|ErrorBatchProcessingStopped  <br/> | このエラーは、アイテムの処理中に例外が発生したことと、例外が次の項目に発生する可能性を示します。 要求は、複数の項目を含める可能性があります。たとえば、GetItem 操作の要求には、複数の識別子が含まれます。 一般に、項目は、処理済みの 1 つずつです。 アイテムの処理中に例外が発生して、例外が次の項目に発生する可能性がある場合、後に続く項目は処理されません。  <br/><br/>  以下は、次の項目の処理を停止するエラーの例です。<br/>  <br/>-ErrorAccessDenied  <br/>-ErrorAccountDisabled  <br/>-ErrorADUnavailable  <br/>-ErrorADOperation  <br/>-ErrorConnectionFailed  <br/>-ErrorMailboxStoreUnavailable  <br/>-ErrorMailboxMoveInProgress  <br/>-ErrorPasswordChangeRequired  <br/>-ErrorPasswordExpired  <br/>-ErrorQuotaExceeded  <br/>-ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |このエラーは、定期的な予定表アイテムの出現箇所をコピーまたは移動する試みが行われたときに発生します。  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | 削除済みアイテム フォルダーに存在し、会議の更新やキャンセルは、 **SendMeetingInvitationsOrCancellations**属性の値に従って送信する予定表アイテムを更新しようと、このエラーが発生します。 <br/><br/>次に、この属性で使用できる値を示します。  <br/><br/>-SendToAllAndSaveCopy  <br/>-SendToChangedAndSaveCopy  <br/>-SendOnlyToAll  <br/>-SendOnlyToChanged  <br/>  <br/>ただし、この属性の値が SendToNone に設定されている場合にのみこのような更新が許可されます。  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |UpdateItem、GetItem、DeleteItem、MoveItem、CopyItem、または SendItem 操作が呼び出され、指定された ID は定期的な予定表アイテムのアイテム ID ではありません、このエラーが発生します。  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |**UpdateItem**、 **GetItem**、 **DeleteItem**、 **MoveItem**、 **CopyItem**、または**SendItem**操作が呼び出され、指定された ID は定期的なマスター アイテムの ID ではありません、このエラーが発生します。  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |このエラーが発生**CreateItem**または**UpdateItem**操作中に予定表アイテムの期間が許可されている最大長より長い場合は現在の 5 年間です。  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |カレンダーの終了時刻は開始時刻の前後に同時に設定されている場合、このエラーが発生します。  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |このエラーは、予定表フォルダーの種類の[予定表ビュー](calendarview.md)の要素を持つ**FindItem**操作の指定したフォルダーがない場合に発生します。  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |このエラーは、時間の変更のパターンを定義するのには 1 日、WeekendDay、および曜日の無効な値を使用すると、 **CreateItem**または**UpdateItem**操作中に発生します。  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |このエラーは、日、曜日、および WeekendDay の無効な値を使用して、毎週の頻度を指定する場合に、 **CreateItem**または**UpdateItem**操作中に発生します。  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |このエラーは、予定表アイテムの繰り返しバイナリ ラージ オブジェクト (BLOB) Exchange ストア内の状態が無効である場合に発生します。  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |このエラーは、指定された定期的なアイテムを作成できない場合に発生します。  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |このエラーは、無効なタイム ゾーンが発生したときに発生します。  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |このエラーは、予定表アイテムがキャンセルされたことを示します。  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |このエラーは、予定表アイテムがキャンセルされたことを示します。  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |このエラーは、予定表アイテムがキャンセルされたことを示します。  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |このエラーは、予定表アイテムがキャンセルされたことを示します。  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |このエラーは、 [AcceptItem](acceptitem.md)要素が委任のシナリオでは、予定表アイテムまたは会議出席依頼に対して有効であることを示します。  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |このエラーは、 [DeclineItem](declineitem.md)要素が委任のシナリオでは、予定表アイテムまたは会議出席依頼に対して有効であることを示します。  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |このエラー[での RemoveItem](removeitem.md)要素が委任のシナリオでは、会議の取り消し通知に対して有効であることを示します。  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |このエラーは、 [TentativelyAcceptItem](tentativelyacceptitem.md)要素が委任のシナリオでは、予定表アイテムまたは会議出席依頼に対して有効であることを示します。  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |このエラーは、予定表アイテムの操作 (現在は CancelItem) が出席者に対して有効ではないことを示します。 会議の開催者だけでは、会議をキャンセルできます。  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |このエラーは、 [AcceptItem](acceptitem.md)が開催者の予定表アイテムに対して有効であることを示します。  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |このエラーは、 [DeclineItem](declineitem.md)が開催者の予定表アイテムに対して有効であることを示します。  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |このエラー[での RemoveItem](removeitem.md)が開催者の予定表アイテムに対して有効であることを示します。 予定表から会議を削除するのには、開催者は CancelCalendarItem を使用しなければなりません。  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |このエラーは、 [TentativelyAcceptItem](tentativelyacceptitem.md)が開催者の予定表アイテムに対して有効であることを示します。  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |このエラーは、会議出席依頼が古くなって更新できないことを示します。  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |このエラーは、インデックスは、現在のパターン内の出来事を指していないことを示します。 たとえば、3 つの会議の予定の定期的なパターンを定義し、5 番目のアイテムにアクセスしようとする、この応答コードが発生します。  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |このエラーは、(定期的なマスター ID とアイテムのインデックスを使用して解決)、削除されたアイテムのすべての操作が有効ではないことを示します。  <br/> |
|ErrorCalendarOutOfRange  <br/> |プロパティの値が範囲外ですと、createitem メソッドと UpdateItem の予定表アイテム、またはタスクの定期的なアイテムのプロパティの操作にこのエラーが報告されます。 たとえば、月の第 15 週を指定すると、この応答コード。  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |このエラーが発生する[予定表ビュー](calendarview.md)の要素は、現在 2 年間の許容最大値より多くの範囲の最後に起動とします。  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |このエラーは、要求元のアカウントは、ディレクトリ データベース内の有効なアカウントではないことを示します。  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |取引先担当者のタスクの予定表フォルダーをアーカイブしようとすることを示します。  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |パブリック フォルダーのアイテムを保存しようとすることを示します。  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |その試みましたアーカイブ メールボックス内のアイテムをアーカイブすることを示します。  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |このエラーは、予定表アイテムが作成されると、 **SavedItemFolderId**属性がない予定表フォルダーを参照するときに発生します。  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |このエラーは、連絡先が作成されると、 **SavedItemFolderId**属性は、連絡先以外のフォルダーを参照するときに発生します。  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |このエラーは、予定表、連絡先、タスク、メモ、およびようになど、メール フォルダー以外のフォルダーに投稿するアイテムを作成することはできませんを示します。  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |このエラーは、タスクが作成されると、 **SavedItemFolderId**属性は、タスクではないフォルダーを参照するときに発生します。  <br/> |
|ErrorCannotDeleteObject  <br/> |アイテムまたはフォルダーを削除するのには削除できない場合、このエラーが発生します。  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |[DeleteItem の操作](deleteitem-operation.md)は、定期的なタスクの現在のアイテムを削除に失敗したときにこのエラーを返します。 これは SpecifiedOccurrenceOnly に**AffectedTaskOccurrences**属性が設定されている場合のみ発生します。  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Mandatorty の拡張機能を無効にしようとすることを示します。  <br/> |
|ErrorCannotEmptyFolder  <br/> |このエラーは、サーバー フォルダーを空にできない場合に返されます必要があります。  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |ソース フォルダーのパスを取得できませんでしたを示します。  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |サーバーを取得できませんでした外部 URL の Outlook Web App オプションを指定します。  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |**GetAttachment**操作は、添付ファイルの本文を取得できない場合にこのエラーを返します。  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |このエラーは、呼び出し元が非予定表フォルダーの予定表のアクセス許可を設定しようとしたことを示します。  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |このエラーは、呼び出し元が [予定表] フォルダー以外のカレンダーのアクセス権を設定しようとしたことを示します。  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |このエラーは、アクセス許可セットで不明なアクセス許可を設定することはできないことを示します。  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |ソース フォルダーと検索フォルダーを指定しようとすることを示します。  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |アイテム識別子を必要とする要求は、フォルダーの識別子を指定すると、このエラーが発生します。  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |フォルダー識別子を必要とする要求には、アイテム識別子が与えられると、このエラーが発生します。  <br/> |
|ErrorChangeKeyRequired  <br/> |この応答コードは、 **ErrorChangeKeyRequiredForWriteOperations**で置き換えられています <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |見つからないか、古いアイテムのキーの変更は、このエラーが返されます。 <br/><br/>SendItem、UpdateItem、UpdateFolder 操作の呼び出し元は、項目の変更が正しく、現在のキーに渡す必要があります。 これは UpdateItem と競合の解決が常に上書きする設定のときにも注意してください。  <br/> |
|ErrorClientDisconnected  <br/> |クライアントが切断されたことを指定します。  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorClientIntentNotFound  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorConnectionFailed  <br/> |このエラーは、Exchange Web サービスは、メールボックスに接続できない場合に発生します。  <br/> |
|ErrorContainsFilterWrongType  <br/> |このエラーは、含まれるフィルターの検査されたプロパティが文字列型ではないことを示します。  <br/> |
|ErrorContentConversionFailed  <br/> |**GetItem**操作は、Exchange Web サービスでは、項目の MIME コンテンツを取得できないときにこのエラーが要求を返します。 <br/><br/>**CreateItem**操作は、Exchange Web サービスが提供されている MIME コンテンツの項目を作成することはときにこのエラーを返します。 通常これは、item プロパティが破損しているか、切り捨てられることを示す値です。  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |検索が要求されるクエリ文字列オプションを使用して、コンテンツのインデックス作成が移動先のメールボックスを有効になっていない場合、このエラーが発生します。  <br/> |
|ErrorCorruptData  <br/> |このエラーは、データが破損しているし、処理できないときに発生します。  <br/> |
|ErrorCreateItemAccessDenied  <br/> |このエラーは、呼び出し元は項目を作成する権限を持っていない場合に発生します。  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |このエラーが発生するか、CreateManagedFolder 操作の要求で指定された管理フォルダーの作成できませんでした。 作成されたフォルダーと、フォルダーが存在しないを決定するには、各フォルダーを検索します。  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |このエラーは、呼び出し元のアカウントにサブフォルダーを作成するために必要なアクセス許可があるない場合に発生します。  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |このエラーが発生したは、1 つのメールボックスからアイテムまたはフォルダーを移動しようとします。 移動元のメールボックスと移動先のメールボックスが異なる場合、このエラーが表示されます。  <br/> |
|ErrorCrossSiteRequest  <br/> |このエラーは、要求を処理する必要がありますクライアント アクセス サーバーは、別のサイトであるために要求が許可されないことを示します。  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |このエラーは、次のシナリオで発生します。<br/>  <br/>-しようとしましたがアクセスしたり、項目のプロパティを記述し、プロパティの値が大きすぎます。<br/>要求 XML 内での長さが制限を超えるコンテンツの MIME を base64 にエンコードされます。<br/>-既存のアイテムの本文の本文のサイズを超えています。<br/>-消費者が、html 形式またはテキスト本文の長さ (または追加の場合の合計の長さ) を超えていますを設定しようとするとします。 |
|ErrorDataSourceOperation  <br/> |このエラーは、基になるデータ プロバイダーが操作を完了する失敗したときに発生します。  <br/> |
|ErrorDelegateAlreadyExists  <br/> |このエラーは、デリゲートのリストで指定したユーザーが既に存在する場合、 **AddDelegate**操作で発生します。  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |このエラーは、メールボックスの所有者は、指定したユーザーを追加するとき、 **AddDelegate**操作で発生します。  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |このエラーは、いずれかがない場合にローカルの空き時間情報メッセージについては、代理人またはない Active Directory パブリック デリゲートなし「パブリック デリゲート」(AD DS に「代理送信」エントリがありません)、 **GetDelegate**の操作で発生します。  <br/> |
|ErrorDelegateNoUser  <br/> |このエラーは、指定されたユーザーは、AD DS のユーザーにマッピングできない場合に発生します。  <br/> |
|ErrorDelegateValidationFailed  <br/> |このエラーは、追加した代理人のユーザーが無効な場合**AddDelegate**操作で発生します。  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |識別フォルダーを削除しようとすると、このエラーが発生します。  <br/> |
|ErrorDeleteItemsFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |このエラーは、ユーザーの識別 ID が操作に対して有効ではないことを示します。 **DistinguishedUserType**は、要求内に存在しない場合があります。  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |このエラーは、要求の配布リストのメンバーは、配布リストに存在しないことを示します。  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |**CreateManagedFolder**操作要求の[表示](foldernames.md)要素内で重複しているフォルダー名を指定する場合、このエラーが発生します。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |このエラーは、SOAP ヘッダーの重複があることを示します。  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |このエラーは、重複するユーザー ID が見つかったことでアクセス許可セットでは、既定または匿名のいずれかを複数回、設定や重複した Sid または受信者があることを示します。  <br/> |
|ErrorEmailAddressMismatch  <br/> |このエラーは、要求が検索フォルダーの検索パラメーターの作成または更新しようとするときに発生します。 たとえば、メールボックスの検索フォルダーが作成されますが、別のメールボックスを検索する検索フォルダーを送信するときに、この問題が発生することができます。  <br/> |
|ErrorEventNotFound  <br/> |透かしに関連付けられているイベントが削除されると、イベントが返される前に、このエラーが発生します。 このエラーが返された場合は、サブスクリプションも削除されます。  <br/> |
|ErrorExceededConnectionCount  <br/> |同時にこのエラー ・ iIndicates は、ユーザーのポリシーで許可されているよりも、サーバーに対して要求します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |このエラーは、ユーザーがサブスクリプションの最大数を超過しましたが、ポリシーを調整のことを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |このエラーは、検索操作の呼び出しが返されるアイテムの合計数を超えたことを示します。  <br/> |
|ErrorExpiredSubscription  <br/> |期限切れになったために、サブスクリプションを削除しています、 [GetEvents 操作](getevents-operation.md)が呼び出された場合、このエラーが発生します。  <br/> |
|ErrorExtensionNotFound  <br/> |拡張モジュールが見つからなかったことを示します。  <br/> |
|ErrorFolderCorrupt  <br/> |フォルダーが破損しているし、保存できない場合、このエラーが発生します。  <br/> |
|ErrorFolderExists  <br/> |このエラーが発生したは、同じ親に別のフォルダーと同じ名前を持つフォルダーを作成しようとします。 重複するフォルダー名を指定することはできません。  <br/> |
|ErrorFolderNotFound  <br/> |このエラーは、指定されたフォルダー ID が有効なフォルダーに対応していませんか、代理人に、フォルダーにアクセスする権限がないことを示します。  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |このエラーは、要求されたプロパティを取得できませんでしたを示します。 これには、プロパティが存在しないこと、ですが、取得に失敗したことに、プロパティがなんらかの方法で壊れていることは示されません。  <br/> |
|ErrorFolderSave  <br/> |このエラーは、フォルダーを作成またはできなかった無効な状態が原因で更新を示します。  <br/> |
|ErrorFolderSaveFailed  <br/> |このエラーは、フォルダーを作成またはできなかった無効な状態が原因で更新を示します。  <br/> |
|ErrorFolderSavePropertyError  <br/> |このエラーは、フォルダーを作成またはできなかった無効なプロパティ値があるため更新を示します。 応答コードは、問題の原因であるプロパティを一覧表示します。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |このエラーは、配布リスト用の空き時間情報を取得するため、最大のグループのメンバーの数に達して ことを示します。  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |間にある障害のための空き時間情報を取得することはできませんとこのエラーが返されます。  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorImContactLimitReached  <br/> |連絡先の最大数に達したために、新しいインスタント メッセージング (IM) の連絡先を追加することはできませんとこのエラーが返されます。 このエラーは、Exchange Server 2013 で導入されました。  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |既存のグループには既に同じ表示名とグループの表示名を追加しようと、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorImGroupLimitReached  <br/> |グループの最大数に達したために、IM の新しいグループを追加することはできませんとこのエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorImpersonateUserDenied  <br/> |エラーが返されるサーバーからサーバーへの認証の場合は Exchange 偽装呼び出し元に特定のユーザーを偽装するように適切な権限がないと、問題の。 このエラーは、偽装するように、ms-Exch-EPI-月-拡張された権利を Active Directory にマップします。  <br/> |
|ErrorImpersonationDenied  <br/> |呼び出し元に対して要求を行うには、クライアント アクセス サーバーを偽装するように適切な権限を持たない場合、Exchange の偽装をサーバーからサーバーへの認証にこのエラーが返されます。 これは、ms-Exch ・ EPI ・偽装拡張された権利を Active Directory にマップされます。  <br/> |
|ErrorImpersonationFailed  <br/> |このエラーは、サーバーからサーバーへの認証を実行しようとしたときに予期しないエラーが認識したことを示します。 この応答コード通常を示しているか、Exchange Web サービスがディレクトリと通信できません、または、フォレスト間に信頼関係が正しくされていない、アプリケーション プールが正しく構成されていない Exchange Web サービスを実行しているサービス アカウント構成されています。  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |このエラーは、要求が Exchange Server の現在のバージョンに有効でしたが、指定された要求のサーバーのバージョンに対して無効ですを示します。  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |[UpdateItem](updateitem.md)または[UpdateFolder](updatefolder.md)要素の各変更の説明が更新するプロパティを 1 つだけをリストする必要がありますこのエラーを示します。  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |このエラーは、解決するのには多くの参加者が要求に含まれている場合に発生します。 既定では、解決できる出席者の最大数は、100 です。  <br/> |
|ErrorInsufficientResources  <br/> |このエラーは、メールボックス サーバーが過負荷になっている場合に発生します。 後でもう一度やり直してください。  <br/> |
|ErrorInternalServerError  <br/> |このエラーは、Exchange Web サービスに、復旧できませんでしたし、発生したエラーに関連付けられている具体的な応答コードが存在しないエラーが発生したことを示します。  <br/> |
|ErrorInternalServerTransientError  <br/> |このエラーは、内部サーバー エラーが発生したことと、要求を後で再試行する必要があることを示します。  <br/> |
|ErrorInvalidAccessLevel  <br/> |このエラーは、呼び出し元が空き時間情報データに対して持っているアクセス権のレベルが有効ではないことを示します。  <br/> |
|ErrorInvalidArgument  <br/> |このエラーは、 [GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)に渡されるすべての無効な引数によって発生したエラーを示します。<br/><br/> 次のシナリオでは、このエラーが返されます。 <br/><br/>-で指定したユーザー、_を送信する-として_パラメーターは、ディレクトリに存在しません。 <br/>-で指定したユーザー、_を送信する-として_パラメーターは、ディレクトリ内で一意ではありません。 <br/>-_を送信する-として_アドレスが空です。<br/>-_を送信する-として_アドレスが有効な電子メール アドレスではありません。  <br/> |
|ErrorInvalidAttachmentId  <br/> |[GetAttachment 操作](getattachment-operation.md)によってこのエラーが返されるか、 [DeleteAttachment 操作](deleteattachment-operation.md)に指定した ID に対応する添付ファイルが見つかりません。  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |このエラーは、複雑な添付ファイル テーブルの制限を使用して既存の検索フォルダーにバインドしようとするときに発生します。 Exchange Web サービスのみをサポートしています簡単には、添付ファイル テーブルに対してフィルターが含まれています。 既存の検索フォルダーにバインドしようとする場合より複雑な添付ファイル テーブルの制限 (サブフィルター) が、Exchange Web サービスは、そのフィルターの XML を表示することはできませんし、この応答コードを返します。 <br/><br/>フォルダーで GetFolder の操作を呼び出すことができますが、 [SearchParameters](searchparameters.md)要素を要求しないことに注意してください。  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |このエラーは、複雑な添付ファイル テーブルの制限を使用して既存の検索フォルダーにバインドしようとするときに発生します。 Exchange Web サービスのみをサポートしています簡単には、添付ファイル テーブルに対してフィルターが含まれています。 <br/><br/>さらに複雑な添付ファイル テーブルの制限を持つ既存の検索フォルダーにバインドしようとすると、Exchange Web サービスは、そのフィルターの XML を表示できません。 この例では、添付ファイルのサブフィルターにテキスト フィルターが含まれていますが、添付ファイルの表示名を参照していません。<br/><br/> フォルダーで GetFolder の操作を呼び出すことができますが、 [SearchParameters](searchparameters.md)要素を要求しないことに注意してください。  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | このエラーは、要求元の承認手順が失敗したことを示します。  <br/> |
|ErrorInvalidChangeKey  <br/> |このエラーは、フォルダーまたはアイテムの識別子で解析できない変更キーを使用してコンシューマーを通過するときに発生します。 たとえば、無効な base64 のコンテンツまたは空の文字列では、この可能性があります。  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |このエラーは、呼び出し元の id を解決するにはしようとしたときに内部エラーが認識したことを示します。  <br/> |
|ErrorInvalidCompleteDate  <br/> |将来の時刻にタスクの[CompleteDate](completedate.md)要素の値を設定しようと、このエラーが返されます。 クライアント アクセス サーバーのローカル時刻に変換すると、タスクの[CompleteDate](completedate.md)をクライアント アクセス サーバー上のローカル時刻より後の値に設定できません。  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |このエラーは、無効な電子メール アドレスが連絡先を提供されていることを示します。  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |このエラーは、電子メールのエントリの無効な電子メールのインデックス値が提供されていることを示します。  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |プロキシに使用される資格情報と、このエラーが発生する別のディレクトリ サービスのフォレストへの要求が認証に失敗します。  <br/> |
|ErrorInvalidDelegatePermission  <br/> |このエラーは、指定したフォルダーのアクセス許可が有効ではないことを示します。  <br/> |
|ErrorInvalidDelegateUserId  <br/> |このエラーは、指定したデリゲートのユーザー ID が有効ではないことを示します。  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |このエラーは、呼び出し元は、UPN、電子メール アドレス、またはユーザーの SID を指定していない場合、Exchange の偽装中に発生します。 これは、呼び出し元が 1 つ以上のものを指定し、値が空の場合にも発生します。  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |このエラーは、[除外](excludes.md)要素の制限に渡されたビットマスクが解析できない場合に発生します。  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidExtendedProperty  <br/> | 次のイベントが発生すると、このエラーが発生します。 <br/> <br/>-呼び出し元は、Exchange Web サービスでサポートされていない拡張プロパティを使用しようとします。  <br/>、拡張プロパティの属性値の無効な組み合わせで呼び出し元に渡します。 これは、属性が渡されない場合にも発生します。 特定の組み合わせのみが許可されています。  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |このエラーは、拡張プロパティの [値] セクションでは、プロパティの型が一致しない場合に発生します。 <br/><br/>登録するときは、拡張プロパティを設定するたとえば、="String"への整数の配列は、このエラーが発生します。 拡張プロパティに指定された型に強制変換ではない任意の文字列形式には、このエラーが得られます。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |このエラーは、共有への招待の送信者が共有の招待状のメタデータを作成していないことを示します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |このエラーは、共有メッセージが呼び出し元の目的としていないことを示します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |このエラーは、要求側の組織のフェデレーション オブジェクトを正しく構成されていないことを示します。  <br/> |
|ErrorInvalidFolderId  <br/> |このエラーは、フォルダー ID が破損している場合に発生します。  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |このエラーは、指定したフォルダーの種類が現在の操作に対して有効ではないことを示します。 たとえば、パブリック フォルダーで検索フォルダーを作成できません。  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | このエラーは、ユーザーが次のいずれかを指定するときに、分数形式のページングで行われます。 <br/> <br/>-分子が分母より大きい  <br/>が 0 より小さい値である、分子  <br/>-分母が 0 未満です。  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |このエラーは、[データ型](datatype.md)および ShareFolderId の要素は、両方の要求内に存在を示します。  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |このエラーは、[なし] は、 [FreeBusyViewType](freebusyviewtype.md)と[GetUserAvailability の操作](getuseravailability-operation.md)が呼び出されたときに発生します。  <br/> |
|ErrorInvalidId  <br/> |このエラーは、ID や変更キーが不正なことを示します。  <br/> |
|ErrorInvalidIdEmpty  <br/> |このエラーは、呼び出し元が空では**Id**属性を指定するときに発生します。  <br/> |
|ErrorInvalidLikeRequest  <br/> |このエラーは、項目をリンクできない場合に発生します。 Exchange のビルド番号 15.00.0913.09 以降のバージョンには、この値が含まれます。  <br/> |
|ErrorInvalidIdMalformed  <br/> |このエラーは、呼び出し元が異常な**Id**属性を指定するときに発生します。  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |このエラーは、Exchange 2007 SP1 のバージョンを含む要求に対して指定された以降に、Exchange 2007 形式を使用しているフォルダーまたはアイテムの ID をしたことを示します。 Exchange 2007 SP1 またはそれ以降の要求での Exchange 2007 の Id を使用することはできません。 最初に変換するのには、 [ConvertId 操作](convertid-operation.md)を使用する必要があります。  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |このエラーは、呼び出し元**Id**属性が長すぎることを指定するときに発生します。  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |ID は ID が添付ファイル ID を受け取る Web サービス メソッドに渡されたアイテムの添付ファイルではないときにこのエラーが返されます  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |このエラーは、メールボックス内の連絡先が破損している場合に発生します。  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |このエラーは、呼び出し元**Id**属性が長すぎることを指定するときに発生します。  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |アイテムに添付ファイルの階層は、255 レベルの深さの最大値を超えたときは、このエラーが返されます。  <br/> |
|ErrorInvalidIdXml  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidImContactId  <br/> |指定した IM 連絡先の id が有効な識別子を表さない場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |指定した IM 配布グループ SMTP アドレス識別子が有効な識別子を表さない場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidImGroupId  <br/> |指定した IM グループ識別子が有効な識別子を表さない場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |インデックス付きページングのオフセットが負の場合、このエラーが発生します。  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |アイテムが**ArchiveItem**操作に対して有効なことを示します。  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |AcceptItem 応答オブジェクトを使用して、会議出席依頼または予定表アイテム以外の項目の種類をしようとしたとき、または削除済みアイテム フォルダー内にある予定表のアイテム アイテムをそのまま使用しようとしましたが、このエラーが発生します。  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |CancelItem response オブジェクトを使用して、予定表アイテム以外の項目の種類にしようとしたとき、このエラーが発生します。  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | サポートされていない種類のアイテムの添付ファイルを作成しようと、このエラーが返されます。  <br/><br/>  項目の添付ファイルのサポートされている項目の種類には、次のオブジェクトが含まれます。  <br/><br/>- [アイテム](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [カレンダー項目](calendaritem.md) <br/>- [タスク](task.md) <br/>- [連絡先](contact.md) <br/> <br/> たとえば、 [MeetingMessage](meetingmessage.md)の添付ファイルを作成しようとすると、この応答コードが発生します。  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | 要求にサポートされていない項目の種類が含まれている場合は、 [CreateItem 操作](createitem-operation.md)からこのエラーが返されます。 <br/><br/>サポートされている項目には、次のオブジェクトが含まれます。<br/>  <br/>- [アイテム](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [カレンダー項目](calendaritem.md) <br/>- [タスク](task.md) <br/>- [連絡先](contact.md) <br/><br/>  特定の種類は、何の副作用として作成されます。 出席者の予定表アイテムを送信するときに作成などのメッセージを達成するには、明示的に作成されません。  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |以外の会議出席依頼または予定表アイテムでは、項目の種類の DeclineItem の応答オブジェクトを使用しようとしましたがとき、または削除済みアイテム フォルダー内にある予定表のアイテム アイテムを辞退しようとしましたが、このエラーが発生します。  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |このエラーは、 [ExpandDL 操作](expanddl-operation.md)が個人用配布リストに対してのみ有効であることを示します。  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |要求は、会議ではない項目を指定した場合での RemoveItem 応答オブジェクトからこのエラーが返されますキャンセル アイテムです。  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |要求メッセージの項目ではない項目を指定する場合、このエラーが[SendItem 操作](senditem-operation.md)から返されます。  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |[TentativelyAcceptItem](tentativelyacceptitem.md)以外の会議出席依頼または予定表アイテムでは、項目の種類を使用しようとしましたがとき、または削除済みアイテム フォルダー内にある予定表アイテムの出現を仮承諾しようとしましたが、このエラーが発生します。  <br/> |
|ErrorInvalidLogonType  <br/> |このエラーは、内部でのみ使用します。 このエラーは返されません。  <br/> |
|ErrorInvalidMailbox  <br/> |このエラーは、 [CreateItem 操作](createitem-operation.md)または[UpdateItem 操作](updateitem-operation.md)を作成または個人用配布リストを更新中に失敗したことを示します。  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |このエラーは、管理フォルダーの構造が破損していて表示できない場合に発生します。  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |このエラーは、管理対象フォルダーに設定されているクォータが小さい場合に発生以上破損している管理対象のフォルダーを示します。  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |管理フォルダーに設定されているサイズが小さいときにこのエラーが発生した以上破損している管理対象のフォルダーを示します。  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |このエラーは、指定された結合された空き/予約済み内部値が無効である場合に発生します。 既定の最小値は、5 分です。 既定の最大値は、1440 分です。  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |このエラーは、名前が[ResolveNames 操作](resolvenames-operation.md)に対して無効な場合に発生します。 たとえば、長さ 0 の文字列、1 つのスペース、コンマ、およびダッシュは、すべての無効な名前です。  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |このエラーは、クライアント アクセス サーバー上のネットワーク サービス アカウントでエラーを示します。  <br/> |
|ErrorInvalidOofParameter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidOperation  <br/> | これは、要求された操作が無効である場合に使用される一般的なエラーです。 <br/><br/>たとえば、次の操作を行うことはできません。 <br/> <br/>-パブリック フォルダーに[FindFolder 操作](findfolder-operation.md)を使用して、「詳細」走査を実行します。  <br/>-移動、またはパブリック フォルダーのルートにコピーします。  <br/>-「ハード」を削除する以外のモードを使用して、関連付けられているアイテムを削除します。  <br/>-移動または関連付けられているアイテムをコピーします。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |このエラーは、呼び出し元が別の組織内のユーザーの空き時間情報を要求したが、組織の関係が空き時間情報が有効になってことを示します。  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |このエラーは、ゼロまたは負の値を取得する行の最大数で、消費者が通過するときに発生します。  <br/> |
|ErrorInvalidParentFolder  <br/> |このエラーは、操作に対して無効な親フォルダーに消費者が通過するときに発生します。 たとえば、検索フォルダー内にフォルダーを作成しようとする場合にこのエラーが返されます。  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |とき、タスクの達成率を無効な値に設定しようとしましたが、このエラーが返されます。 0 ~ 100 (両端を含む) の値がある必要があります。  <br/> |
|ErrorInvalidPermissionSettings  <br/> |このエラーは、アクセス許可レベルのアクセス許可の設定と矛盾がないことを示します。  <br/> |
|ErrorInvalidPhoneCallId  <br/> |このエラーは、呼び出し元 id が有効ではないことを示します。  <br/> |
|ErrorInvalidPhoneNumber  <br/> |このエラーは、電話番号が正しくないまたはダイヤル プランのルールに適合しないことを示します。  <br/> |
|ErrorInvalidPropertyAppend  <br/> | 追加しようとしているプロパティが、追加をサポートしていない場合、このエラーが発生します。 <br/><br/>追加モードをサポートする唯一のプロパティは、次のように。 <br/> <br/>-受信者のコレクション (ToRecipients、CcRecipients、BccRecipients)  <br/>出席者コレクション (RequiredAttendees、OptionalAttendees、リソース)  <br/>: 本文  <br/>-ReplyTo  <br/><br/>  さらに、このエラーは、要求で指定された形式でストア内の項目の形式が一致しない場合、メッセージの本文が追加された場合に発生します。  <br/> |
|ErrorInvalidPropertyDelete  <br/> |このエラーは、削除操作が削除操作をサポートしていないプロパティまたは[UpdateFolder](updatefolder-operation.md) [UpdateItem 操作](updateitem-operation.md)の呼び出しで指定されている場合に発生します。 たとえば、 [Item](item.md)オブジェクトの[アイテム Id](itemid.md)要素を削除できません。  <br/> |
|ErrorInvalidPropertyForExists  <br/> |[Exists](exists.md)フィルター フラグ プロパティのいずれかで、消費者が合格した場合、このエラーが発生します。 たとえば、 [IsRead](isread.md)または[IsFromMe](isfromme.md)フラグは、 [Exists](exists.md)要素で指定されている場合に、このエラーが発生します。 要求する必要があります代わりに[IsEqualTo](isequalto.md)要素これらのフラグと 1 つのプロパティの一部であるので。  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |プロパティを操作しようとしているがその上で実行される操作をサポートしていない場合、このエラーが発生します。  <br/> |
|ErrorInvalidPropertyRequest  <br/> | このエラーは、要求で指定されているプロパティがアイテムの種類で利用可能でない場合に発生します。 [GetItem 操作](getitem-operation.md)で、予定表のアイテムでのみ使用されるプロパティが要求された場合にこのエラーが返されます、メッセージ、または[UpdateItem 操作](updateitem-operation.md)で更新されたメッセージの呼び出しです。 <br/> <br/>  これは、次の操作で発生します。 <br/> <br/>- [GetItem 操作](getitem-operation.md) <br/>- [GetFolder の操作](getfolder-operation.md) <br/>- [UpdateItem 操作](updateitem-operation.md) <br/>- [UpdateFolder 操作](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |このエラーは、プロパティを操作しようとしているがその上で実行される操作をサポートしていないことを示します。 たとえば、設定しようとしているプロパティが読み取り専用である場合にこのエラーが返されます。  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | このエラーは、クライアントが既に送信されたメッセージの特定のプロパティを更新するとき、 [UpdateItem 操作](updateitem-operation.md)中に発生します。<br/><br/> たとえば、送信済みのメッセージに次のプロパティを更新できません。 <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |プッシュ サブスクリプション ID を使用して、 [GetEvents 操作](getevents-operation.md)または[登録解除の操作](unsubscribe-operation.md)を呼び出す場合、このエラーが発生します。 、プッシュ サブスクリプションのサブスクリプションを解除するのには、アンサブスク ライブ応答によってプッシュ要求に応答または Web サービスの接続を切断してくださいタイムアウト時間にプッシュ通知を待ちます。  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | 「プッシュ」サブスクリプションを作成し、要求に含まれている URL が有効ではないことを示す場合は、[購読操作](subscribe-operation.md)によってこのエラーが返されます。<br/><br/>URL をそのまま使用する Exchange Web サービスの次の条件を満たす必要があります。 <br/> <br/>-長さの文字列\>0 と\<2083。  <br/>プロトコルは、http または https です。  <br/>URL は、URI の Microsoft.NET Framework のクラスによって解析されます。  <br/> |
|ErrorInvalidRecipients  <br/> |このエラーは、メッセージの受信者コレクションまたは予定表アイテムの出席者コレクションが無効であることを示します。 たとえば、受信者が指定されていないアイテムを送信しようとしましたがときにこのエラーが返されます。  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |このエラーは、検索フォルダーが Exchange Web サービスを表現できない受信者テーブルのフィルターを持っていることを示します。 このエラーを回避するには、検索パラメーターを要求しなくてもフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |このエラーは、検索フォルダーが Exchange Web サービスを表現できない受信者テーブルのフィルターを持っていることを示します。 このエラーを回避するには、検索パラメーターを要求しなくてもフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |このエラーは、検索フォルダーが Exchange Web サービスを表現できない受信者テーブルのフィルターを持っていることを示します。 このエラーを回避するには、検索パラメーターを要求しなくてもフォルダーを取得します。  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |このエラーは、検索フォルダーが Exchange Web サービスを表現できない受信者テーブルのフィルターを持っていることを示します。 このエラーを回避するには、検索パラメーターを要求しなくてもフォルダーを取得します。  <br/> |
|ErrorInvalidReferenceItem  <br/> | このエラーは、次のシナリオでの転送および返信応答オブジェクトに対する[CreateItem 操作](createitem-operation.md)から返されます。<br/>  <br/>-参照されている項目の識別子は、[メッセージ](message-ex15websvcsotherref.md)、[カレンダー項目](calendaritem.md)では、または**メッセージ**または**カレンダー項目**の子ではありません。  <br/>-参照の項目の識別子の**カレンダー項目**開催者が自分自身に返信] または [全員に返信するしようとしています。  <br/>-メッセージは下書きで、返信] または [全員に返信を選択します。  <br/>-参照項目、 [SuppressReadReceipt](suppressreadreceipt.md)は、**メッセージ**または**メッセージ**の子孫ではありません。  <br/> |
|ErrorInvalidRequest  <br/> |このエラーは、SOAP 要求が SOAP 本体の SOAP アクション ヘッダーが、何もが発生します。 SOAP アクション ヘッダーは、Exchange Web サービスは SOAP 本文内のルート要素のローカル名から呼び出す方法を決定することができます、必須ではないことを確認します。  <br/> |
|ErrorInvalidRestriction  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |指定された保持タグにそれに関連付けられている不正な操作がある場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |**PolicyTag**プロパティに存在しない、または非表示のタグを設定するのには試行が行われたときは、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |**PolicyTag**プロパティの暗黙のタグを設定しようと、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |GUID の保持タグが有効なことを示します。  <br/> |
|ErrorInvalidRoutingType  <br/> |このエラーは、 [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)の要素に渡されるルーティングの種類が無効な場合に発生します。 通常、ルーティングの種類は簡易メール転送プロトコル (SMTP) に設定されます。  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |このエラーは、指定した期間の終了時刻が開始時刻より大きい値でない場合、または終了時刻が、将来的に発生しない場合に発生します。  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |このエラーは、プロキシの要求を別のサーバーに送信されましたが、バージョンの不一致のための要求を処理することではないことを示します。  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |このエラーは、ストア内の予定表フォルダーの Exchange セキュリティ記述子が破損していることを示します。  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |このエラーは、 [SavedItemFolderId](saveditemfolderid.md)は、要求で指定されていますが、 **SaveItemToFolder**プロパティが**false**に設定項目の送信の試行中に発生します。  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |このエラーは、ヘッダーで渡されたトークンに形式が正しくありませんし、ディレクトリ内の有効なアカウントを参照していないまたは、プライマリ グループの**ConnectingSID**が不足していることを示します。  <br/> |
|ErrorInvalidSharingData  <br/> |このエラーは、共有メタデータが有効ではないことを示します。 これは、無効な XML で発生することができます。  <br/> |
|ErrorInvalidSharingMessage  <br/> |このエラーは、共有メッセージが有効ではないことを示します。 これは、不足しているプロパティで発生することができます。  <br/> |
|ErrorInvalidSid  <br/> |無効な SID が要求で渡されたときに、このエラーが発生します。  <br/> |
|ErrorInvalidSIPUri  <br/> |このエラーは、SIP の名前、ダイヤル プラン、または電話番号が無効な SIP Uri を示します。  <br/> |
|ErrorInvalidServerVersion  <br/> |このエラーは、無効な要求のサーバーのバージョンが、要求で指定されたことを示します。  <br/> |
|ErrorInvalidSmtpAddress  <br/> |このエラーは、SMTP アドレスを解析できない場合に発生します。  <br/> |
|ErrorInvalidSubfilterType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubscription  <br/> |このエラーは、サブスクリプションが有効ではないことを示します。 クライアント アクセス サーバーを再起動するため、またはサブスクリプションの有効期限が切れているために、この可能性があります。  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |このエラーは、subscribe 要求に複数のパブリック フォルダーの Id が含まれていることを示します。 サブスクリプションは、同じメールボックス ストアまたはパブリック フォルダーの 1 つの ID からの複数のフォルダーを含めることができます。  <br/> |
|ErrorInvalidSyncStateData   <br/> |渡される[同期状態](syncstate-ex15websvcsotherref.md)データが有効でない場合は、 [SyncFolderItems](syncfolderitems.md)または[SyncFolderHierarchy](syncfolderhierarchy.md)によってこのエラーが返されます。 このエラーを修正するには、同期状態に再同期化する必要があります。 確認保持する同期をする場合は Blob の状態、誤って BLOB を切り捨ててはありません。  <br/> |
|ErrorInvalidTimeInterval  <br/> |このエラーは、指定した時間間隔が有効ではないことを示します。 開始時刻は、終了時間以上である必要があります。  <br/> |
|ErrorInvalidUserInfo  <br/> |このエラーでは、アクセス許可の操作を内部的に一貫性のない[ユーザー Id](userid.md)が指定されていることを示します。 などの識別のユーザー ID が指定された既定値 (匿名) の場合は、このエラーが返されますもする場合、SID、またはプライマリ SMTP アドレスを指定するか、このユーザーの名前を表示します。  <br/> |
|ErrorInvalidUserOofSettings  <br/> |このエラーは、ユーザーの Office (OOF) の設定を有効な内部または外部の不足している応答のためを示します。  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Exchange 偽装中にこのエラーが発生します。 SOAP ヘッダーには、ディレクトリにアクセスできませんでした、無効な UPN の呼び出し元に渡されます。  <br/> |
|ErrorInvalidUserSid  <br/> |無効な SID が要求で渡されたときに、このエラーが発生します。  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidValueForProperty  <br/> |このエラーは、制限における比較値が、比較対象のプロパティで無効であることを示します。<br/><br/> たとえば、比較値を[DateTimeCreated](datetimecreated.md)の > **true**はこの応答コードを返します。 <br/><br/>この応答コードは、比較で列挙型プロパティを指定する場合は、比較対象の値がその列挙体の有効な値ではありませんも返されます。  <br/> |
|ErrorInvalidWatermark  <br/> |によって、無効な透かしは、このエラーが発生します。  <br/> |
|ErrorIPGatewayNotFound  <br/> |このエラーは、有効な VoIP ゲートウェイが使用できないことを示します。  <br/> |
|ErrorIrresolvableConflict  <br/> |このエラーは、競合の解決がプロパティの変更を解決するのにはできなかったことを示します。 ストア内の項目が変更されている可能性があり、更新が必要です。 更新された変更キーを取得してからやり直してください。  <br/> |
|ErrorItemCorrupt  <br/> |このエラーは、オブジェクトの状態が破損しているし、取得することはできませんを示します。 アイテムを取得するときにこの状態で、[本文](body.md)や[MimeContent](mimecontent.md)など特定の要素だけになります。 これらの要素を省略し、操作を再試行します。  <br/> |
|ErrorItemNotFound  <br/> |アイテムが見つかりませんでした。 または、アイテムにアクセスする権限がないとき、このエラーが発生します。  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |アイテムのプロパティの要求が失敗した場合、このエラーが発生します。 プロパティが存在する場合がありますが、それを取得できませんでした。  <br/> |
|ErrorItemSave  <br/> |アイテムまたはフォルダーを保存するのには試行が失敗した場合、このエラーが発生します。  <br/> |
|ErrorItemSavePropertyError  <br/> |アイテムまたはフォルダーを保存するために失敗した無効なプロパティの値と、このエラーが発生します。 応答コードには、無効なプロパティのパスが含まれています。  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |このエラーは、可用性サービスが、適切なサイトまたはフォレストに要求をプロキシするネットワーク サービスとしてログオンできることを示します。 この応答は、通常、構成エラーを示します。  <br/> |
|ErrorMailboxConfiguration  <br/> |このエラーは、AD DS 内のメールボックス情報の構成が正しくないことを示します。  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |このエラーは、要求内の[MailboxDataArray](mailboxdataarray.md)要素が空であることを示します。 メールボックスの 1 つ以上の識別子を指定してください。  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |このエラーが発生するは、100 を超えるエントリが[MailboxDataArray](mailboxdataarray.md)要素で指定されます。  <br/> |
|ErrorMailboxFailover  <br/> |このエラーは、メールボックスがフェイル オーバー ・ プロセスのためにメールボックスにアクセスしようが失敗したことを示します。  <br/> |
|ErrorMailboxHoldNotFound  <br/> |メールボックスの保留リストが見つからなかったことを示します。  <br/> |
|ErrorMailboxLogonFailed  <br/> |このエラーは、予定表ビューの情報を取得するためのメールボックスへの接続が失敗したときに発生します。  <br/> |
|ErrorMailboxMoveInProgress  <br/> | このエラーは、別のメールボックス ストアまたはサーバーにメールボックスを移動していることを示します。 このエラーは、メールボックスが別のサーバーまたはメールボックス データベースであるにもわかります。  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | このエラーは、次の条件が発生したエラーのいずれかを示します。  <br/><br/>-メールボックス ストアは、壊れています。  <br/>-メールボックス ストアを停止しています。  <br/>-メールボックス ストアでは、オフラインです。  <br/>にメールボックス ストアにアクセスしようとしたときネットワーク エラーが発生しました。  <br/>-メールボックス ストアでは、オーバー ロードし、これ以上の接続を受け付けることができません。  <br/>-メールボックス ストアが停止されています。  <br/> |
|ErrorMailRecipientNotFound  <br/> |[MailboxData](mailboxdata.md)要素の情報は、有効なメールボックス アカウントにマップできない場合、このエラーが発生します。  <br/> |
|ErrorMailTipsDisabled  <br/> |このエラーは、メール ヒントは無効になっていることを示します。  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |このエラーは、メールボックス内の管理フォルダーが既に作成しようとしているが存在する場合に発生します。  <br/> |
|ErrorManagedFolderNotFound  <br/> |このエラーは、要求で指定されたフォルダー名は、AD DS 内の管理フォルダー定義にマップされない場合に発生します。 のみ、AD DS で定義されているフォルダー用の管理フォルダーのインスタンスを作成できます。 名前を確認してからやり直してください。  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |このエラーは、管理フォルダーのルートがメールボックスから削除されたことや、管理フォルダーのルートの名前を持つ同じ親フォルダーにフォルダーが存在することを示します。 これがルートを作成しようとすると、管理のフォルダーが失敗した場合も発生します。  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |このエラーは、推奨事項を生成しようとしたとき、候補エンジンで問題が発生したことを示します。  <br/> |
|ErrorMessageDispositionRequired  <br/> | このエラーは、 **MessageDisposition**属性が設定されていない場合に発生します。<br/><br/> この属性は、次のような必要です。 <br/> <br/>- [CreateItem 操作](createitem-operation.md)と[UpdateItem 操作](updateitem-operation.md)アイテムの作成中または更新したときには、[メッセージ](message-ex15websvcsotherref.md)です。  <br/>- [CancelCalendarItem](cancelcalendaritem.md)、 [AcceptItem](acceptitem.md)、 [DeclineItem](declineitem.md)、または[TentativelyAcceptItem](tentativelyacceptitem.md)応答オブジェクト。  <br/> |
|ErrorMessageSizeExceeded  <br/> |このエラーは、メッセージを送信しようとしているが許容範囲を超えていることを示します。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |このエラーは、指定されたドメインが見つからないことを示します。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |このエラーは、メッセージ サービスを追跡することはできません、メッセージを追跡することを示します。  <br/> |
| ErrorMessageTrackingTransientError  <br/> |このエラーは、メッセージ追跡用のサービスがダウンまたはビジー状態のいずれかであることを示します。 このエラー コードは、一時的なエラーを示します。 クライアントは、このエラーを受信したときにサーバーに接続を再試行できます。  <br/> |
|ErrorMimeContentConversionFailed  <br/> |MIME コンテンツが、無効である場合にこのエラーが発生、 [CreateItem 操作](createitem-operation.md)の iCal。 [GetItem 操作](getitem-operation.md)では、この応答は、MIME コンテンツを生成できませんでしたを示します。  <br/> |
|ErrorMimeContentInvalid  <br/> |MIME コンテンツが無効である場合、このエラーが発生します。  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |このエラーは、要求の MIME コンテンツがない有効な base 64 文字列である場合に発生します。  <br/> |
|ErrorMissingArgument  <br/> |このエラーは、必要な引数が要求されないことを示します。 応答メッセージのテキストでは、確認する引数を示します。  <br/> |
|ErrorMissingEmailAddress  <br/> |このエラーは、要求を作成したアカウントには、システム上のメールボックスはありませんが、要求で識別フォルダー ID を指定することを示します。 その場合は、 [DistinguishedFolderId](distinguishedfolderid.md)の下にある[メールボックス](mailbox.md)のサブ要素を指定してください。  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |このエラーは、要求を作成したアカウントには、システム上のメールボックスはありませんが、要求で識別フォルダー ID を指定することを示します。 その場合は、 [DistinguishedFolderId](distinguishedfolderid.md)の下にある[メールボックス](mailbox.md)のサブ要素を指定してください。 [CreateManagedFolder 操作](createmanagedfolder-operation.md)からは、この応答が返されます。  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素が存在しない場合、このエラーが発生します。  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |このエラーは、 [ReferenceItemId](referenceitemid.md)が存在しない場合に発生します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラー コードが返されることはありません。  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |[CreateAttachment 操作](createattachment-operation.md)の要求の**ItemAttachment**要素に項目要素を含めないようにしようと、このエラーが返されます。  <br/> |
|ErrorMissingManagedFolderId  <br/> |ポリシー Id プロパティ、プロパティ タグ 0x6732、フォルダーが見つからない場合、このエラーが発生します。 必要がありますこのフォルダーが破損しています。  <br/> |
|ErrorMissingRecipients  <br/> |このエラーは、受信者を指定せずにアイテムを送信しようとすることを示します。 そのメッセージが送信されるメッセージ廃棄を使用して[CreateItem 操作](createitem-operation.md)を呼び出すと、表示されます、次の応答コードに注意してください: **ErrorInvalidRecipients**。  <br/> |
|ErrorMissingUserIdInformation  <br/> |このエラーは、ことの[ユーザー Id](userid.md)完全が指定されていません、アクセス許可セットを示します。  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |このエラーは、要求内の 1 つ以上の[ExchangeImpersonation](exchangeimpersonation.md)要素の値を指定したことを示します。  <br/> |
|ErrorMoveCopyFailed  <br/> |このエラーは、移動またはコピー操作が失敗したことを示します。 移動は、 [CreateItem 操作](createitem-operation.md)で削除済みアイテム フォルダーにある会議出席依頼を承諾するとします。 さらに場合は、予定表アイテムのキャンセル、または予定表から会議を削除する会議出席依頼を辞退する、削除済みアイテム フォルダーに移動します。  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |識別フォルダーを移動しようとすると、このエラーが発生します。  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |このエラーは、要求が複数のメールボックス サーバーにアクセスしようとするときに発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |[ResolveNames 操作](resolvenames-operation.md)が複数の結果を返します。 または、指定したあいまいな名前がディレクトリ内の 1 つ以上のオブジェクトと一致する場合、このエラーが発生します。 応答コードには、応答データで一致する名前が含まれています。  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |このエラーは、呼び出し元が、システム上のメールボックスを持っていないことを示します。 [ResolveNames 操作](resolvenames-operation.md)または[ExpandDL 操作](expanddl-operation.md)は、メールボックスを持たないユーザーを接続するため無効です。  <br/> |
|ErrorNameResolutionNoResults  <br/> |このエラーは、 [ResolveNames 操作](resolvenames-operation.md)に結果が返されないことを示します。  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |このエラー コードは、Web サービス要求を処理するためにサーバーが見つからない場合に返される必要があります。  <br/> |
|ErrorNoCalendar  <br/> |このエラーは、メールボックスの予定表フォルダーがない場合に発生します。  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照ですが、Windows 認証の場合は、移動先サイト内のクライアント アクセス サーバーが構成されていません、そのため、要求できませんでした。 プロキシを示します。  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照ですが、SSL 接続の場合は、移動先サイト内のクライアント アクセス サーバーが構成されていません、そのため要求できませんでした。 プロキシを示します。  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |このエラーことを示します要求が別の Active Directory サイト内のメールボックスに呼ばれますが、要求を受信するのには、許容可能な製品のバージョンのクライアント アクセス サーバーの移動先のサイトがなかったため要求できませんでした。 プロキシ。  <br/> |
|ErrorNoFolderClassOverride  <br/> |このエラーは、汎用フォルダー以外のアイテムを作成するときに[FolderClass](folderclass.md)要素を設定する場合に発生します。 [CalendarFolder](calendarfolder.md)や[TasksFolder](tasksfolder.md)などの型指定されたフォルダーは、フォルダー クラスは暗黙的に指定します。 **ErrorObjectTypeChanged**応答[UpdateFolder 操作](updatefolder-operation.md)の結果を使用して別のフォルダーの種類にフォルダー クラスを設定します。 代わりに、汎用フォルダーを使用するが、フォルダー クラスを必要な値に設定します。 Exchange Web サービスでは、適切な厳密に型指定されたフォルダーを作成します。  <br/> |
|ErrorNoFreeBusyAccess  <br/> |このエラーは、呼び出し元問題のある予定表フォルダーに、空き時間情報を表示する権限がないことを示します。  <br/> |
|ErrorNonExistentMailbox  <br/> | このエラーは、次のシナリオで発生します。 <br/> <br/>-電子メール アドレスが空で[CreateManagedFolder です](createmanagedfolder.md)。  <br/>-電子メール アドレスは、Exchange 偽装呼び出しのように本文または SOAP ヘッダーで、電子メール アドレスを取得する要求に有効なアカウントを参照していません。  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |このエラーは、呼び出し元がプライマリ以外の SMTP アドレスで通過するときに発生します。 応答には、使用する正しい SMTP アドレスが含まれています。  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |このエラーを示している 0x8000 カスタム範囲の MAPI プロパティと、プロパティ タグで参照することはできません。 PropertySetId 属性を使用して EWS のマネージ API の[PropertySetId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)プロパティまたは EWS [ExtendedFieldURI](extendedfielduri.md)要素を使用する必要があります。  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |この応答コードは使用されません。  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |このエラー コードは、パブリック フォルダー サーバーが利用できない場合、または呼び出し元がパブリックのホーム サーバーを持っていない場合に返される必要があります。  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |このエラーは、サイトが応答して、そのため要求できませんでしたプロキシとなったという点で、別の Active Directory サイトがどのクライアント アクセス サーバーのメールボックスに、要求が呼ばれることを示します。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |このエラーは、呼び出し元が別の組織内のユーザーの予定表や連絡先フォルダーにアクセス許可を付与しようとした場合、試行失敗したことを示します。  <br/> |
|ErrorNotDelegate  <br/> |このエラーは、ユーザーがメールボックスの代理人ではないことを示します。 デリゲートのリストで指定した代理ユーザーが見つからない場合は、 [GetDelegate 操作](getdelegate-operation.md)、 [RemoveDelegate の操作](removedelegate-operation.md)、および[UpdateDelegate 操作](updatedelegate-operation.md)によって返されます。  <br/> |
|ErrorNotEnoughMemory  <br/> |このエラーは、操作がメモリ不足のため完了できませんでしたを示します。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |このエラーは、共有メッセージがサポートされていないことを示します。  <br/> |
|ErrorObjectTypeChanged  <br/> |このエラーは、オブジェクトの種類を変更した場合に発生します。  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |このエラーは、発生の[開始](start.md)または[終了](end-ex15websvcsotherref.md)時間は更新され、対応する前または次の発生より前または後に発生する発生が予定されている場合に発生します。  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |このエラーは、同じ定期的なアイテムの別のアイテムに指定されたアイテムの時間配分が重なっていることを示します。 この応答は、指定した回数分の長さは、Int32.MaxValue よりも大きい場合にも発生します。  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |このエラーは、現在の操作がパブリック フォルダーのルートに対して有効ではないことを示します。  <br/> |
|ErrorOrganizationNotFederated  <br/> |このエラーは、依頼者が外部ユーザーに送信する共有メッセージを作成することはできません、または外部のユーザーから受信した共有メッセージを受け付けることができませんので、依頼者の組織を連携させるしないことを示します。  <br/> |
|ErrorParentFolderIdRequired  <br/> |この応答コードは使用されません。  <br/> |
|ErrorParentFolderNotFound  <br/> |このエラーは、親フォルダーが見つからない場合、 [CreateFolder 操作](createfolder-operation.md)で発生します。  <br/> |
|ErrorPasswordChangeRequired  <br/> |このエラーは、このメールボックスにアクセスする前にパスワードを変更することを示します。 これは、新しいアカウントが作成されており、管理者は、ユーザーが最初のログオン時にパスワードを変更する必要があります示されている場合に発生します。 Exchange Web サービスを使用してパスワードを更新することはできません。 パスワードを変更するのに Web アプリケーションの Microsoft Office Outlook などのツールを使用する必要があります。  <br/> |
|ErrorPasswordExpired  <br/> |このエラーは、パスワードの有効期限が切れていることを示します。 Exchange Web サービスを使用してパスワードを変更することはできません。 パスワードを変更するのには、Outlook Web App などのツールを使用する必要があります。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |このエラーは、依頼者の予定表のアクセス許可を付与しようとしたこと、または外部ユーザーですが依頼者に割り当てられている共有ポリシーを [連絡先] フォルダーは、要求されたアクセス許可レベルがどのような共有ポリシーより高いことを示しますを示します。  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |このエラーは、正しい形式で電話番号はなかったことを示します。  <br/> |
|ErrorPropertyUpdate  <br/> |このエラーは、無効なプロパティ値があるため、更新が失敗したことを示します。 応答メッセージには、無効なプロパティのパスが含まれています。  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorPropertyValidationFailure  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |このエラーは、要求が別のクライアント アクセス サーバー上に存在するサブスクリプションに呼ばれますが、プロキシをクライアント アクセス サーバーへの要求に失敗しましたを示します。  <br/> |
|ErrorProxyCallFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照、最初の呼び出し元は 3,000 件を超えるグループのメンバーを示します。  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |このエラーは、 [GetUserAvailabilityRequest](getuseravailabilityrequest.md)要求を実行しようとするとき、Exchange Web サービスが別のクライアント アクセス サーバーに送信される要求が有効なことを示します。 この応答コードは、通常、構成または権限のエラーが発生したこと、または他の人としましたが失敗した可用性のプロキシ要求を模倣することを示します。  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |このエラーは、Exchange Web サービスでプロキシ可用性の要求を別のクライアント アクセス サーバーに処理をしようとしましたが、要求が失敗したことを示します。 この応答は、ネットワーク接続の問題によって発生することができます。 または要求のタイムアウトの問題です。  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |このエラー コードは、Web サービスは、要求がターゲット サーバー上で実行するのには、または別のサーバーに中継されるかどうかを判断できない場合に返される必要があります。  <br/> |
|ErrorProxyTokenExpired  <br/> |この応答コードは使用されません。  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |このエラーは、パブリック フォルダーのメールボックスの URL が見つからない場合に発生します。 このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |このエラーは、パブリック フォルダーにアクセスしようとしましたが、試行が失敗するときに発生します。 このエラーは、2013Exchange サーバーの Exchange 2013 で導入されました。  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |[GetUserAvailability 操作](getuseravailability-operation.md)に渡された受信者が Exchange Server、Exchange 2007 では、および空き時間情報を取得する要求より前のバージョンを実行しているコンピューター上にあるときにこのエラーが発生しますパブリック フォルダー サーバーから受信者に失敗しました。  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |[GetUserAvailability 操作](getuseravailability-operation.md)に渡された受信者が Exchange Server、Exchange 2007 では、および空き時間情報を取得する要求より前のバージョンを実行しているコンピューター上にあるときにこのエラーが発生しますパブリック フォルダー サーバーから受信者は、組織単位に関連付けられたパブリック フォルダー サーバーを持っていないために失敗しました。  <br/> |
|ErrorPublicFolderSyncException  <br/> |このエラーは、同期を実行してプライマリ パブリック フォルダーのメールボックスに対しては成功しますが、2 つ目のパブリック フォルダーのメールボックスに対して成功しない場合に発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorQueryFilterTooLong  <br/> |このエラーは、検索フォルダーの制限が有効な場合がありますが、EWS でサポートされていないことを示します。 Exchange Web サービスでは、最大 255 のフィルター式を格納するための制限を制限します。 255 を超える既存の検索フォルダーにバインドしようとすると、この応答コードが返されます。  <br/> |
|ErrorQuotaExceeded  <br/> |このエラーは、メールボックスのクォータを超えた場合に発生します。  <br/> |
|ErrorReadEventsFailed  <br/> |イベント情報を取得中にエラーが発生した場合は、 [GetEvents 操作](getevents-operation.md)またはプッシュ通知によってこのエラーが返されます。 このエラーが返された場合は、サブスクリプションが削除されます。 最後の既知のウォーターマークに基づいて、イベントの同期を再作成します。  <br/> |
|ErrorReadReceiptNotPending  <br/> |メッセージの送信者がメッセージの開封確認メッセージを要求していない場合、またはメッセージが [迷惑メール] フォルダー内にある場合、開封確認メッセージを抑制しようとした場合は、 [CreateItem 操作](createitem-operation.md)によってこのエラーが返されます。  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |9/1/4500 の後は、定期的なアイテムの終了日と、このエラーが発生します。  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |このエラーは、指定された定期的なアイテムが指定した範囲のすべてのアイテムのインスタンスを持っていない場合に発生します。  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |このエラーは、デリゲートが削除された後で保存するのには、デリゲートのリストが失敗したことを示します。  <br/> |
|ErrorRequestAborted  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRequestStreamTooBig  <br/> | このエラーは、要求ストリームでは、400 KB を超える場合に発生します。  <br/> |
|ErrorRequiredPropertyMissing  <br/> |[CreateAttachment 操作](createattachment-operation.md)の要求の必要なプロパティが見つからない場合、このエラーが返されます。 応答では、不足しているプロパティ URI にはが含まれます。  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |このエラーは、呼び出し元が、 [ResolveNames 操作](resolvenames-operation.md)を [連絡先] フォルダーではないフォルダーを指定したことを示します。  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |このエラーは、呼び出し元が、 [ResolveNames 操作](resolvenames-operation.md)を 1 つ以上の連絡先フォルダーを指定したことを示します。  <br/> |
|ErrorResponseSchemaValidation  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRestrictionTooLong  <br/> |制限には、255 個以上のノードが含まれている場合、このエラーが発生します。  <br/> |
|ErrorRestrictionTooComplex  <br/> |制限は、Exchange Web サービスで評価できない場合、このエラーが発生します。  <br/> |
|ErrorResultSetTooBig  <br/> |このエラーは、指定された受信者の予定表エントリの数が 1000 の許容範囲を超えているを示します。 ウィンドウを縮小してからやり直してください。  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |このエラーは、 [SavedItemFolderId](saveditemfolderid.md)が見つからない場合に発生します。  <br/> |
|ErrorSchemaValidation  <br/> | 要求は、スキーマに照らして検証することはできませんこのエラーが発生します。  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |このエラーは、検索フォルダーが作成されましたが、フォルダーの検索条件が設定されたことはありませんを示します。 これは、別の API またはクライアントを使用して作成された破損した検索フォルダーにアクセスするときにのみ発生します。 このエラーを解決するには、 [SearchParameters](searchparameters.md)要素を含める必要がある場合、フォルダーの制限を設定するのには[UpdateFolder 操作](updatefolder-operation.md)を使用します。  <br/> |
|ErrorSendAsDenied  <br/> | このエラーは、次の条件の両方が発生したときに発生します。 <br/> <br/>-ユーザーは、CanActAsOwner のアクセス許可が与えられては、プリンシパルのメールボックスに対する代理人アクセス権が与えられていません。  <br/>-同じユーザーを作成し、SendAndSaveCopy オプションを使用して、プリンシパルのメールボックスで電子メール メッセージを送信しようとするとします。<br/>  <br/>  ErrorSendAsDenied エラー、およびプリンシパルの [下書き] フォルダー内の電子メール メッセージの作成になります。  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |**SendMeetingCancellations**属性が要求されない、予定表の項目を削除するのには、 [DeleteItem 操作](deleteitem-operation.md)によってこのエラーが返されます。  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |**SendMeetingInvitationsOrCancellations**属性が要求されない、予定表の項目を更新するのには、 [UpdateItem 操作](updateitem-operation.md)によってこのエラーが返されます。  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |**SendMeetingInvitations**属性が要求されない、予定表の項目を作成するのには、 [CreateItem 操作](createitem-operation.md)によってこのエラーが返されます。  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |このエラーは、その開催者が会議出席依頼を送信した後、要求を更新できませんを示します。 会議を変更するには、会議出席依頼ではなく、予定表アイテムを変更します。  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |このエラーは、その仕事の開始者は、仕事の依頼を送信した後その依頼を更新できませんを示します。  <br/> |
|ErrorServerBusy  <br/> |このエラーは、サーバーがビジー状態のときに発生します。  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |このエラーは、Exchange Web サービス プロキシ ユーザーの可用性要求を適切なフォレストに、受信者のサービスの検出エラーのため要求を送信する場所を特定できませんでしたを示します。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |このエラーは、Active Directory データベースの外部の URL プロパティが設定されていないことを示します。  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |このエラーは、共有フォルダーの同期時の試行が失敗したことを示します。 <br/><br/>次の場合、このエラー コードが返されます。<br/><br/>-共有フォルダーのサブスクリプションが見つかりませんでした。<br/>-共有フォルダーが見つかりません。<br/>-対応するディレクトリのユーザーが見つかりませんでした。<br/>-ユーザーが存在しません。<br/>予定が正しくありません。<br/>連絡先アイテムを使用することはできません。<br/>-は、リモート サーバーとの通信障害です。  <br/> |
|ErrorStaleObject  <br/> |このエラーは、キーの変更、更新されていないか指定されていない場合、 [UpdateItem 操作](updateitem-operation.md)または[SendItem 操作](senditem-operation.md)で発生します。 更新された変更キーを取得してから、もう一度[GetItem 操作](getitem-operation.md)を呼び出します。  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |このエラーは、ユーザーすぐに送信できないより多くの要求送信クォータに達したためにことを示します。  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |このエラーは、そのサブスクリプションを作成していないアカウントを使用してサブスクリプションにアクセスしようとするときに発生します。 各サブスクリプションは、サブスクリプションの作成者だけがアクセスできます。  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |このエラーは、所有者ではないか、メールボックス所有者のアクセス権はありません、サブスクリプションを作成できないことを示します。  <br/> |
|ErrorSubscriptionNotFound  <br/> |このエラーは、指定した[サブスクリプション Id (GetEvents)](subscriptionid-getevents.md)に対応するサブスクリプションが見つからなかった場合に発生します。 サブスクリプションの期限が切れている可能性があります、Exchange Web サービスのプロセスが再起動されたか、無効なサブスクリプションが渡されました。 サブスクリプションが有効だった場合は、最新のウォーターマークを使用してサブスクリプションを再作成します。 これは、[購読の取り消し操作](unsubscribe-operation.md)または[GetEvents 操作](getevents-operation.md)の応答が返されます。  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |要求が行われると、このエラー コードを返す必要がありますサブスクライブされたサブスクリプションにします。  <br/> |
|ErrorSyncFolderNotFound  <br/> |指定されている親フォルダーが見つからない場合は、 [SyncFolderItems 操作](syncfolderitems-operation.md)によってこのエラーが返されます。  <br/> |
|ErrorTeamMailboxNotFound  <br/> |このエラーは、チームのメールボックスが見つからなかったことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |このエラーは、チームのメールボックスが見つかりましたが、SharePoint サーバーにリンクされていないことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |このエラーは、チームのメールボックスが見つかりましたが、SharePoint サーバーへのリンクが有効ではないことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |このエラー コードは使用されません。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |このエラー コードは使用されません。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |このエラーは、チームのメールボックスの所有者に通知を送信する試みが失敗したことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |このエラーは、チームのメールボックスにアクセスしようとするときに発生する可能性がある一般的なエラーを示します。 後で要求を送信してください。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTimeIntervalTooBig  <br/> |このエラーは、指定された時間ウィンドウが許可されている制限よりも大きいことを示します。 既定で許可されている制限は、42 です。  <br/> |
|ErrorTimeoutExpired  <br/> | このエラーは、要求の処理を完了するのに十分な時間がない場合に発生します。  <br/> |
|ErrorTimeZone  <br/> |このエラーは、タイム ゾーンのエラーがあることを示します。  <br/> |
|ErrorToFolderNotFound  <br/> |このエラーは、インストール先フォルダーが存在しないことを示します。  <br/> |
|ErrorTokenSerializationDenied  <br/> |このエラーは、呼び出し元のトークンのシリアル化要求を実行しようとしています。 ですが、クライアント アクセス サーバー上の ms-Exch ・ EPI ・ TokenSerialization がない場合に発生します。  <br/> |
|ErrorTooManyObjectsOpened  <br/> |このエラーは、開いているオブジェクトの内部制限を超えているときに発生します。  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |このエラーは、ユーザーのダイヤル プランが利用できないことを示します。  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |このエラーはユーザーが見つかりませんことを示します。  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |このエラーは、要求を処理するためにダイヤル プランに対して有効なサーバーが見つかることを示します。  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |IM の連絡先をグループから削除するのには失敗が行われると、このエラーが発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUnsupportedCulture  <br/> |**オペレ**クラスによって解析ではない値に**カルチャ**プロパティを設定しようとするとき、このエラーが発生します。  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |このエラーは、呼び出し元の種類のオブジェクト、オブジェクト配列、エラー、または null の拡張プロパティを使用しようとするときに発生します。  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |[PostItem](postitem.md)、[メッセージ](message-ex15websvcsotherref.md)、または[カレンダー項目](calendaritem.md)のオブジェクト以外のアイテムの MIME コンテンツの設定を取得またはしようとしている場合、このエラーが発生します。  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |このエラーは、呼び出し元は、クエリに無効なプロパティを通過するときに発生します。 これは、計算されたプロパティを使用する場合に発生します。  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |このエラーは、呼び出し元は、並べ替えまたはグループ化プロパティの無効なプロパティを通過するときに発生します。 これは、計算されたプロパティを使用する場合に発生します。  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |このエラーは、検索フォルダーの制限が有効な場合がありますが、EWS でサポートされていないことを示します。  <br/> |
|ErrorUnsupportedRecurrence  <br/> |このエラーは、タスクに対して指定した定期的なアイテムがサポートされていないことを示します。  <br/> |
|ErrorUnsupportedSubFilter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |このエラーは、Exchange Web サービスは、ストアでプロパティの種類を検出するが、プロパティの型の XML を生成することはできませんを示します。  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |このエラーは、代理人が更新された後で保存するのには、デリゲートのリストが失敗したことを示します。  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |このエラーは、変更の説明に記載されている 1 つのプロパティのパスが実際の[アイテム](item.md)または[フォルダー](folder.md)のオブジェクト内で設定される 1 つのプロパティと一致しない場合に発生します。  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |このエラーは、依頼者が有効でないことを示します。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |このエラーは、依頼者の予定表のアクセス許可を付与しようとしたこと、または外部ユーザーですが依頼者に割り当てられている共有ポリシーを [連絡先] フォルダーは、ポリシー内の外部ユーザーのドメインが表示されていないことを示しますを示します。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |依頼者の組織のフェデレーション ドメインのセットには依頼者の組織には、フェデレーション ドメインのいずれかの SMTP プロキシ アドレスがないことを示します。  <br/> |
|ErrorValueOutOfRange  <br/> |このエラーは、[カレンダー] ビューの開始日または終了日が 1/1/0001 に設定されてのことを示します 12時 00分: 00 または 12/31/9999 11時 59分: 59 PM。  <br/> |
|ErrorVirusDetected  <br/> |このエラーは、Exchange ストアがメッセージのウイルスを検出することを示します。  <br/> |
|ErrorVirusMessageDeleted  <br/> |このエラーは、Exchange ストアはメッセージでウイルスを検出し、削除を示します。  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWebRequestInInvalidState  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWin32InteropError  <br/> |このエラーは、アンマネージ コードとの通信中に内部エラーがあったことを示します。  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWrongServerVersion  <br/> |このエラーは、要求はメールボックス サーバーと同じバージョンではサーバーにしか適用できることを示します。  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |このエラーは、要求が主体のメールボックス サーバーと別のサーバーのバージョンを持つ代理人によって行われたことを示します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラー コードが返されることはありません。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |SOAP ヘッダーの重複があることを指定します。  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | 共有フォルダーの同期時の試行が失敗したことを指定します。<br/><br/> このエラー コードする必要がある場合、返されます。<br/><br/>-共有フォルダーのサブスクリプションが見つかりませんでした。  <br/>-共有フォルダーが見つかりませんでした。  <br/>-対応するディレクトリのユーザーは見つかりませんでした。  <br/>-ユーザーが存在しません。  <br/>予定が正しくありません。  <br/>連絡先アイテムを使用することはできません。  <br/>-リモート サーバーと通信エラーが発生しました。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Active Directory データベースの外部の URL プロパティが設定されていないことを指定します。 このエラー コードは、Active Directory データベース内の外部の URL プロパティが設定されていない場合に返される必要があります。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |配布リスト用の空き時間情報を取得するため、最大のグループのメンバーの数に達して ことを指定します。 このエラーは、配布リスト用の空き時間情報を取得するため、最大のグループのメンバーの数に到達したときに返されます必要があります。  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |ShareFolderId データ型と要素の両方の要求内に存在があることを指定します。 このエラー コードは、データ型および ShareFolderId の要素は、両方の要求である場合に返される必要があります。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |呼び出し元がの別の組織および失敗したユーザーに、予定表や連絡先フォルダーにアクセス許可を付与しようとしたことを指定します。 呼び出し元または呼び出し元に割り当てられている共有ポリシーが要求されたレベルまたは要求されたフォルダーの種類の共有を禁止するときの共有ポリシーが無効になっている場合、このエラー コードを返す必要があります。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |指定、リクエスターが、その予定表のアクセス許可を付与しようとしています。 外部のユーザーも、リクエスターに割り当てられている共有ポリシーを [連絡先] フォルダーは、ポリシー内の外部ユーザーのドメインが表示されていないことを指定します。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |リクエスターを外部のユーザーも、リクエスターに割り当てられている共有ポリシーをその予定表や連絡先のフォルダーのアクセス許可が要求されたアクセス許可レベルが高いことを指定を許可しようとしていますが、共有ポリシーがどのようなを指定します。  <br/> |
|ErrorOrganizationNotFederated  <br/> |リクエスターを外部ユーザーに送信する共有メッセージを作成することはできませんまたは外部のユーザーから受信した共有メッセージを受け付けることができませんので、要求側の組織を連携させるされませんを指定します。 このエラー コードは、要求側の組織が連携していない場合に返される必要があります。  <br/> |
|ErrorMailboxFailover  <br/> |メールボックスがフェイル オーバー ・ プロセスのためにメールボックスにアクセスしようが失敗したことを指定します。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |共有への招待の送信者が共有の招待状のメタデータを作成していないことを指定します。 共有への招待の送信者は、共有の招待状のメタデータを作成していない場合、このエラー コードを返す必要があります。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |メッセージ サービスを追跡することはできません、メッセージを追跡することを指定します。  <br/> |
|ErrorMessageTrackingTransientError  <br/> |追跡サービスのいずれかのメッセージが下方向またはビジー状態であることを示します。 このエラー コードは、一時的なエラーを指定します。 クライアントは、このエラーを受信したときにサーバーに接続を再試行できます。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |指定されたドメインが見つからないことを指定します。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |要求側の組織のフェデレーション ドメインのセットには要求側の組織には、フェデレーション ドメインのいずれかの SMTP プロキシ アドレスがないことを示します。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |呼び出し元が別の組織内のユーザーの空き時間情報を要求した組織の関係が空き時間有効になっていることを示します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |要求側の組織のフェデレーション オブジェクトが正しく構成されていないことを指定します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |共有メッセージが呼び出し元の目的としていないことを指定します。  <br/> |
|ErrorInvalidSharingData  <br/> |共有メタデータが有効ではないことを指定します。 これは、無効な XML で発生することができます。  <br/> |
|ErrorInvalidSharingMessage  <br/> |共有メッセージが有効ではないことを指定します。 これは、不足しているプロパティで発生することができます。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |共有メッセージがサポートされていないことを指定します。  <br/> |
|ErrorApplyConversationActionFailed  <br/> |このエラーは、スレッドの 1 つまたは複数のアイテムにアクションを適用できない場合に返されます必要があります。  <br/> |
|ErrorInboxRulesValidationError  <br/> |このエラーは、すべてのルールが検証されない場合に返されます必要があります。  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |このエラーは、別のクライアントは、受信トレイ ルールをアクセスした後、受信トレイ ルールを管理しようとするが発生したときに返されます必要があります。  <br/> |
|ErrorRulesOverQuota  <br/> |このエラーは、ユーザーのルール クォータを超過したときに返されます必要があります。  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |このエラーは、2 番目のサブスクリプションの接続が開かれている場合、サブスクリプションの最初の接続に返されます必要があります。  <br/> |
|ErrorMissedNotificationEvents  <br/> |このエラーは、イベント通知が失敗したときに返されます必要があります。  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Active Directory ドメイン サービス (AD DS) 内に従来の識別名が重複しているが存在する場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |このエラーは、クライアントのアクセス トークンを取得するための要求が有効なことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorNoSpeechDetected  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUMServerUnavailable  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorRecipientNotFound  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorRecognizerNotInstalled  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSpeechGrammarError  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |SOAP ヘッダーの[ManagementRole](managementrole.md)ヘッダーが正しくない場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorLocationServicesDisabled  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |このエラーは内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorWeatherServiceDisabled  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |コンテンツ検索のインデックスの[クエリ文字列 (String)](querystring-string.md)の要素を使用せず、対象とした検索の試行が実行されると、このエラーが返されます。 これは、 **SearchMailboxes**と**FindConversation**の操作に適用されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |このエラーは、アーカイブ メールボックスの検索が失敗したときに返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |アーカイブ メールボックスの URL が検出できない場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |このエラーは、リモート ・ アーカイブ メールボックスのフォルダーを取得する操作が失敗したときに発生します。  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |このエラーは、リモート ・ アーカイブのメールボックス フォルダーを検索する操作が失敗したときに発生します。  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |このエラーは、リモート ・ アーカイブのメールボックスのアイテムを取得する操作が失敗したときに発生します。  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |このエラーは、リモート ・ アーカイブ メールボックスのアイテムをエクスポートする操作が失敗したときに発生します。  <br/> |
|ErrorInvalidPhotoSize  <br/> |サーバーから、無効な写真のサイズが要求された場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |**GetUserPhoto**操作の要求で、予期しない写真のサイズが要求されたときは、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |**SearchMailboxes**操作の要求には、多くのメールボックスを検索するが含まれている場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |このエラーは、このユーザーの保持タグが見つかりませんだったことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |テナントまたはサーバーの検索が無効になっている場合、このエラーが返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |このエラーは、呼び出しの[SeekToConditionPageItemView](seektoconditionpageitemview.md)と[FindItem 操作](finditem-operation.md)のサポートされていない予定表アイテムをフェッチするためにしようとしたときに発生します。  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |このエラーは内部使用のみを目的としています。  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |テナントは削除対象としてマークします。  <br/> |
|ErrorInvalidLicense  <br/> |ユーザーは、有効なライセンスを持っていません。  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |フォルダーごとのメッセージが表示されるクォータを超えています。  <br/> |
   
## <a name="remarks"></a>備考

この要素は必須ではなく、すべての応答に含まれません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

