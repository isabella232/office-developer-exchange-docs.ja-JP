---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: ResponseMessages 要素には、Web Services 要求の応答メッセージExchange含まれます。
ms.openlocfilehash: 23fa25b29cec0377d83ecf56a094da86af6c5213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516391"
---
# <a name="responsemessages"></a>ResponseMessages

**ResponseMessages 要素には**、Web Services 要求の応答メッセージExchange含まれます。 
  
```XML
<ResponseMessages>
   <CreateItemResponseMessage/>
</ResponseMessages>
```

```xml
<ResponseMessages>
   <DeleteItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <EmptyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UploadItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExportItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ResolveNamesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExpandDLResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetServerTimeZonesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetStreamingEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UnsubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendNotificationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderHierarchyResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateManagedFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ConvertIdResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingMetadataResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <RefreshSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomListsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRemindersResponse/>
</ResponseMessages
```

```xml 
<ResponseMessages>
   <PerformReminderActionResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ApplyConversationActionResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetPasswordExpirationDateResponse />
</ResponseMessages>
```


**ArrayOfResponseMessagesType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1 つの CopyFolder 要求の状態と結果を格納します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |単一の CopyItem 要求の状態と結果を格納します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1 つの CreateAttachment 要求の状態と結果を格納します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |1 つの CreateFolder 要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |1 つの CreateItem 要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |1 つの CreateManagedFolder 要求の状態と結果を格納します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |単一の DeleteAttachment 要求の状態と結果を格納します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |1 つの DeleteFolder 要求の状態と結果を格納します。  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |1 つの DeleteItem 要求の状態と結果を格納します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |1 つの EmptyFolder 要求の状態と [結果を格納](emptyfolder.md) します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1 つの ExpandDL 要求の状態と結果を格納します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |1 つの FindFolder 要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1 つの FindItem 要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1 つの GetAttachment 要求の状態と結果を格納します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |1 つの UploadItems 要求の状態と結果を格納します。  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |単一の ExportItems 要求の状態と結果を格納します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |1 つの GetEvents 要求の状態と結果を格納します。  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |1 つの GetStreamingEvents 要求の状態と結果を格納します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1 つの GetFolder 要求の状態と結果を格納します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |1 つの GetItem 要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1 つの MoveFolder 要求の状態と結果を格納します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1 つの MoveItem 要求の状態と結果を格納します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の状態と結果を格納します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |1 つの SendItem 要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1 つの SendNotification 要求の状態と結果を格納します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |1 つのサブスクライブ要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の状態と結果を格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |SyncFolderItems 要求の状態と結果を格納します。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |1 つの Unsubscribe 要求の状態と結果を格納します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |単一の UpdateFolder 要求の状態と結果を格納します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |単一の UpdateItem 要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |ConvertId 要求の状態と結果を格納します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |GetSharingMetadata 要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |RefreshSharingFolder 要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |GetSharingFolder 要求の状態と結果を格納します。  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |CreateUserConfiguration 要求の状態と結果を格納します。  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |DeleteUserConfiguration 要求の状態と結果を格納します。  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |GetUserConfiguration 要求の状態と結果を格納します。  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |UpdateUserConfiguration 要求の状態と結果を格納します。  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |GetRoomLists 要求の状態と結果を格納します。  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |GetRooms 要求の状態と結果を格納します。  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |GetReminders 要求の状態と結果を格納します。  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |PerformReminderAction 要求の状態と結果を格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |1 つの GetServerTimeZones 要求の状態と結果を格納します。  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |[ApplyConversationAction](applyconversationaction-operation.md)操作要求の状態と結果を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponse](copyfolderresponse.md) <br/> |CopyFolder 要求に対する応答を定義します。  <br/> |
|[CopyItemResponse](copyitemresponse.md) <br/> |CopyItem 要求に対する応答を定義します。  <br/> |
|[CreateAttachmentResponse](createattachmentresponse.md) <br/> |CreateAttachment 要求に対する応答を定義します。  <br/> |
|[CreateFolderResponse](createfolderresponse.md) <br/> |CreateFolder 要求への応答を定義します。  <br/> |
|[CreateItemResponse](createitemresponse.md) <br/> |CreateItem 要求に対する応答を定義します。  <br/> |
|[CreateManagedFolderResponse](createmanagedfolderresponse.md) <br/> |CreateManagedFolder 要求に対する応答を定義します。  <br/> |
|[DeleteAttachmentResponse](deleteattachmentresponse.md) <br/> |DeleteAttachment 要求に対する応答を定義します。  <br/> |
|[DeleteFolderResponse](deletefolderresponse.md) <br/> |DeleteFolder 要求に対する応答を定義します。  <br/> |
|[DeleteItemResponse](deleteitemresponse.md) <br/> |DeleteItem 要求に対する応答を定義します。  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |EmptyFolder 要求に対する応答を定義します。  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |ExpandDL 要求に対する応答を定義します。  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |単一の ExportItems 要求に対する応答を表します。  <br/> |
|[FindFolderResponse](findfolderresponse.md) <br/> |FindFolder 要求への応答を定義します。  <br/> |
|[FindItemResponse](finditemresponse.md) <br/> |FindItem 要求に対する応答を定義します。  <br/> |
|[GetAttachmentResponse](getattachmentresponse.md) <br/> |GetAttachment 要求への応答を定義します。  <br/> |
|[GetEventsResponse](geteventsresponse.md) <br/> |GetEvents 要求に対する応答を定義します。  <br/> |
|[GetStreamingEventsResponse](getstreamingeventsresponse.md) <br/> |GetStreamingEvents 要求への応答を定義します。  <br/> |
|[GetFolderResponse](getfolderresponse.md) <br/> |GetFolder 要求に対する応答を定義します。  <br/> |
|[GetItemResponse](getitemresponse.md) <br/> |GetItem 要求に対する応答を定義します。  <br/> |
|[MoveFolderResponse](movefolderresponse.md) <br/> |MoveFolder 要求への応答を定義します。  <br/> |
|[MoveItemResponse](moveitemresponse.md) <br/> |MoveItem 要求に対する応答を定義します。  <br/> |
|[ResolveNamesResponse](resolvenamesresponse.md) <br/> |ResolveNames 要求に対する応答を定義します。  <br/> |
|[SendItemResponse](senditemresponse.md) <br/> |SendItem 要求に対する応答を定義します。  <br/> |
|[SendNotificationResult](sendnotificationresult.md) <br/> |SendNotification 要求に対する応答を定義します。  <br/> |
|[SubscribeResponse](subscriberesponse.md) <br/> |サブスクライブ要求に対する応答を定義します。  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |SyncFolderHierarchy 要求への応答を定義します。  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |SyncFolderItems 要求に対する応答を定義します。  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |Unsubscribe 要求に対する応答を定義します。  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |UpdateFolder 要求に対する応答を定義します。  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |UpdateItem 要求に対する応答を定義します。  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |ConvertId 要求に対する応答を含む。  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |GetServerTimeZones 要求への応答を定義します。  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |CreateUserConfiuration 要求への応答を定義します。  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |DeleteUserConfiguration 要求への応答を定義します。  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |GetUserConfiguration 要求に対する応答を定義します。  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |UpdateUserConfiguration 要求への応答を定義します。  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |[ApplyConversationAction 操作要求への応答を定義](applyconversationaction-operation.md)します。  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |[GetPasswordExpirationDate 操作要求への応答を](getpasswordexpirationdate-operation.md)定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md) 
- [UploadItems 操作](uploaditems-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

