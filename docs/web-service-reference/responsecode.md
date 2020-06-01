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
description: 応答 Secな要素は、要求に関する状態情報を提供します。
ms.openlocfilehash: 6481272c61aab3dc9aeb2fd988e3544169306f06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457467"
---
# <a name="responsecode"></a>ResponseCode

応答**secな**要素は、要求に関する状態情報を提供します。 
  
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
|[ResponseMessage](responsemessage.md) <br/> | 応答状態に関する説明情報を提供します。<br/><br/>  この要素に使用できる XPath 式は次のとおりです。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |単一の[DeleteItem 操作](deleteitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |単一の[SendItem 操作](senditem-operation.md)要求の状態と結果を格納します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |1つの[Deletefolder 操作](deletefolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |1回の[Deleteattachment 操作](deleteattachment-operation.md)要求の状態と結果を格納します。  <br/> |
|[非表示の表示/非表示のメッセージ](unsubscriberesponsemessage.md) <br/> |1回の登録[解除操作](unsubscribe-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の[CreateFolder 操作](createfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1つの[Getfolder 操作](getfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |1つの[Updatefolder 操作](updatefolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1つの[Movefolder 操作](movefolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1つの[Copyfolder 操作](copyfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |単一の[CreateManagedFolder 操作](createmanagedfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |単一の[Findfolder 操作](findfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |単一の[CreateItem 操作](createitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |単一の[GetItem 操作](getitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |1つの[Updateitem 操作](updateitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1つの[Moveitem 操作](moveitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |1つの[Copyitem 操作](copyitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1つの[Createattachment 操作](createattachment-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1つの[Getattachment 操作](getattachment-operation.md)要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1つの[FindItem 操作](finditem-operation.md)要求の状態と結果を格納します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |[ResolveNames 操作](resolvenames-operation.md)要求の状態と結果を格納します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1つの[Expanddl 操作](expanddl-operation.md)要求の状態と結果を格納します。  <br/> |
|[メッセージの表示](subscriberesponsemessage.md) <br/> |単一の[サブスクライブ操作](subscribe-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |単一の[GetEvents 操作](getevents-operation.md)要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1回の SendNotification 操作要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |[Syncfolderhierarchy 操作](syncfolderhierarchy-operation.md)要求の状態と結果を格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[Syncfolderitems 操作](syncfolderitems-operation.md)要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |[状態]-[バケット][操作](convertid-operation.md)要求の状態と結果を格納します。  <br/> |
|[含む adddelegateresponse](adddelegateresponse.md) <br/> |[Adddelegate 操作](adddelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |[Getdelegate 操作](getdelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |[Removedelegate 操作](removedelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |[代理人操作](updatedelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |[GetServerTimeZones 操作](getservertimezones-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |[Getsharingfolder 操作](getsharingfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |[Getsharingfolder 操作](getsharingfolder-operation.md)要求への応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |[Getsharingmetadata 操作](getsharingmetadata-operation.md)要求への応答を定義します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |[Refreshsharingfolder 操作](refreshsharingfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |[Refreshsharingfolder 操作](refreshsharingfolder-operation.md)要求への応答を定義します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |[Findconversation 操作](findconversation-operation.md)の応答の状態と結果を格納します。  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |[ApplyConversationAction 操作](applyconversationaction-operation.md)要求の状態と結果を格納します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |単一の[Emptyfolder 操作](emptyfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[Update受信トレイルールの応答](updateinboxrulesresponse.md) <br/> |[Update受信トレイルール操作](updateinboxrules-operation.md)要求の状態と結果を格納します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |[UploadItems 操作](uploaditems-operation.md)要求の状態と結果を格納します。  <br/> |
|[Get受信規則の応答](getinboxrulesresponse.md) <br/> |[Get受信トレイの操作](getinboxrules-operation.md)* * * * 要求に対する応答を含みます。  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)要求への応答を含みます。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、テキスト値が必要です。 次の表では、この要素で返される値について説明します。
  
|値|説明|
|:-----|:-----|
|NoError  <br/> |要求に対してエラーが発生していません。  <br/> |
|ErrorAccessDenied  <br/> |このエラーは、呼び出し元のアカウントに、要求された操作を実行する権限がない場合に発生します。  <br/> |
|ErrorAccessModeSpecified  <br/> |このエラーは、内部使用のみを対象としています。 このエラーは返されません。  <br/> |
|ErrorAccountDisabled  <br/> |このエラーは、対象のアカウントが無効になっている場合に発生します。  <br/> |
|ErrorAddDelegatesFailed  <br/> |このエラーは、代理人が追加されたリストを保存できない場合に発生します。  <br/> |
|Erroraddressでした。  <br/> |このエラーは、フォレスト間の可用性のアドレス空間レコードまたはドメインネームシステム (DNS) ドメイン名が Active Directory データベースで見つからない場合に発生します。  <br/> |
|ErrorADOperation  <br/> |このエラーは、Active Directory ドメインサービス (AD DS) との通信に問題が発生したために操作が失敗した場合に発生します。  <br/> |
|ErrorADSessionFilter  <br/> |このエラーは、 **ResolveNames**操作要求で無効な名前が指定されている場合に返されます。  <br/> |
|ErrorADUnavailable 不可  <br/> |このエラーは、AD DS が使用できない場合に発生します。 後で要求を再試行してください。  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |このエラーは、 **AffectedTaskOccurrences**属性が指定されていなかったことを示します。 [DeleteItem](deleteitem.md)要素を使用して、タスクである少なくとも1つの項目を削除し、そのタスクが定期かどうかに関係なく、 **AffectedTaskOccurrences**属性を指定する必要があります。これにより、 **DeleteItem**は現在のオカレンスを削除するか、データ系列全体を削除するかを決定することができます。  <br/> |
|Errorアーカイブ Folderpathの作成  <br/> |アーカイブフォルダーのパスの作成でエラーが発生したことを示します。  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |アーカイブメールボックスが有効になっていないことを示します。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |アーカイブメールボックスサービスの検出が失敗したことを示します。  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |入れ子にされた10個を超える添付ファイルを持つアイテムを作成しようとしたことを指定します。 この値は、Exchange Server 2010 Service Pack 2 (SP2) で導入されました。  <br/> |
|ErrorAttachmentSizeLimitExceeded 超過しました  <br/> |Int32 を超えるサイズの添付ファイルを作成しようとした場合、 [createattachment](createattachment.md)要素はこのエラーを返します。 MaxValue はバイト単位です。  <br/> Int32 を超えるサイズの既存の添付ファイルを取得しようとした場合、 [Getattachment](getattachment.md)要素はこのエラーを返します。 MaxValue はバイトです。  <br/> |
|ErrorAutoDiscoverFailed  <br/> |このエラーは、Exchange Web サービス2010が、自動検出サービスを使用して、クライアントアクセスサーバーの役割がインストールされているフォレスト間のコンピューターの場所を判断しようとしたが、自動検出サービスの呼び出しが失敗したことを示します。  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |このエラーは、ローカルフォレストの可用性構成情報が AD DS にないことを示します。  <br/> |
|ErrorBatchProcessingStopped  <br/> | このエラーは、アイテムの処理中に例外が発生し、その後に続くアイテムに対してその例外が発生する可能性があることを示しています。 要求には複数のアイテムを含めることができます。たとえば、GetItem 操作要求には複数の識別子を含めることができます。 一般に、アイテムは一度に1つずつ処理されます。 アイテムの処理中に例外が発生し、その後のアイテムでその例外が発生する可能性がある場合は、次のアイテムは処理されません。  <br/><br/>  以下に、次のようなアイテムの処理を停止するエラーの例を示します。<br/>  <br/>-ErrorAccessDenied  <br/>-ErrorAccountDisabled  <br/>-ErrorADUnavailable 不可  <br/>-ErrorADOperation  <br/>-ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |このエラーは、定期的な予定表アイテムの発生を移動またはコピーしようとしたときに発生します。  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | このエラーは、削除済みアイテムフォルダーにある予定表アイテムを更新しようとしたとき、および会議の更新または取り消しが**SendMeetingInvitationsOrCancellations**属性の値に従って送信される場合に発生します。 <br/><br/>次に、この属性で使用できる値を示します。  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>-SendOnlyToChanged  <br/>  <br/>ただし、このような更新は、この属性の値が SendToNone に設定されている場合にのみ許可されます。  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |このエラーは、UpdateItem、GetItem、DeleteItem、MoveItem、CopyItem、または SendItem 操作が呼び出されたときに、指定された ID が定期的な予定表アイテムの発生 ID ではない場合に発生します。  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |このエラーは、 **Updateitem**、 **GetItem**、 **DeleteItem**、 **Moveitem**、 **copyitem**、または**SendItem**操作が呼び出されたときに、指定された id が定期的なマスターアイテムの id ではない場合に発生します。  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |このエラーは、予定表アイテムの期間が許可された最大値 (現在は5年) を超えている場合に、 **CreateItem**または**updateitem**操作中に発生します。  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |このエラーは、予定表の終了時刻が同じ時刻に設定されている場合、または開始時刻を過ぎた場合に発生します。  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |このエラーは、 [CalendarView](calendarview.md)要素を持つ**FindItem**操作の指定したフォルダーが、予定表フォルダーの種類ではない場合に発生します。  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |このエラーは、 **CreateItem**または**updateitem**操作中に、日付、WeekendDay、および曜日の無効な値が時間変更パターンの定義に使用される場合に発生します。  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |このエラーは、 **CreateItem**または**updateitem**操作中に、曜日、曜日、WeekendDay の無効な値を使用して週単位の繰り返しを指定すると発生します。  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |このエラーは、Exchange ストア内の予定表アイテムの定期的なバイナリラージオブジェクト (BLOB) の状態が無効である場合に発生します。  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |この応答コードは使用されません。  <br/> |
|ErrorCalendarInvalidRecurrence なアイテム  <br/> |このエラーは、指定した定期的な予定を作成できない場合に発生します。  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |このエラーは、無効なタイムゾーンが検出された場合に発生します。  <br/> |
|Errorcalendariscancel/承諾  <br/> |このエラーは、予定表アイテムが取り消されたことを示します。  <br/> |
|Errorcalendariscancel/辞退  <br/> |このエラーは、予定表アイテムが取り消されたことを示します。  <br/> |
|Errorcalendariscancel/削除  <br/> |このエラーは、予定表アイテムが取り消されたことを示します。  <br/> |
|Errorcalendariscancel/仮承諾  <br/> |このエラーは、予定表アイテムが取り消されたことを示します。  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |このエラーは、委任されたシナリオで、 [Acceptitem](acceptitem.md)要素が予定表アイテムまたは会議出席依頼に対して無効であることを示します。  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |このエラーは、委任されたシナリオで、 [Declineitem](declineitem.md)要素が予定表アイテムまたは会議出席依頼に対して無効であることを示します。  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |このエラーは、委任されたシナリオでは、 [Removeitem](removeitem.md)要素が会議の取り消しに対して無効であることを示しています。  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |このエラーは、委任されたシナリオで、 [TentativelyAcceptItem](tentativelyacceptitem.md)要素が予定表アイテムまたは会議出席依頼に対して無効であることを示します。  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |このエラーは、予定表アイテムの操作 (現在はキャンセルアイテム) が出席者に対して有効ではないことを示します。 会議の開催者のみが会議を取り消すことができます。  <br/> |
|Errorcalendarisオーガナイザー Erforaccept  <br/> |このエラーは、 [Acceptitem](acceptitem.md)が開催者の予定表アイテムに対して無効であることを示します。  <br/> |
|Errorcalendarisオーガナイザー Erfor辞退  <br/> |このエラーは、 [Declineitem](declineitem.md)が開催者の予定表アイテムに対して無効であることを示します。  <br/> |
|Errorcalendarisオーガナイザー Erforremove  <br/> |このエラーは、 [Removeitem](removeitem.md)が開催者の予定表アイテムに対して無効であることを示します。 予定表から会議を削除するには、開催者は CancelCalendarItem を使用する必要があります。  <br/> |
|Errorcalendarisオーガナイザー Erfor仮設  <br/> |このエラーは、 [TentativelyAcceptItem](tentativelyacceptitem.md)が開催者の予定表アイテムに対して無効であることを示します。  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |このエラーは、会議出席依頼が古く、更新できないことを示します。  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |このエラーは、オカレンスインデックスが現在の定期的なアイテムを指していないことを示します。 たとえば、定期的なパターンで3つの会議の予定を定義している場合に、5回目の会議にアクセスしようとすると、この応答コードが生成されます。  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |このエラーは、削除されたアイテム (定期的なマスター ID とオカレンスインデックスを介してアドレス指定されたもの) に対して何らかの操作が無効であることを示します。  <br/> |
|ErrorCalendarOutOfRange  <br/> |このエラーは、プロパティ値が範囲外の場合に、予定表アイテムまたはタスクの繰り返しのプロパティの CreateItem および UpdateItem 操作で報告されます。 たとえば、月の15週を指定すると、この応答コードが生成されます。  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |このエラーは、 [CalendarView](calendarview.md)要素の開始範囲の終了が許容最大値 (現在は2年) を超える場合に発生します。  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |このエラーは、要求元のアカウントがディレクトリデータベースの有効なアカウントではないことを示します。  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |予定表連絡先タスクフォルダーのアーカイブが試行されたことを示します。  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |パブリックフォルダー内のアイテムのアーカイブが試みられたことを示します。  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |アーカイブメールボックス内のアイテムのアーカイブが試みられたことを示します。  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |このエラーは、予定表アイテムが作成されており、 **SavedItemFolderId**属性が非予定表フォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |このエラーは、連絡先が作成され、 **SavedItemFolderId**属性が連絡先以外のフォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |このエラーは、予定表、連絡先、タスク、メモなど、メールフォルダー以外のフォルダーに投稿アイテムを作成できないことを示します。  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |このエラーは、タスクが作成され、 **SavedItemFolderId**属性が非タスクフォルダーを参照している場合に発生します。  <br/> |
|ErrorCannotDeleteObject  <br/> |このエラーは、削除するアイテムまたはフォルダーを削除できない場合に発生します。  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |[DeleteItem 操作](deleteitem-operation.md)は、定期的なタスクの現在の発生を削除しようとして失敗した場合に、このエラーを返します。 これが発生するのは、AffectedTaskOccurrences 属性が、 **AffectedTaskOccurrences**属性が設定されている場合のみです。  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Mandatorty 拡張機能を無効にしようとしたことを示します。  <br/> |
|ErrorCannotEmptyFolder  <br/> |サーバーがフォルダーを空にできない場合、このエラーが返される必要があります。  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |ソースフォルダーのパスを取得できなかったことを示します。  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |サーバーが Outlook Web App のオプションの外部 URL を取得できなかったことを指定します。  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |**Getattachment**操作は、添付ファイルの本文を取得できない場合にこのエラーを返します。  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |このエラーは、呼び出し元が予定のないフォルダーに対して予定表のアクセス許可を設定しようとしたことを示します。  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |このエラーは、発信者が予定表フォルダーに対して予定表以外のアクセス許可を設定しようとしたことを示します。  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |このエラーは、アクセス許可セットに不明なアクセス許可を設定できないことを示します。  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |検索フォルダーをソースフォルダーとして指定しようとしたことを示します。  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |このエラーは、アイテム識別子を必要とする要求にフォルダー識別子が指定されている場合に発生します。  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |このエラーは、フォルダー識別子を必要とする要求にアイテム識別子が指定されている場合に発生します。  <br/> |
|ErrorChangeKeyRequired  <br/> |この応答コードは、 **Errorchangekeyrequiredforwriteoperations**に置き換えられました <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |このエラーは、アイテムの変更キーが見つからないか、または古くなっている場合に返されます。 <br/><br/>SendItem、UpdateItem、および Updateitem 操作の場合、呼び出し元は、アイテムの正しいおよび現在の変更キーを渡す必要があります。 これは、競合の解決が常に上書きされるように設定されている場合でも、UpdateItem に該当することに注意してください。  <br/> |
|ErrorClientDisconnected  <br/> |クライアントが切断されたことを指定します。  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorClientIntentNotFound  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorConnectionFailed  <br/> |このエラーは、Exchange Web サービスがメールボックスに接続できない場合に発生します。  <br/> |
|ErrorContainsFilterWrongType  <br/> |このエラーは、に対して検査されたプロパティが文字列型ではないことを示します。  <br/> |
|ErrorContentConversionFailed  <br/> |**GetItem**操作は、Exchange Web サービスが要求されたアイテムの MIME コンテンツを取得できない場合にこのエラーを返します。 <br/><br/>Exchange Web サービスが提供された MIME コンテンツからアイテムを作成できない場合、 **CreateItem**操作はこのエラーを返します。 通常、これは、アイテムのプロパティが破損しているか、切り捨てられていることを示します。  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |このエラーは、検索要求が QueryString オプションを使用して行われ、対象のメールボックスに対してコンテンツのインデックス処理が有効になっていない場合に発生します。  <br/> |
|ErrorCorruptData  <br/> |このエラーは、データが破損して処理できない場合に発生します。  <br/> |
|ErrorCreateItemAccessDenied  <br/> |このエラーは、呼び出し元にアイテムを作成する権限がない場合に発生します。  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |このエラーは、CreateManagedFolder 操作要求で指定された1つ以上の管理フォルダーの作成に失敗した場合に発生します。 各フォルダーを検索して、どのフォルダーが作成され、どのフォルダーが存在しないかを確認します。  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |このエラーは、呼び出し元のアカウントにサブフォルダーの作成に必要なアクセス許可がない場合に発生します。  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |このエラーは、あるメールボックスから別のメールボックスにアイテムまたはフォルダーを移動しようとしたときに発生します。 移行元メールボックスと移動先メールボックスが異なる場合、このエラーが表示されます。  <br/> |
|Errorクロスバー Sit/その他の方法  <br/> |このエラーは、要求を処理する必要があるクライアントアクセスサーバーが別のサイトにあるため、要求が許可されていないことを示します。  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |このエラーは、次のシナリオで発生します。<br/>  <br/>-アイテムのプロパティへのアクセスまたは書き込みが行われましたが、プロパティの値が大きすぎます。<br/>-要求 XML 内の base64 でエンコードされた MIME コンテンツの長さが制限を超えています。<br/>-既存のアイテム本文の本文のサイズが制限を超えています。<br/>-コンシューマーは HTML またはテキストの本文を設定しようとしています。この値は、長さ (append の場合は文字の長さの組み合わせ) を超えています。 |
|ErrorDataSourceOperation  <br/> |このエラーは、基になるデータプロバイダーで操作の完了に失敗した場合に発生します。  <br/> |
|ErrorDelegateAlreadyExists  <br/> |このエラーは、指定されたユーザーが代理人の一覧に既に存在する場合に、 **Adddelegate**操作で発生します。  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |このエラーは、追加する指定されたユーザーがメールボックスの所有者である場合に、 **Adddelegate**操作で発生します。  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |このエラーは、 **Getdelegate**操作で、ローカルの FreeBusy メッセージに代理人情報が存在しない場合、または Active Directory のパブリック委任がない場合 (「public delegate」または「代理送信」エントリが AD DS にない) の場合に発生します。  <br/> |
|ErrorDelegateNoUser  <br/> |このエラーは、指定されたユーザーを AD DS 内のユーザーにマップできない場合に発生します。  <br/> |
|ErrorDelegateValidationFailed  <br/> |このエラーは、追加された代理人ユーザーが有効でない場合に、 **adddelegate**操作で発生します。  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |このエラーは、識別フォルダーの削除が試行されたときに発生します。  <br/> |
|ErrorDeleteItemsFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |このエラーは、操作に対して識別ユーザー ID が有効ではないことを示します。 **DistinguishedUserType**は、要求に含まれていてはなりません。  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |このエラーは、要求配布リストのメンバーが配布リストに存在しないことを示します。  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |このエラーは、 **CreateManagedFolder**操作要求の[foldernames](foldernames.md)要素内で重複するフォルダー名が指定されている場合に発生します。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |このエラーは、SOAP ヘッダーが重複していることを示しています。  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |このエラーは、アクセス許可セットに重複するユーザー ID が見つかったことを示します。既定または匿名は複数回設定されているか、Sid または受信者が重複しています。  <br/> |
|ErrorEmailAddressMismatch  <br/> |このエラーは、要求が検索フォルダーの検索パラメーターを作成または更新しようとしたときに発生します。 たとえば、検索フォルダーがメールボックス内に作成されていても、検索フォルダーが別のメールボックスを参照するように指示されている場合に、この現象が発生することがあります。  <br/> |
|ErrorEventNotFound  <br/> |このエラーは、ウォーターマークに関連付けられたイベントが返される前に削除されると発生します。 このエラーが返されると、サブスクリプションも削除されます。  <br/> |
|ErrorExceededConnectionCount  <br/> |このエラーは、サーバーに対する同時要求の数が、ユーザーのポリシーで許可されている数を超えていることを示します。  <br/> |
|ErrorExceededSubscriptionCount  <br/> |このエラーは、ユーザーの調整ポリシーの最大サブスクリプション数を超えたことを示します。  <br/> |
|ErrorExceededFindCountLimit  <br/> |このエラーは、検索操作の呼び出しが、返される可能性のあるアイテムの合計数を超えたことを示します。  <br/> |
|ErrorExpiredSubscription  <br/> |このエラーは、サブスクリプションの有効期限が切れているために削除されているため、 [GetEvents 操作](getevents-operation.md)が呼び出された場合に発生します。  <br/> |
|ErrorExtensionNotFound  <br/> |拡張機能が見つからなかったことを示します。  <br/> |
|ErrorFolderCorrupt  <br/> |このエラーは、フォルダーが破損していて、保存できない場合に発生します。  <br/> |
|ErrorFolderExists  <br/> |このエラーは、同じ親の別のフォルダーと同じ名前を持つフォルダーを作成しようとした場合に発生します。 フォルダー名を複製することはできません。  <br/> |
|ErrorFolderNotFound  <br/> |このエラーは、指定されたフォルダー ID が有効なフォルダーに対応していないこと、または代理人がフォルダーへのアクセス許可を持っていないことを示します。  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |このエラーは、要求されたプロパティを取得できなかったことを示します。 これは、プロパティが存在しないことを示しますが、取得に失敗したことを示す何らかの方法でプロパティが破損しています。  <br/> |
|ErrorFolderSave  <br/> |このエラーは、無効な状態のためにフォルダーを作成または更新できなかったことを示します。  <br/> |
|ErrorFolderSaveFailed  <br/> |このエラーは、無効な状態のためにフォルダーを作成または更新できなかったことを示します。  <br/> |
|ErrorFolderSavePropertyError  <br/> |このエラーは、無効なプロパティ値のためにフォルダーを作成または更新できなかったことを示します。 応答コードには、問題の原因となったプロパティが表示されます。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |このエラーは、配布リストの空き時間情報を取得するために、グループメンバーの最大数に達したことを示します。  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |このエラーは、余分なエラーのために空き時間情報を取得できない場合に返されます。  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorImContactLimitReached 達しました  <br/> |このエラーは、連絡先の最大数に達したために新しいインスタントメッセージング (IM) の連絡先を追加できない場合に返されます。 このエラーは、Exchange Server 2013 で導入されました。  <br/> |
|Errorimgroupdisplaynameexists が既に存在します  <br/> |このエラーは、既存のグループの表示名が既に同じ場合に、グループの表示名を追加しようとすると返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorImGroupLimitReached  <br/> |このエラーは、グループの最大数に達したために新しい IM グループを追加できない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorImpersonateUserDenied  <br/> |このエラーは、呼び出し元が問題の特定のユーザーを偽装するための適切な権限を持っていない場合に、Exchange 偽装のサーバー間認証のケースで返されます。 このエラーは、Exch-EPI-Impersonate 拡張 Active Directory 権限にマッピングされます。  <br/> |
|ErrorImpersonationDenied  <br/> |このエラーは、発信者が要求を行っているクライアントアクセスサーバーを介して偽装する適切な権限を持っていない場合に、Exchange 偽装のサーバー間認証で返されます。 これは、Exch-EPI の拡張された Active Directory 権限にマップされます。  <br/> |
|ErrorImpersonationFailed  <br/> |このエラーは、サーバー間認証を実行しようとしたときに予期しないエラーが発生したことを示します。 この応答コードは、通常、Exchange Web サービスアプリケーションプールを実行しているサービスアカウントが正しく構成されていないか、Exchange Web サービスがディレクトリと通信できないか、フォレスト間の信頼が正しく構成されていないことを示します。  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |このエラーは、現在の Exchange Server バージョンでは要求が有効であったが、指定された要求サーバーのバージョンでは無効であったことを示します。  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |このエラーは、 [Updateitem](updateitem.md)要素または[updateitem](updatefolder.md)要素の各変更の説明に、更新するプロパティを1つだけ表示する必要があることを示します。  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |このエラーは、要求に含まれている出席者が多すぎて解決できない場合に発生します。 既定では、解決する参加者の最大数は100です。  <br/> |
|ErrorInsufficientResources  <br/> |このエラーは、メールボックスサーバーが過負荷になっている場合に発生します。 後で要求を再試行してください。  <br/> |
|ErrorInternalServerError  <br/> |このエラーは、Exchange Web サービスで回復できないエラーが発生し、発生したエラーに関連付けられたより具体的な応答コードが存在しないことを示しています。  <br/> |
|ErrorInternalServerTransientError  <br/> |このエラーは、内部サーバーエラーが発生し、後で要求を再試行する必要があることを示しています。  <br/> |
|ErrorInvalidAccessLevel  <br/> |このエラーは、呼び出し元が空き時間情報データに対して持っているアクセスレベルが無効であることを示します。  <br/> |
|ErrorInvalidArgument  <br/> |このエラーは、 [Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)に渡されたすべての無効な引数が原因でエラーが発生したことを示します。<br/><br/> このエラーは、次のシナリオで返されます。 <br/><br/>-_送信者_パラメーターで指定されたユーザーがディレクトリに存在しません。 <br/>-_送信者_パラメーターで指定されたユーザーがディレクトリ内で一意ではありません。 <br/>-_送信者_アドレスが空である。<br/>-_送信者_アドレスは、有効な電子メールアドレスではありません。  <br/> |
|ErrorInvalidAttachmentId  <br/> |このエラーは、指定された ID に対応する添付ファイルが見つからない場合に、 [Getattachment 操作](getattachment-operation.md)または[deleteattachment 操作](deleteattachment-operation.md)によって返されます。  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |このエラーは、複雑な添付ファイルテーブル制限を使用して既存の検索フォルダーにバインドしようとした場合に発生します。 Exchange Web サービスは、添付ファイルテーブルに対して単純なフィルターをサポートします。 より複雑な添付ファイルテーブルの制限 (サブフィルター) を持つ既存の検索フォルダーにバインドしようとすると、Exchange Web サービスはそのフィルターの XML をレンダリングできないため、この応答コードを返します。 <br/><br/>なお、フォルダーに対して GetFolder 操作を呼び出すことはできますが、 [Searchparameters](searchparameters.md)要素は要求しません。  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |このエラーは、複雑な添付ファイルテーブル制限を使用して既存の検索フォルダーにバインドしようとした場合に発生します。 Exchange Web サービスは、添付ファイルテーブルに対して単純なフィルターをサポートします。 <br/><br/>より複雑な添付ファイルテーブルの制限がある既存の検索フォルダーにバインドしようとすると、Exchange Web サービスはそのフィルターの XML を表示できません。 この例では、添付ファイルのサブフィルターにテキストフィルターが含まれていますが、添付ファイルの表示名を参照していません。<br/><br/> なお、フォルダーに対して GetFolder 操作を呼び出すことはできますが、 [Searchparameters](searchparameters.md)要素は要求しません。  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | このエラーは、リクエスターの承認手順が失敗したことを示します。  <br/> |
|ErrorInvalidChangeKey  <br/> |このエラーは、コンシューマーが、解析できない変更キーを持つフォルダーまたはアイテムの識別子を渡したときに発生します。 たとえば、無効な base64 コンテンツまたは空の文字列になることがあります。  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |このエラーは、発信者の id を解決しようとしたときに内部エラーが発生したことを示します。  <br/> |
|ErrorInvalidCompleteDate  <br/> |このエラーは、タスクの[Completedate](completedate.md)要素の値を将来の時刻に設定しようとした場合に返されます。 クライアントアクセスサーバーのローカル時刻に変換された場合、タスクの[Completedate](completedate.md)は、クライアントアクセスサーバー上のローカル時刻よりも後の値に設定することはできません。  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |このエラーは、連絡先に対して無効な電子メールアドレスが提供されたことを示します。  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |このエラーは、電子メールエントリに対して無効な電子メールのインデックス値が指定されたことを示します。  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |このエラーは、別のディレクトリサービスフォレストへの要求をプロキシするために使用される資格情報が認証に失敗した場合に発生します。  <br/> |
|ErrorInvalidDelegatePermission  <br/> |このエラーは、指定されたフォルダーのアクセス許可が無効であることを示します。  <br/> |
|ErrorInvalidDelegateUserId  <br/> |このエラーは、指定された委任ユーザー ID が無効であることを示します。  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |このエラーは、発信者が UPN、電子メールアドレス、またはユーザー SID を指定しない場合に Exchange の偽装時に発生します。 これは、呼び出し元が1つ以上の値を指定し、それらの値が空の場合にも発生します。  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |このエラーは、[除外](excludes.md)要素の制限に渡されたビットマスクを解析できない場合に発生します。  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidExtendedProperty  <br/> | このエラーは、次のイベントが発生したときに発生します。 <br/> <br/>-発信者が、Exchange Web サービスでサポートされていない拡張プロパティを使用しようとしています。  <br/>-呼び出し元は、拡張プロパティの属性値の無効な組み合わせを渡します。 これは、属性が渡されていない場合にも発生します。 特定の組み合わせのみが許可されます。  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |このエラーは、拡張プロパティの value セクションがプロパティの種類と一致しない場合に発生します。 <br/><br/>たとえば、Recordtype = "String" を持つ拡張プロパティを整数の配列に設定すると、このエラーが発生します。 このエラーは、拡張プロパティに指定された型に対して強制できない任意の文字列表記によって発生します。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |このエラーは、共有への招待の送信者が共有の招待のメタデータを作成しなかったことを示します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |このエラーは、共有メッセージが発信者に対して意図されていないことを示します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |このエラーは、要求者の組織のフェデレーションオブジェクトが正しく構成されていないことを示します。  <br/> |
|ErrorInvalidFolderId  <br/> |このエラーは、フォルダー ID が破損している場合に発生します。  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |このエラーは、指定されたフォルダーの種類が現在の操作に対して無効であることを示します。 たとえば、パブリックフォルダーに検索フォルダーを作成することはできません。  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | このエラーは、ユーザーが次のいずれかを指定した場合に、小数ページングで発生します。 <br/> <br/>-分母より大きい分子  <br/>-負の数 (ゼロより小さい)  <br/>-0 以下の分母です。  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |このエラーは、 [DataType](datatype.md)要素と ShareFolderId 要素の両方が要求内に存在することを示します。  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |このエラーは、 [Getuseravailability 操作](getuseravailability-operation.md)が[FreeBusyViewType](freebusyviewtype.md)のない状態で呼び出されたときに発生します。  <br/> |
|ErrorInvalidId  <br/> |このエラーは、ID または変更キーの形式が正しくないことを示します。  <br/> |
|ErrorInvalidIdEmpty  <br/> |このエラーは、呼び出し元が空の**Id**属性を指定した場合に発生します。  <br/> |
|ErrorInvalidLikeRequest  <br/> |このエラーは、アイテムが賛同できない場合に発生します。 ビルド番号15.00.0913.09 以降のバージョンの Exchange には、この値が含まれています。  <br/> |
|ErrorInvalidIdMalformed  <br/> |このエラーは、呼び出し元が誤った形式の**Id**属性を指定した場合に発生します。  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |このエラーは、exchange 2007 形式を使用しているフォルダーまたはアイテム ID が、Exchange 2007 SP1 以降のバージョンの要求に対して指定されたことを示しています。 Exchange 2007 の ID を Exchange 2007 SP1 以降の要求で使用することはできません。 最初に変換するには、[変換[tid 操作](convertid-operation.md)を使用する必要があります。  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |このエラーは、呼び出し元が長すぎる**Id**属性を指定した場合に発生します。  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |このエラーは、アイテムの添付ファイル ID 以外の ID が、添付ファイル ID を必要とする Web サービスメソッドに渡されるたびに返されます。  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |このエラーは、メールボックス内の連絡先が破損している場合に発生します。  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |このエラーは、呼び出し元が長すぎる**Id**属性を指定した場合に発生します。  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |このエラーは、アイテムの添付ファイル階層が、最大で255レベルの深さを超えた場合に返されます。  <br/> |
|ErrorInvalidIdXml  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidImContactId  <br/> |このエラーは、指定された IM 連絡先識別子が有効な識別子を表していない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |このエラーは、指定された IM 配布グループ SMTP アドレス識別子が有効な識別子を表していない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidImGroupId  <br/> |このエラーは、指定された IM グループ識別子が有効な識別子を表していない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |このエラーは、インデックス付きページングのオフセットが負の場合に発生します。  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |アイテムが**アーカイブアイテム**の操作に対して無効であったことを示します。  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |このエラーは、会議出席依頼または予定表アイテム以外のアイテムの種類に対して AcceptItem response オブジェクトを使用しようとした場合、または [削除済みアイテム] フォルダーにある予定表アイテムの発生を承諾しようとした場合に発生します。  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |このエラーは、予定表アイテム以外のアイテムの種類で CancelItem response オブジェクトを使用しようとした場合に発生します。  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | このエラーは、サポートされていない種類のアイテムの添付ファイルを作成しようとした場合に返されます。  <br/><br/>  アイテムの添付ファイルに対してサポートされるアイテムの種類には、次のオブジェクトが含まれます。  <br/><br/>- [部分](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [仕事](task.md) <br/>- [情報](contact.md) <br/> <br/> たとえば、[会議メッセージ](meetingmessage.md)の添付ファイルを作成しようとすると、この応答コードが発生します。  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | このエラーは、要求にサポートされていないアイテムの種類が含まれている場合に、 [CreateItem 操作](createitem-operation.md)から返されます。 <br/><br/>サポートされているアイテムには、次のオブジェクトがあります。<br/>  <br/>- [部分](item.md) <br/>- [メッセージ](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [仕事](task.md) <br/>- [情報](contact.md) <br/><br/>  特定の種類は、他の操作を行った場合と同じように作成されます。 会議メッセージは、たとえば、予定表アイテムを出席者に送信するときに作成されます。これらは明示的には作成されません。  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |このエラーは、会議出席依頼または予定表アイテム以外のアイテムの種類に対して DeclineItem response オブジェクトを使用しようとした場合、または [削除済みアイテム] フォルダーにある予定表アイテムの発生を辞退しようとした場合に発生します。  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |このエラーは、 [Expanddl 操作](expanddl-operation.md)がプライベート配布リストに対してのみ有効であることを示します。  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |このエラーは、要求が会議の取り消しアイテム以外のアイテムを指定した場合に、RemoveItem response オブジェクトから返されます。  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |このエラーは、要求がメッセージアイテム以外のアイテムを指定した場合に、 [SendItem 操作](senditem-operation.md)から返されます。  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |このエラーは、会議出席依頼または予定表アイテム以外のアイテムの種類に対して[TentativelyAcceptItem](tentativelyacceptitem.md)を使用しようとした場合、または [削除済みアイテム] フォルダーにある予定表アイテムの発生を仮承諾しようとした場合に発生します。  <br/> |
|ErrorInvalidLogonType  <br/> |このエラーは、内部使用のみを対象としています。 このエラーは返されません。  <br/> |
|ErrorInvalidMailbox  <br/> |このエラーは、個人用配布リストの作成または更新中に[CreateItem 操作](createitem-operation.md)または[updateitem 操作](updateitem-operation.md)が失敗したことを示します。  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |このエラーは、管理フォルダーの構造が破損していて、表示できない場合に発生します。  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |このエラーは、管理フォルダーに設定されているクォータが0より小さい場合に発生します。これは、管理フォルダーが破損していることを示します。  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |このエラーは、管理フォルダーに設定されているサイズが0より小さい場合に発生します。これは、管理フォルダーが破損していることを示します。  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |このエラーは、提供されたマージされた空き時間情報の内部値が無効な場合に発生します。 既定の最小値は5分です。 既定の最大値は1440分です。  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |このエラーは、 [ResolveNames 操作](resolvenames-operation.md)の名前が無効な場合に発生します。 たとえば、長さ0の文字列、1つのスペース、コンマ、およびダッシュは、すべて無効な名前です。  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |このエラーは、クライアントアクセスサーバー上のネットワークサービスアカウントでエラーが発生したことを示します。  <br/> |
|ErrorInvalidOofParameter  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidOperation  <br/> | これは、要求された操作が無効な場合に使用される一般的なエラーです。 <br/><br/>たとえば、次の操作を行うことはできません。 <br/> <br/>-パブリックフォルダーで[Findfolder 操作](findfolder-operation.md)を使用して、"ディープ" 走査を実行します。  <br/>-パブリックフォルダーのルートを移動またはコピーします。  <br/>-"Hard" 削除以外のモードを使用して、関連付けられたアイテムを削除します。  <br/>-関連付けられたアイテムを移動またはコピーします。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |このエラーは、発信者が別の組織のユーザーの空き時間情報を要求したが、組織上の関係の空き時間情報が有効になっていないことを示します。  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |このエラーは、コンシューマーが返される最大行数に0または負の値が渡されると発生します。  <br/> |
|ErrorInvalidParentFolder  <br/> |このエラーは、コンシューマーが操作の無効な親フォルダーを渡したときに発生します。 たとえば、検索フォルダー内にフォルダーを作成しようとすると、このエラーが返されます。  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |このエラーは、タスク完了率を無効な値に設定しようとした場合に返されます。 値は 0 ~ 100 (包含) である必要があります。  <br/> |
|ErrorInvalidPermissionSettings  <br/> |このエラーは、アクセス許可レベルがアクセス許可の設定と一致しないことを示します。  <br/> |
|ErrorInvalidPhoneCallId  <br/> |このエラーは、呼び出し元の識別子が無効であることを示します。  <br/> |
|ErrorInvalidPhoneNumber  <br/> |このエラーは、電話番号が正しくないか、ダイヤルプランのルールに該当しないことを示します。  <br/> |
|ErrorInvalidPropertyAppend  <br/> | このエラーは、追加しようとしているプロパティが追加をサポートしていない場合に発生します。 <br/><br/>以下に、追加をサポートする唯一のプロパティを示します。 <br/> <br/>-Recipient コレクション (トーラスの場合)、CcRecipients 場合、BccRecipients 場合  <br/>-出席者コレクション (Requiredatん Dees、[任意出席者]、[リソース])  <br/>-本文  <br/>-ReplyTo  <br/><br/>  また、要求で指定された形式がストア内のアイテムの形式と一致しない場合に、メッセージ本文が追加されると、このエラーが発生します。  <br/> |
|ErrorInvalidPropertyDelete  <br/> |このエラーは、削除操作がサポートされていないプロパティに対する[Updateitem 操作](updateitem-operation.md)または[updateitem 操作](updatefolder-operation.md)呼び出しで delete 操作が指定された場合に発生します。 たとえば、[アイテム](item.md)オブジェクトの[ItemId](itemid.md)要素を削除することはできません。  <br/> |
|ErrorInvalidPropertyForExists  <br/> |このエラーは、consumer が、 [Exists](exists.md)フィルターのフラグプロパティのいずれかを渡した場合に発生します。 たとえば、 [Exists](exists.md)要素で[Isread](isread.md)または[isfromme](isfromme.md)フラグが指定されている場合に、このエラーが発生します。 この要求は、フラグとして、1つのプロパティの一部であるため、 [IsEqualTo](isequalto.md)要素を代わりに使用する必要があります。  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |このエラーは、操作しようとしているプロパティが、実行中の操作をサポートしていない場合に発生します。  <br/> |
|ErrorInvalidPropertyRequest  <br/> | このエラーは、要求で指定されているプロパティがアイテムの種類に対して使用できない場合に発生します。 たとえば、予定表アイテムでのみ使用可能なプロパティが、メッセージの[GetItem 操作](getitem-operation.md)呼び出しで要求された場合、またはメッセージの[updateitem 操作](updateitem-operation.md)呼び出しで更新された場合に、このエラーが返されます。 <br/> <br/>  これは、次の操作で発生します。 <br/> <br/>- [GetItem 操作](getitem-operation.md) <br/>- [GetFolder 操作](getfolder-operation.md) <br/>- [UpdateItem 操作](updateitem-operation.md) <br/>- [UpdateFolder 操作](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |このエラーは、操作しようとしているプロパティが、実行中の操作をサポートしていないことを示しています。 たとえば、設定しようとしているプロパティが読み取り専用である場合に、このエラーが返されます。  <br/> |
|Errorinvalidpropertyの更新 Entmessage  <br/> | このエラーは、クライアントが既に送信されているメッセージの特定のプロパティを更新しようとしたときに、 [Updateitem 操作](updateitem-operation.md)中に発生します。<br/><br/> たとえば、送信されたメッセージに対して次のプロパティを更新することはできません。 <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |このエラーは、プッシュサブスクリプション ID を使用して[GetEvents 操作](getevents-operation.md)または登録[解除操作](unsubscribe-operation.md)を呼び出した場合に発生します。 プッシュサブスクリプションの登録を解除するには、サブスクライブ解除応答を使用してプッシュ要求に応答するか、Web サービスを切断して、プッシュ通知がタイムアウトするまで待機する必要があります。  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | このエラーは、 [Subscribe 操作](subscribe-operation.md)で "プッシュ" サブスクリプションが作成されたときに返され、要求に含まれる URL が無効であることを示します。<br/><br/>Exchange Web サービスが URL を受け入れるには、次の条件を満たす必要があります。 <br/> <br/>-文字列の長さ \> 0 および \< 2083.  <br/> -Protocol は http または https です。  <br/>-URL は、URI Microsoft .NET Framework クラスで解析できます。  <br/> |
|ErrorInvalidRecipients  <br/> |このエラーは、メッセージの受信者コレクションまたは予定表アイテムの出席者コレクションが無効であることを示します。 たとえば、受信者がいないアイテムを送信しようとすると、このエラーが返されます。  <br/> |
|Errorinvalid受信者サブフィルター  <br/> |このエラーは、Exchange Web サービスが表すことができない受信者テーブルフィルターが検索フォルダーにあることを示しています。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|Errorinvalid受信者 Subfiltercomparison  <br/> |このエラーは、Exchange Web サービスが表すことができない受信者テーブルフィルターが検索フォルダーにあることを示しています。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|Errorinvalid受信者サブ Filterorder  <br/> |このエラーは、Exchange Web サービスが表すことができない受信者テーブルフィルターが検索フォルダーにあることを示しています。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|Errorinvalid受信者 Subfiltertextfilter  <br/> |このエラーは、Exchange Web サービスが表すことができない受信者テーブルフィルターが検索フォルダーにあることを示しています。 このエラーを回避するには、検索パラメーターを要求せずにフォルダーを取得します。  <br/> |
|ErrorInvalidReferenceItem  <br/> | このエラーは、次のシナリオでは、転送および返信の応答オブジェクトの[CreateItem 操作](createitem-operation.md)から返されます。<br/>  <br/>-参照されているアイテムの識別子が、[メッセージ](message-ex15websvcsotherref.md)、予定表[アイテム](calendaritem.md)、または**メッセージ**または予定表**アイテム**の子ではありません。  <br/>-参照アイテム識別子が**calendaritem**用であり、開催者が自分に返信または ReplyAll をしようとしています。  <br/>-メッセージは下書きで、返信または ReplyAll が選択されています。  <br/>- [SuppressReadReceipt](suppressreadreceipt.md)の参照項目は、**メッセージ**でも、**メッセージ**の子孫でもありません。  <br/> |
|ErrorInvalidRequest  <br/> |このエラーは、soap 要求に soap アクションヘッダーがあり、SOAP 本文には何もない場合に発生します。 Soap アクションヘッダーは、SOAP 本文のルート要素のローカル名から呼び出す方法を Exchange Web サービスが決定するため、必要ではないことに注意してください。  <br/> |
|ErrorInvalidRestriction  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |このエラーは、指定した保持タグに、正しくないアクションが関連付けられている場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |このエラーは、 **policytag**プロパティに存在しないタグまたは不可視タグを設定しようとした場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |このエラーは、 **policytag**プロパティに暗黙的なタグを設定しようとした場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |保持タグ GUID が無効であったことを示します。  <br/> |
|ErrorInvalidRoutingType  <br/> |このエラーは、 [routingtype (EmailAddressType)](routingtype-emailaddresstype.md)要素に渡されるルーティングの種類が無効な場合に発生します。 通常、ルーティングの種類は、簡易メール転送プロトコル (SMTP) に設定されます。  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |このエラーは、指定された期間の終了時刻が開始時刻よりも前になっていない場合、または終了時刻が今後発生しない場合に発生します。  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |このエラーは、別のサーバーに送信されたプロキシ要求が、バージョン管理が一致しないため、要求を処理できないことを示します。  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |このエラーは、ストア内の予定表フォルダーの Exchange セキュリティ記述子が破損していることを示しています。  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |このエラーは、 [SavedItemFolderId](saveditemfolderid.md)が要求で指定されているアイテムを送信しようとしたときに、 **Saveitemtofolder**プロパティが**false**に設定されている場合に発生します。  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |このエラーは、ヘッダーに渡されたトークンの形式が正しくないか、ディレクトリ内の有効なアカウントを参照していないか、またはプライマリグループの**ConnectingSID**が存在しないことを示します。  <br/> |
|ErrorInvalidSharingData  <br/> |このエラーは、共有メタデータが無効であることを示します。 これは、無効な XML によって発生する可能性があります。  <br/> |
|ErrorInvalidSharingMessage  <br/> |このエラーは、共有メッセージが無効であることを示します。 この問題は、プロパティがないことが原因で発生する場合があります。  <br/> |
|ErrorInvalidSid  <br/> |このエラーは、無効な SID が要求に渡されると発生します。  <br/> |
|エラー Invalidsi紫 i  <br/> |このエラーは、SIP 名、ダイヤルプラン、または電話番号が無効な SIP Uri であることを示します。  <br/> |
|ErrorInvalidServerVersion  <br/> |このエラーは、要求に無効な要求サーバーのバージョンが指定されたことを示します。  <br/> |
|ErrorInvalidSmtpAddress  <br/> |このエラーは、SMTP アドレスを解析できない場合に発生します。  <br/> |
|ErrorInvalidSubfilterType  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |この応答コードは使用されません。  <br/> |
|Errorinvalidsubfiltertypenot受信者の種類  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidSubscription  <br/> |このエラーは、サブスクリプションが有効でなくなったことを示します。 これは、クライアントアクセスサーバーが再起動しているか、サブスクリプションの有効期限が切れているために考えられます。  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |このエラーは、subscribe 要求に複数のパブリックフォルダー Id が含まれていることを示します。 サブスクリプションには、同じメールボックスまたは1つのパブリックフォルダー ID からの複数のフォルダーを含めることができます。  <br/> |
|ErrorInvalidSyncStateData  <br/> |このエラーは、渡された[Syncstate](syncstate-ex15websvcsotherref.md)データが無効な場合に、 [syncfolderitems](syncfolderitems.md)または[syncfolderitems](syncfolderhierarchy.md)によって返されます。 このエラーを修正するには、同期状態を使用せずに再同期する必要があります。 同期状態 Blob を永続化している場合は、誤って BLOB を切り捨てていないことを確認してください。  <br/> |
|ErrorInvalidTimeInterval  <br/> |このエラーは、指定された時間間隔が無効であることを示します。 開始時刻は、終了時刻以上である必要があります。  <br/> |
|ErrorInvalidUserInfo  <br/> |このエラーは、アクセス許可操作に対して内部的に不整合な[UserId](userid.md)が指定されたことを示します。 たとえば、識別ユーザー ID が指定されている (既定または匿名) 場合、このユーザーの SID またはプライマリ SMTP アドレスまたは表示名も指定しようとすると、このエラーが返されます。  <br/> |
|ErrorInvalidUserOofSettings  <br/> |このエラーは、内部または外部の返信がないために、ユーザーの不在時 (OOF) 設定が無効であることを示します。  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |このエラーは、Exchange の偽装時に発生します。 発信者が、ディレクトリ内でアクセスできない無効な UPN を SOAP ヘッダーに渡しました。  <br/> |
|エラー Invalidusersid  <br/> |このエラーは、無効な SID が要求に渡されると発生します。  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |この応答コードは使用されません。  <br/> |
|ErrorInvalidValueForProperty  <br/> |このエラーは、制限の比較値が、比較対象のプロパティに対して無効であることを示します。<br/><br/> たとえば、 [DateTimeCreated](datetimecreated.md)true の比較値を指定する  >  **true**と、この応答コードが返されます。 <br/><br/>この応答コードは、比較で列挙プロパティを指定した場合にも返されますが、比較する値がその列挙の有効な値ではありません。  <br/> |
|ErrorInvalidWatermark  <br/> |このエラーは、無効なウォーターマークが原因で発生します。  <br/> |
|ErrorIPGatewayNotFound  <br/> |このエラーは、有効な VoIP ゲートウェイが使用できないことを示します。  <br/> |
|ErrorIrresolvableConflict  <br/> |このエラーは、競合の解決によってプロパティの変更を解決できなかったことを示します。 ストア内のアイテムが変更されており、更新する必要がある可能性があります。 更新した変更キーを取得して、もう一度実行してください。  <br/> |
|ErrorItemCorrupt  <br/> |このエラーは、オブジェクトの状態が破損していて、取得できないことを示します。 アイテムを取得するとき、 [Body](body.md) 、 [MimeContent](mimecontent.md)など、特定の要素のみがこの状態になります。 これらの要素を省略して、操作を再試行してください。  <br/> |
|ErrorItemNotFound  <br/> |このエラーは、アイテムが見つからないか、アイテムにアクセスする権限がない場合に発生します。  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |このエラーは、アイテムのプロパティ要求が失敗した場合に発生します。 プロパティが存在する場合がありますが、取得できませんでした。  <br/> |
|ErrorItemSave  <br/> |このエラーは、アイテムまたはフォルダーを保存しようとして失敗した場合に発生します。  <br/> |
|ErrorItemSavePropertyError  <br/> |このエラーは、プロパティの値が無効なため、アイテムまたはフォルダーを保存しようとして失敗した場合に発生します。 応答コードには、無効なプロパティのパスが含まれています。  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |この応答コードは使用されません。  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |このエラーは、可用性サービスが、適切なサイトまたはフォレストへの要求をプロキシするために、ネットワークサービスとしてログオンできなかったことを示しています。 通常、この応答は構成エラーを示します。  <br/> |
|ErrorMailboxConfiguration  <br/> |このエラーは、AD DS のメールボックス情報が正しく構成されていないことを示します。  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |このエラーは、要求の[MailboxDataArray](mailboxdataarray.md)要素が空であることを示します。 少なくとも1つのメールボックス識別子を指定する必要があります。  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |このエラーは、 [MailboxDataArray](mailboxdataarray.md)要素で100個を超えるエントリが指定されている場合に発生します。.  <br/> |
|ErrorMailboxFailover  <br/> |このエラーは、メールボックスがフェールオーバープロセスにあるために、メールボックスにアクセスしようとして失敗したことを示します。  <br/> |
|ErrorMailboxHoldNotFound  <br/> |メールボックスの保持が見つからなかったことを示します。  <br/> |
|ErrorMailboxLogonFailed  <br/> |このエラーは、予定表ビュー情報を取得するためのメールボックスへの接続が失敗したときに発生します。  <br/> |
|ErrorMailboxMoveInProgress  <br/> | このエラーは、メールボックスが別のメールボックスストアまたはサーバーに移動されていることを示します。 このエラーは、メールボックスが別のサーバーまたはメールボックスデータベース上にあることを示している可能性もあります。  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | このエラーは、次のいずれかのエラー状態が発生したことを示します。  <br/><br/>-メールボックスストアが破損しています。  <br/>-メールボックスストアが停止されています。  <br/>-メールボックスストアがオフラインになっている。  <br/>-メールボックスストアへのアクセスが試みられたときに、ネットワークエラーが発生しました。  <br/>-メールボックスストアは過負荷になっており、それ以上の接続を受け付けることはできません。  <br/>-メールボックスストアが一時停止されています。  <br/> |
|ErrorMailRecipientNotFound  <br/> |このエラーは、 [MailboxData](mailboxdata.md)要素の情報を有効なメールボックスアカウントにマップできない場合に発生します。  <br/> |
|Errormailヒントが無効  <br/> |このエラーは、メールヒントが無効になっていることを示します。  <br/> |
|Errormanagedfolderは既に存在します  <br/> |このエラーは、作成しようとしている管理フォルダーがメールボックス内に既に存在する場合に発生します。  <br/> |
|ErrorManagedFolderNotFound  <br/> |このエラーは、要求で指定されたフォルダー名が AD DS 内の管理フォルダー定義にマップされていない場合に発生します。 管理フォルダーのインスタンスは、AD DS で定義されたフォルダーに対してのみ作成できます。 名前を確認して、もう一度実行してください。  <br/> |
|Errormanagedフォルダー Rootfailure  <br/> |このエラーは、管理フォルダーのルートがメールボックスから削除されたこと、または管理フォルダーのルートの名前を持つ同じ親フォルダーに存在するフォルダーであることを示しています。 このエラーは、ルート管理フォルダーを作成しようとして失敗した場合にも発生します。  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |このエラーは、提案を作成しようとしたときに、提案エンジンで問題が発生したことを示します。  <br/> |
|ErrorMessageDispositionRequired  <br/> | このエラーは、 **MessageDisposition**属性が設定されていない場合に発生します。<br/><br/> この属性は、次の場合に必要です。 <br/> <br/>-作成または更新されているアイテムが[メッセージ](message-ex15websvcsotherref.md)である場合の[CreateItem 操作](createitem-operation.md)と[updateitem 操作](updateitem-operation.md)。  <br/>- [Cancelcalendaritem](cancelcalendaritem.md)、 [acceptitem](acceptitem.md)、 [Declineitem](declineitem.md)、または[TentativelyAcceptItem](tentativelyacceptitem.md) response オブジェクト。  <br/> |
|Errorメッセージ Izeを超過しました  <br/> |このエラーは、送信しようとしているメッセージが許可されている制限を超えていることを示します。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |このエラーは、指定されたドメインが見つからないことを示します。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |このエラーは、メッセージ追跡サービスがメッセージを追跡できないことを示します。  <br/> |
| ErrorMessageTrackingTransientError  <br/> |このエラーは、メッセージ追跡サービスが停止しているかビジー状態であることを示します。 このエラーコードは、一時的なエラーを示します。 このエラーを受け取ったときに、クライアントはサーバーへの接続を再試行できます。  <br/> |
|ErrorMimeContentConversionFailed  <br/> |このエラーは、MIME コンテンツが[CreateItem 操作](createitem-operation.md)に対して有効な iCal ではない場合に発生します。 [GetItem 操作](getitem-operation.md)の場合、この応答は MIME コンテンツを生成できなかったことを示します。  <br/> |
|ErrorMimeContentInvalid  <br/> |このエラーは、MIME の内容が無効な場合に発生します。  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |このエラーは、要求内の MIME コンテンツが有効なベース64文字列ではない場合に発生します。  <br/> |
|ErrorMissingArgument  <br/> |このエラーは、要求に必要な引数が欠落していたことを示します。 応答メッセージのテキストは、確認する引数を示します。  <br/> |
|ErrorMissingEmailAddress  <br/> |このエラーは、要求で識別フォルダー ID が指定されたが、要求を行ったアカウントにシステム上にメールボックスが存在しないことを示しています。 その場合は、 [DistinguishedFolderId](distinguishedfolderid.md)の下に[メールボックス](mailbox.md)サブ要素を指定する必要があります。  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |このエラーは、要求で識別フォルダー ID が指定されたが、要求を行ったアカウントにシステム上にメールボックスが存在しないことを示しています。 その場合は、 [DistinguishedFolderId](distinguishedfolderid.md)の下に[メールボックス](mailbox.md)サブ要素を指定する必要があります。 この応答は、 [CreateManagedFolder 操作](createmanagedfolder-operation.md)から返されます。  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |このエラーは、 [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素が存在しない場合に発生します。  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |このエラーは、 [Referenceitemid](referenceitemid.md)が見つからない場合に発生します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラーコードは返されません。  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |このエラーは、 [createattachment 操作](createattachment-operation.md)要求の**itemattachment**要素に item 要素を含めないようにした場合に返されます。  <br/> |
|ErrorMissingManagedFolderId  <br/> |このエラーは、フォルダーの policy IDs プロパティ (property タグ 0x6732) が存在しない場合に発生します。 破損したフォルダーがあることを考慮する必要があります。  <br/> |
|ErrorMissingRecipients  <br/> |このエラーは、受信者を含めずにアイテムを送信しようとしたことを示します。 メッセージが送信される原因となるメッセージの廃棄を使用して[CreateItem 操作](createitem-operation.md)を呼び出すと、次の応答コードが返されます。 **errorinvalidrecipients**。  <br/> |
|ErrorMissingUserIdInformation  <br/> |このエラーは、アクセス許可セットに[ユーザー id](userid.md)が完全に指定されていないことを示します。  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |このエラーは、1つの要求内で複数の[Exchangeimpersonation](exchangeimpersonation.md)要素の値が指定されたことを示します。  <br/> |
|ErrorMoveCopyFailed  <br/> |このエラーは、移動またはコピー操作が失敗したことを示します。 移動は、[削除済みアイテム] フォルダー内の会議出席依頼を承諾したときに[CreateItem 操作](createitem-operation.md)で行われます。 また、会議出席依頼を辞退したり、予定表アイテムを取り消したり、予定表から会議を削除したりすると、それが [削除済みアイテム] フォルダーに移動されます。  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |このエラーは、識別フォルダーを移動しようとした場合に発生します。  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |このエラーは、要求が複数のメールボックスサーバーにアクセスしようとした場合に発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |このエラーは、 [ResolveNames 操作](resolvenames-operation.md)で複数の結果が返された場合、または指定したあいまいな名前がディレクトリ内の複数のオブジェクトと一致する場合に発生します。 応答コードには、応答データに一致する名前が含まれています。  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |このエラーは、発信者がシステム上にメールボックスを持っていないことを示します。 [ResolveNames 操作](resolvenames-operation.md)または[expanddl 操作](expanddl-operation.md)は、メールボックスなしでユーザーを接続する場合は無効です。  <br/> |
|ErrorNameResolutionNoResults  <br/> |このエラーは、 [ResolveNames 操作](resolvenames-operation.md)で結果が返されないことを示します。  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |このエラーコードは、Web サービスが要求を処理するサーバーを見つけることができない場合に返される必要があります。  <br/> |
|エラー Nocalendar  <br/> |このエラーは、メールボックスの予定表フォルダーが存在しない場合に発生します。  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照しているにもかかわらず、宛先サイト内のクライアントアクセスサーバーが Windows 認証用に構成されていなかったため、要求をプロキシできなかったことを示します。  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |このエラーは、要求が別の Active Directory サイトのメールボックスを参照したが、宛先サイト内のクライアントアクセスサーバーが SSL 接続用に構成されておらず、要求をプロキシできなかったことを示しています。  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照していて、宛先サイト内のクライアントアクセスサーバーが、要求を受信するために許容可能な製品バージョンではなかったため、要求をプロキシできなかったことを示します。  <br/> |
|ErrorNoFolderClassOverride  <br/> |このエラーは、汎用フォルダー以外のアイテムを作成するときに、 [Folderclass](folderclass.md)要素を設定した場合に発生します。 [Calendarfolder](calendarfolder.md)や仕事[フォルダー](tasksfolder.md)などの、型指定されたフォルダーの場合は、フォルダークラスが暗黙的に使用されます。 [Updatefolder 操作](updatefolder-operation.md)を使用してフォルダークラスを別のフォルダーの種類に設定すると、 **Errorobjecttypechanged**応答が返されます。 代わりに、汎用フォルダーの種類を使用しますが、folder クラスを必要な値に設定します。 Exchange Web サービスは、厳密に型指定された適切なフォルダーを作成します。  <br/> |
|ErrorNoFreeBusyAccess  <br/> |このエラーは、該当する予定表フォルダーで、呼び出し元に空き時間情報の表示権限がないことを示します。  <br/> |
|エラー非居住 Entmailbox メールボックス  <br/> | このエラーは、次のシナリオで発生します。 <br/> <br/>-電子メールアドレスが[CreateManagedFolder](createmanagedfolder.md)で空になっています。  <br/>-電子メールアドレスは、本文または SOAP ヘッダーに電子メールアドレスを取得する、Exchange の偽装呼び出しなどの、要求で有効なアカウントを参照していません。  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |このエラーは、発信者がプライマリ以外の SMTP アドレスを渡した場合に発生します。 応答には、使用する適切な SMTP アドレスが含まれています。  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |このエラーは、ユーザー設定範囲で0x8000 以上の MAPI プロパティがプロパティタグによって参照できないことを示しています。 EWS マネージ API の[propertysetid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)プロパティまたは Ews の[ExtendedFieldURI](extendedfielduri.md)要素を propertysetid 属性と共に使用する必要があります。  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |この応答コードは使用されません。  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |このエラーコードは、パブリックフォルダーサーバーが使用できない場合、または発信者が自宅のパブリックサーバーを持っていない場合に返される必要があります。  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照したが、そのサイト内のクライアントアクセスサーバーが応答しなかったため、要求をプロキシできなかったことを示します。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |このエラーは、呼び出し元が自分の予定表または連絡先フォルダー内のアクセス許可を別の組織のユーザーに付与しようとして失敗したことを示します。  <br/> |
|ErrorNotDelegate  <br/> |このエラーは、ユーザーがメールボックスの代理人ではないことを示します。 これは、指定された代理ユーザーが代理人の一覧に見つからない場合に、 [Getdelegate](getdelegate-operation.md)操作、 [removedelegate 操作](removedelegate-operation.md)、および[updatedelegate 操作](updatedelegate-operation.md)によって返されます。  <br/> |
|ErrorNotEnoughMemory  <br/> |このエラーは、メモリが不足しているために操作を完了できなかったことを示します。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |このエラーは、共有メッセージがサポートされていないことを示します。  <br/> |
|ErrorObjectTypeChanged  <br/> |このエラーは、オブジェクトの種類が変更された場合に発生します。  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |このエラーは、発生の[開始](start.md)時刻または[終了](end-ex15websvcsotherref.md)時刻が更新され、対応する前または次の回の発生より前または後に発生するようにスケジュールされた場合に発生します。  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |このエラーは、指定されたアイテムの時間配分が、同じ定期的なアイテムの別のオカレンスと重複していることを示します。 この応答は、指定された発生の分単位の長さが Int32 より大きい場合にも発生します。  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |このエラーは、現在の操作がパブリックフォルダーのルートに対して有効ではないことを示します。  <br/> |
|Error組織 Notフェデレーション  <br/> |このエラーは、依頼者の組織がフェデレーションされていないため、依頼者は外部ユーザーに送信する共有メッセージを作成できない、または外部ユーザーから受信した共有メッセージを受信できないことを示します。  <br/> |
|ErrorParentFolderIdRequired  <br/> |この応答コードは使用されません。  <br/> |
|ErrorParentFolderNotFound  <br/> |このエラーは、親フォルダーが見つからない場合に、 [CreateFolder 操作](createfolder-operation.md)で発生します。  <br/> |
|ErrorPasswordChangeRequired  <br/> |このエラーは、このメールボックスにアクセスする前にパスワードを変更する必要があることを示しています。 これは、新しいアカウントが作成され、ユーザーが初めてログオンしたときにパスワードを変更する必要があることを管理者が指定した場合に発生します。 Exchange Web サービスを使用してパスワードを更新することはできません。 パスワードを変更するには、Microsoft Office Outlook Web App などのツールを使用する必要があります。  <br/> |
|ErrorPasswordExpired  <br/> |このエラーは、パスワードの有効期限が切れていることを示します。 Exchange Web サービスを使用してパスワードを変更することはできません。 パスワードを変更するには、Outlook Web App などのツールを使用する必要があります。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |このエラーは、リクエスターが自分の予定表または連絡先フォルダーに外部ユーザーにアクセス許可を付与しようとしたが、要求者に割り当てられている共有ポリシーが、要求されたアクセス許可レベルが共有ポリシーで許可されているものよりも高いことを示していることを示しています。  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |このエラーは、電話番号が正しい形式ではないことを示します。  <br/> |
|ErrorPropertyUpdate  <br/> |このエラーは、プロパティの値が無効なために更新が失敗したことを示します。 応答メッセージに、無効なプロパティパスが含まれています。  <br/> |
|Errorprompt発行操作が失敗しました  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorPropertyValidationFailure  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |このエラーは、別のクライアントアクセスサーバーに存在するサブスクリプションを要求が参照したが、そのクライアントアクセスサーバーへの要求をプロキシしようとしたときに失敗したことを示します。  <br/> |
|ErrorProxyCallFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorProxyGroupSidLimitExceeded を超えました  <br/> |このエラーは、要求が別の Active Directory サイト内のメールボックスを参照し、元の発信者が3000を超えるグループのメンバーであることを示します。  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |このエラーは、 [GetUserAvailabilityRequest](getuseravailabilityrequest.md)要求を実行しようとしたときに、Exchange Web サービスが別のクライアントアクセスサーバーに送信した要求が無効であったことを示します。 通常、この応答コードは、構成または権限のエラーが発生したこと、または他のユーザーが可用性プロキシ要求を模倣できなかったことを示します。  <br/> |
|ErrorProxyRequestProcessingFailed 失敗しました  <br/> |このエラーは、Exchange Web サービスが、処理のために別のクライアントアクセスサーバーに可用性要求をプロキシしようとしたが、要求に失敗したことを示します。 この応答は、ネットワーク接続の問題または要求のタイムアウトの問題によって発生する可能性があります。  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |このエラーコードは、要求がターゲットサーバーで実行されるか、別のサーバーにプロキシされるかを Web サービスが判断できない場合に返される必要があります。  <br/> |
|ErrorProxyTokenExpired 切れ  <br/> |この応答コードは使用されません。  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |このエラーは、パブリックフォルダーメールボックスの URL が見つからない場合に発生します。 このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |このエラーは、パブリックフォルダーへのアクセスが試みられ、試行に失敗した場合に発生します。 このエラーは、Exchange 2013Exchange Server 2013 で導入されました。  <br/> |
|ErrorPublicFolderRequestProcessingFailed 失敗しました  <br/> |このエラーは、 [Getuseravailability 操作](getuseravailability-operation.md)に渡された受信者が、exchange 2007 より前のバージョンの exchange Server を実行しているコンピューターに存在し、パブリックフォルダーサーバーから受信者の空き時間情報を取得する要求が失敗した場合に発生します。  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |このエラーは、 [Getuseravailability 操作](getuseravailability-operation.md)に渡された受信者が、exchange 2007 より前のバージョンの exchange Server を実行しているコンピューターに存在し、組織単位に関連付けられたパブリックフォルダーサーバーがないためにパブリックフォルダーサーバーから受信者の空き時間情報を取得する要求が失敗した場合に発生します。  <br/> |
|ErrorPublicFolderSyncException  <br/> |このエラーは、プライマリパブリックフォルダーメールボックスに対して同期操作が正常に実行されたが、セカンダリパブリックフォルダーメールボックスに対して失敗した場合に発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorQueryFilterTooLong/  <br/> |このエラーは、検索フォルダーの制限が有効であることを示しますが、EWS ではサポートされていません。 Exchange Web サービスには、最大255フィルター式を含む制限が制限されています。 255を超える既存の検索フォルダーにバインドしようとすると、この応答コードが返されます。  <br/> |
|ErrorQuotaExceeded  <br/> |このエラーは、メールボックスのクォータを超えた場合に発生します。  <br/> |
|ErrorReadEventsFailed  <br/> |このエラーは、イベント情報の取得中にエラーが発生した場合に、 [GetEvents 操作](getevents-operation.md)またはプッシュ通知で返されます。 このエラーが返されると、サブスクリプションが削除されます。 最後に認識されたウォーターマークに基づいてイベントの同期を再作成します。  <br/> |
|ErrorReadReceiptNotPending  <br/> |このエラーは、メッセージの送信者がメッセージで開封確認を要求しなかった場合、またはメッセージが [迷惑メール] フォルダーにある場合に、開封確認を抑制しようとした場合に、 [CreateItem 操作](createitem-operation.md)によって返されます。  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |このエラーは、定期的なアイテムの終了日が9/1/4500 より後の日付である場合に発生します。  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |このエラーは、指定された定期的なパターンで、指定された範囲内に出現するインスタンスが存在しない場合に発生します。  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |このエラーは、代理人が削除された後、代理人の一覧を保存できなかったことを示します。  <br/> |
|ErrorRequestAborted  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRequestStreamTooBig  <br/> | このエラーは、要求ストリームが 400 KB を超えている場合に発生します。  <br/> |
|ErrorRequiredPropertyMissing  <br/> |このエラーは、 [Createattachment 操作](createattachment-operation.md)要求で必要なプロパティが指定されていない場合に返されます。 不足しているプロパティ URI が応答に含まれています。  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |このエラーは、呼び出し元が連絡先フォルダーではないフォルダーを[ResolveNames 操作](resolvenames-operation.md)に指定したことを示します。  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |このエラーは、呼び出し元が[ResolveNames 操作](resolvenames-operation.md)に複数の連絡先フォルダーを指定したことを示します。  <br/> |
|ErrorResponseSchemaValidation  <br/> |この応答コードは使用されません。  <br/> |
|ErrorRestrictionTooLong  <br/> |このエラーは、制限に255個を超えるノードが含まれている場合に発生します。  <br/> |
|ErrorRestrictionTooComplex  <br/> |このエラーは、Exchange Web サービスによって制限を評価できない場合に発生します。  <br/> |
|ErrorResultSetTooBig  <br/> |このエラーは、指定された受信者の予定表のエントリ数が、許可された上限の1000を超えていることを示しています。 ウィンドウを小さくして、もう一度実行してください。  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |このエラーは、 [SavedItemFolderId](saveditemfolderid.md)が見つからない場合に発生します。  <br/> |
|ErrorSchemaValidation  <br/> | このエラーは、スキーマに対して要求を検証できない場合に発生します。  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |このエラーは、検索フォルダーが作成されたが、検索条件がフォルダーに設定されていないことを示します。 これは、別の API またはクライアントを使用して作成された破損した検索フォルダーにアクセスする場合にのみ発生します。 このエラーを解決するには、 [updatefolder 操作](updatefolder-operation.md)を使用して、フォルダーに存在する制限を含む[searchparameters](searchparameters.md)要素を設定します。  <br/> |
|ErrorSendAsDenied  <br/> | このエラーは、次の両方の条件に該当する場合に発生します。 <br/> <br/>-ユーザーに CanActAsOwner アクセス許可が付与されていますが、プリンシパルのメールボックスに対する代理人権限が与えられていません。  <br/>-同じユーザーが、SendAndSaveCopy オプションを使用して、プリンシパルのメールボックスで電子メールメッセージを作成し、送信しようとしています。<br/>  <br/>  この結果、ErrorSendAsDenied エラーが発生し、プリンシパルの [下書き] フォルダーに電子メールメッセージが作成されます。  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |このエラーは、要求に対して**sendDeleteItem のキャンセル**属性が欠落していて、削除するアイテムが予定表アイテムである場合に、[操作](deleteitem-operation.md)によって返されます。  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |このエラーは、 **SendMeetingInvitationsOrCancellations**属性が要求に欠けており、更新するアイテムが予定表アイテムである場合に、 [updateitem 操作](updateitem-operation.md)によって返されます。  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |このエラーは、要求に対して**sendCreateItem の招待**属性が欠落していて、作成するアイテムが予定表アイテムである場合に、[操作](createitem-operation.md)によって返されます。  <br/> |
|Errorrequest会議の更新プログラム  <br/> |このエラーは、開催者が会議出席依頼を送信した後に、要求を更新できないことを示します。 会議を変更するには、会議出席依頼ではなく、予定表アイテムを変更します。  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |このエラーは、タスクの開始者がタスクの依頼を送信した後、その要求を更新できないことを示します。  <br/> |
|ErrorServerBusy  <br/> |このエラーは、サーバーがビジー状態のときに発生します。  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |このエラーは、Exchange Web サービスが受信者のための適切なフォレストにユーザーの可用性要求をプロキシしようとしたが、サービス検出エラーのために要求を送信する場所を判断できなかったことを示します。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |このエラーは、外部 URL プロパティが Active Directory データベースで設定されていないことを示します。  <br/> |
|Errorsharing同期に失敗しました  <br/> |このエラーは、共有フォルダーを同期しようとして失敗したことを示します。 <br/><br/>このエラーコードは、次のような状況で返されます。<br/><br/>-共有フォルダーのサブスクリプションが見つかりません。<br/>-共有フォルダーが見つかりません。<br/>-対応するディレクトリユーザーが見つかりません。<br/>-ユーザーが存在しません。<br/>-予定が無効です。<br/>-連絡先アイテムが無効です。<br/>-リモートサーバーとの通信障害が発生しています。  <br/> |
|ErrorStaleObject  <br/> |このエラーは、 [Updateitem 操作](updateitem-operation.md)または[SendItem 操作](senditem-operation.md)で、変更キーが最新の状態になっていない場合、または指定されていない場合に発生します。 [GetItem 操作](getitem-operation.md)を呼び出して、更新された変更キーを取得してから、もう一度実行してください。  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |このエラーは、送信クォータに達したために、ユーザーがそれ以上の要求を送信できないことを示します。  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |このエラーは、サブスクリプションを作成していないアカウントを使用してサブスクリプションにアクセスしようとした場合に発生します。 各サブスクリプションには、サブスクリプションの作成者のみがアクセスできます。  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |このエラーは、所有者でない場合、またはメールボックスへの所有者アクセス権を持っていない場合は、サブスクリプションを作成できないことを示します。  <br/> |
|ErrorSubscriptionNotFound  <br/> |このエラーは、指定した[SubscriptionId (GetEvents)](subscriptionid-getevents.md)に対応するサブスクリプションが見つからない場合に発生します。 サブスクリプションの有効期限が切れているか、Exchange Web サービスプロセスが再起動されているか、または無効なサブスクリプションが渡された可能性があります。 サブスクリプションが有効であった場合は、最新のウォーターマークを使用してサブスクリプションを再作成します。 これは、登録[解除操作](unsubscribe-operation.md)または[GetEvents 操作](getevents-operation.md)の応答によって返されます。  <br/> |
|Errorsubscriptionアンサブ Sriベッド  <br/> |このエラーコードは、サブスクライブが解除されたサブスクリプションに対して要求が行われたときに返される必要があります。  <br/> |
|ErrorSyncFolderNotFound  <br/> |このエラーは、指定された親フォルダーが見つからない場合に、 [Syncfolderitems 操作](syncfolderitems-operation.md)によって返されます。  <br/> |
|ErrorTeamMailboxNotFound  <br/> |このエラーは、チームメールボックスが見つからなかったことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |このエラーは、チームメールボックスが見つかったが、SharePoint サーバーにリンクされていないことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |このエラーは、チームメールボックスが見つかったが、SharePoint サーバーへのリンクが無効であることを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |このエラーコードは使用されていません。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |このエラーコードは使用されていません。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |このエラーは、チームメールボックスの所有者に通知を送信しようとして失敗したことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |このエラーは、チームメールボックスにアクセスしようとすると発生する可能性のある一般的なエラーを示します。 後で要求を送信してみてください。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorTimeIntervalTooBig  <br/> |このエラーは、指定された時間枠が許容される制限を超えていることを示します。 既定では、許可される制限は42です。  <br/> |
|ErrorTimeoutExpired  <br/> | このエラーは、要求の処理を完了するのに十分な時間がない場合に発生します。  <br/> |
|ErrorTimeZone  <br/> |このエラーは、タイムゾーンエラーが発生したことを示します。  <br/> |
|ErrorToFolderNotFound  <br/> |このエラーは、宛先フォルダーが存在しないことを示します。  <br/> |
|ErrorTokenSerializationDenied  <br/> |このエラーは、呼び出し元がトークンのシリアル化要求を実行しようとしたときに、クライアントアクセスサーバー上で Exch-EPI-TokenSerialization 化が適切ではない場合に発生します。  <br/> |
|ErrorTooManyObjectsOpened  <br/> |このエラーは、開いているオブジェクトの内部制限を超えた場合に発生します。  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |このエラーは、ユーザーのダイヤルプランが利用できないことを示します。  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |このエラーは、ユーザーが見つからないことを示します。  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |このエラーは、要求を処理するために、ダイヤルプランの有効なサーバーが検出されたことを示します。  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |このエラーは、グループから IM 連絡先を削除しようとして失敗した場合に発生します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errorアン Supportedculture  <br/> |このエラーは、 **Culture**プロパティ**を、system.string クラスで**解析できない値に設定しようとした場合に発生します。  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |このエラーは、呼び出し元が、types オブジェクト、オブジェクト配列、エラー、または null の拡張プロパティを使用しようとした場合に発生します。  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |[Postitem](postitem.md)、 [Message](message-ex15websvcsotherref.md)、または[calendaritem](calendaritem.md)オブジェクト以外のアイテムの MIME コンテンツを取得または設定しようとすると、このエラーが発生します。  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |このエラーは、呼び出し元がクエリに対して無効なプロパティを渡した場合に発生します。 これは、集計プロパティが使用されている場合に発生する可能性があります。  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |このエラーは、呼び出し元が、sort プロパティまたは group by プロパティに対して無効なプロパティを渡した場合に発生します。 これは、集計プロパティが使用されている場合に発生する可能性があります。  <br/> |
|Errorアン Supportedpropertydefinition  <br/> |この応答コードは使用されません。  <br/> |
|Errorアン Supportedqueryfilter  <br/> |このエラーは、検索フォルダーの制限が有効であることを示しますが、EWS ではサポートされていません。  <br/> |
|エラーのない定期的なアイテム  <br/> |このエラーは、指定した定期的なパターンがタスクでサポートされていないことを示します。  <br/> |
|Errorアン Supportedサブフィルター  <br/> |この応答コードは使用されません。  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |このエラーは、Exchange Web サービスがストア内にプロパティの種類を検出したが、そのプロパティの種類の XML を生成できないことを示しています。  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |このエラーは、代理人が更新された後に、代理人の一覧が保存されなかったことを示します。  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |このエラーは、変更の説明に記載されている1つのプロパティパスが、実際の[アイテム](item.md)または[フォルダー](folder.md)オブジェクト内で設定されている単一のプロパティと一致しない場合に発生します。  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |このエラーは、リクエスターが有効になっていないことを示します。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |このエラーは、リクエスターが自分の予定表または連絡先フォルダーに外部ユーザーにアクセス許可を付与しようとしたが、その要求者に割り当てられている共有ポリシーがポリシーに含まれていないことを示していることを示します。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |依頼者の組織にはフェデレーションドメインのセットがありますが、依頼者の組織にはフェデレーションドメインのいずれかに SMTP プロキシアドレスが含まれていないことを示します。  <br/> |
|ErrorValueOutOfRange  <br/> |このエラーは、カレンダービューの開始日または終了日が 1/1/0001 12:00:00 AM または 12/31/9999 11:59:59 PM に設定されていることを示します。  <br/> |
|ErrorVirusDetected  <br/> |このエラーは、Exchange ストアがメッセージでウイルスを検出したことを示します。  <br/> |
|ErrorVirusMessageDeleted  <br/> |このエラーは、Exchange ストアがメッセージ内でウイルスを検出して削除したことを示します。  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWebRequestInInvalidState  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWin32InteropError  <br/> |このエラーは、アンマネージコードとの通信中に内部エラーが発生したことを示します。  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |この応答コードは使用されません。  <br/> |
|ErrorWrongServerVersion  <br/> |このエラーは、メールボックスサーバーと同じバージョンのサーバーにのみ、要求を実行できることを示します。  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |このエラーは、プリンシパルのメールボックスサーバーとは異なるサーバーバージョンを持つ代理人によって要求が行われたことを示します。  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |このエラーコードは返されません。  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |重複する SOAP ヘッダーがあることを指定します。  <br/> |
|Errorsharing同期に失敗しました  <br/> | 共有フォルダーを同期しようとして失敗したことを示します。<br/><br/> このエラーコードは、次の場合に返される必要があります。<br/><br/>-共有フォルダーのサブスクリプションが見つかりません。  <br/>-共有フォルダーが見つかりませんでした。  <br/>-対応するディレクトリユーザーが見つかりませんでした。  <br/>-ユーザーが存在しません。  <br/>-予定が無効です。  <br/>-連絡先アイテムが無効です。  <br/>-リモートサーバーとの通信エラーが発生しました。  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Active Directory データベースで外部 URL プロパティが設定されていないことを指定します。 このエラーコードは、外部 URL プロパティが Active Directory データベースに設定されていない場合に返される必要があります。  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |配布リストの空き時間情報を取得するために、グループメンバーの最大数に達したことを示します。 このエラーは、配布リストの空き時間情報を取得するために、グループメンバーの最大数に達している場合に返される必要があります。  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |DataType と ShareFolderId 要素の両方が要求内に存在することを指定します。 このエラーコードは、データ型と ShareFolderId 要素の両方が要求に含まれている場合に返される必要があります。  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |呼び出し元が、自分の予定表または連絡先フォルダーのアクセス許可を別の組織のユーザーに許可しようとし、失敗したことを指定します。 このエラーコードは、発信者に対して共有ポリシーが無効になっている場合、または発信者に割り当てられた共有ポリシーによって要求されたレベルまたは要求されたフォルダーの種類の共有が禁止されている場合に返されます。  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |リクエスターが予定表または連絡先フォルダーのアクセス許可を外部ユーザーに付与しようとしたが、要求者に割り当てられている共有ポリシーによって、外部ユーザーのドメインがポリシーに一覧表示されていないことを指定したことを指定します。  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |リクエスターが予定表または連絡先フォルダーのアクセス許可を外部ユーザーに付与しようとしたが、要求者に割り当てられた共有ポリシーによって、要求されたアクセス許可レベルが共有ポリシーで許可されているレベルよりも高いことを指定したことを指定します。  <br/> |
|Error組織 Notフェデレーション  <br/> |要求者の組織がフェデレーションされていないことを指定します。このため、リクエスターは、外部ユーザーに送信する共有メッセージを作成したり、外部ユーザーから受信した共有メッセージを受信したりすることはできません。 要求者の組織がフェデレーションされていない場合は、このエラーコードを返す必要があります。  <br/> |
|ErrorMailboxFailover  <br/> |メールボックスがフェールオーバープロセス内にあるために、メールボックスにアクセスしようとして失敗したことを示します。  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |共有の招待の送信者が共有の招待のメタデータを作成しなかったことを指定します。 共有の招待の送信者が共有の招待のメタデータを作成しなかった場合、このエラーコードが返される必要があります。  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |メッセージ追跡サービスがメッセージを追跡できないことを指定します。  <br/> |
|ErrorMessageTrackingTransientError  <br/> |メッセージ追跡サービスが停止しているか、またはビジーであることを指定します。 このエラーコードは、一時的なエラーを指定します。 このエラーを受け取ったときに、クライアントはサーバーへの接続を再試行できます。  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |指定したドメインが見つからないことを指定します。  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |要求者の組織にフェデレーションドメインのセットがあることを指定します。ただし、要求者の組織には、フェデレーションドメインのいずれかに SMTP プロキシアドレスが含まれていません。  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |発信者が別の組織のユーザーの空き時間情報を要求したが、組織上の関係の空き時間情報が有効になっていないことを指定します。  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |要求者の組織のフェデレーションオブジェクトが正しく構成されていないことを指定します。  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |共有メッセージが発信者に対して意図されていないことを指定します。  <br/> |
|ErrorInvalidSharingData  <br/> |共有メタデータが無効であることを指定します。 これは、無効な XML によって発生する可能性があります。  <br/> |
|ErrorInvalidSharingMessage  <br/> |共有メッセージが無効であることを指定します。 この問題は、プロパティがないことが原因で発生する場合があります。  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |共有メッセージがサポートされていないことを指定します。  <br/> |
|ErrorApplyConversationActionFailed  <br/> |このエラーは、スレッド内の1つまたは複数のアイテムに対してアクションを適用できない場合に返される必要があります。  <br/> |
|Error受信ルールの Validationerror  <br/> |このエラーは、ルールが検証されない場合に返される必要があります。  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |受信トレイルールを管理しようとしたときに、別のクライアントが受信トレイルールにアクセスした後に、このエラーが返される必要があります。  <br/> |
|Errorルール超過クォータ  <br/> |このエラーは、ユーザーのルールクォータを超過している場合に返される必要があります。  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |このエラーは、2番目のサブスクリプション接続が開かれたときに、最初のサブスクリプション接続に返される必要があります。  <br/> |
|ErrorMissedNotificationEvents  <br/> |このエラーは、イベント通知が失われたときに返される必要があります。  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |このエラーは、Active Directory ドメインサービス (AD DS) に従来の識別名が重複している場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |このエラーは、クライアントアクセストークンを取得する要求が無効であったことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorNoSpeechDetected  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|エラー Umserver使用不可  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorRecipientNotFound  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Error認識 Izernotinstalled  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSpeechGrammarError  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |このエラーは、SOAP ヘッダーの[Managementrole](managementrole.md)ヘッダーが正しくない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errorlocationサービスが無効  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errorlocationサービス Requestfailed  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errorlocationサービス Invalidrequest  <br/> |このエラーは、内部使用のみを目的としています。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorWeatherServiceDisabled  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |このエラーは、コンテンツインデックス検索で[QueryString (String)](querystring-string.md)要素を使用しないでスコープ指定された検索を実行した場合に返されます。 これは、 **Searchmailboxes ボックス**と**findconversation**操作に適用されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |このエラーは、アーカイブメールボックスの検索が失敗した場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |このエラーは、アーカイブメールボックスの URL が検出できない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errorgetremoteアーカイブ Folder失敗  <br/> |このエラーは、リモートアーカイブメールボックスフォルダーを取得する操作が失敗したときに発生します。  <br/> |
|Errorfindremote書庫 Folderfailed  <br/> |このエラーは、リモートアーカイブメールボックスフォルダーを検索する操作が失敗したときに発生します。  <br/> |
|Errorgetremoteアーカイブアイテムが失敗しました  <br/> |このエラーは、リモートアーカイブメールボックスアイテムを取得する操作が失敗したときに発生します。  <br/> |
|Errorexportremoteアーカイブアイテムが失敗しました  <br/> |このエラーは、リモートアーカイブメールボックスアイテムをエクスポートする操作が失敗したときに発生します。  <br/> |
|ErrorInvalidPhotoSize  <br/> |このエラーは、サーバーから無効な写真のサイズが要求された場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |このエラーは、 **getuserphoto**操作要求で予期しない写真サイズが要求された場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |このエラーは、 **Searchmailboxes ボックス**操作要求に含まれているメールボックスの数が多すぎて検索できない場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |このエラーは、このユーザーの保持タグが検出されなかったことを示します。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|Errordiscovery検索を無効にする  <br/> |このエラーは、テナントまたはサーバーで探索検索が無効になっている場合に返されます。 このエラーは、Exchange 2013 で導入されました。  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |このエラーは、予定表アイテムを取得するために[Seektoconditionpageitemview](seektoconditionpageitemview.md)を使用して[FindItem 操作](finditem-operation.md)を呼び出したときに発生します。これはサポートされていません。  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |このエラーは、内部使用のみを目的としています。  <br/> |
|Error組織の Accessブロック  <br/> |テナントに削除のマークが付けられます。  <br/> |
|ErrorInvalidLicense  <br/> |ユーザーが有効なライセンスを持っていません。  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |フォルダーの受信クォータのメッセージ数を超えました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は必須ではなく、すべての応答に含まれているわけではありません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

