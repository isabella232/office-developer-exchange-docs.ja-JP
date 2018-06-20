---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: ResponseMessages 要素には、Exchange Web サービス要求に対する応答メッセージが含まれています。
ms.openlocfilehash: dc56476447cceac4eca56c171b148ac1ed177cb3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833203"
---
# <a name="responsemessages"></a>ResponseMessages

**ResponseMessages**要素には、Exchange Web サービス要求に対する応答メッセージが含まれています。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |状態および 1 つの CopyFolder 要求の結果が含まれています。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |状態および 1 つの CopyItem 要求の結果が含まれています。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |状態および 1 つの CreateAttachment 要求の結果が含まれています。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |CreateFolder 要求を 1 つの結果には状態が含まれます。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |状態および 1 つの CreateItem 要求の結果が含まれています。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |状態および 1 つの CreateManagedFolder 要求の結果が含まれています。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |状態および 1 つの DeleteAttachment 要求の結果が含まれています。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |状態および 1 つの DeleteFolder 要求の結果が含まれています。  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |状態および 1 つの DeleteItem 要求の結果が含まれています。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |[EmptyFolder](emptyfolder.md)要求を 1 つの結果には状態が含まれます。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |状態および 1 つの ExpandDL 要求の結果が含まれています。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |状態および 1 つの FindFolder 要求の結果が含まれています。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |状態および 1 つの FindItem 要求の結果が含まれています。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |状態および 1 つの GetAttachment 要求の結果が含まれています。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |状態および 1 つの UploadItems 要求の結果が含まれています。  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |状態および 1 つの ExportItems 要求の結果が含まれています。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |状態および 1 つの GetEvents 要求の結果が含まれています。  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |状態および 1 つの GetStreamingEvents 要求の結果が含まれています。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |状態および 1 つの GetFolder 要求の結果が含まれています。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |状態および 1 つの GetItem 要求の結果が含まれています。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |状態および 1 つの MoveFolder 要求の結果が含まれています。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |状態および 1 つの MoveItem 要求の結果が含まれています。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の結果ステータスを格納します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |状態および 1 つの SendItem 要求の結果が含まれています。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |状態および 1 つの SendNotification 要求の結果が含まれています。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |状態および 1 つの購読要求の結果が含まれています。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の結果ステータスを格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |SyncFolderItems 要求の結果ステータスを格納します。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |状態および 1 つの購読の取り消し要求の結果が含まれています。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |状態および 1 つの UpdateFolder 要求の結果が含まれています。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |状態および 1 つの UpdateItem 要求の結果が含まれています。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |状態および ConvertId の要求の結果が含まれています。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |状態および GetSharingMetadata の要求の結果が含まれています。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |状態および RefreshSharingFolder の要求の結果が含まれています。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |状態および GetSharingFolder の要求の結果が含まれています。  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |状態および CreateUserConfiguration の要求の結果が含まれています。  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |状態および DeleteUserConfiguration の要求の結果が含まれています。  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |状態および GetUserConfiguration の要求の結果が含まれています。  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |状態および UpdateUserConfiguration の要求の結果が含まれています。  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |状態および GetRoomLists の要求の結果が含まれています。  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |状態および GetRooms の要求の結果が含まれています。  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |状態および GetReminders の要求の結果が含まれています。  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |状態および PerformReminderAction の要求の結果が含まれています。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |状態および 1 つの GetServerTimeZones 要求の結果が含まれています。  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |状態と[ApplyConversationAction の操作](applyconversationaction-operation.md)要求の結果が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponse](copyfolderresponse.md) <br/> |CopyFolder 要求への応答を定義します。  <br/> |
|[CopyItemResponse](copyitemresponse.md) <br/> |CopyItem 要求への応答を定義します。  <br/> |
|[CreateAttachmentResponse](createattachmentresponse.md) <br/> |CreateAttachment 要求への応答を定義します。  <br/> |
|[CreateFolderResponse](createfolderresponse.md) <br/> |CreateFolder 要求への応答を定義します。  <br/> |
|[CreateItemResponse](createitemresponse.md) <br/> |CreateItem 要求への応答を定義します。  <br/> |
|[CreateManagedFolderResponse](createmanagedfolderresponse.md) <br/> |CreateManagedFolder 要求への応答を定義します。  <br/> |
|[DeleteAttachmentResponse](deleteattachmentresponse.md) <br/> |DeleteAttachment 要求への応答を定義します。  <br/> |
|[DeleteFolderResponse](deletefolderresponse.md) <br/> |DeleteFolder 要求への応答を定義します。  <br/> |
|[DeleteItemResponse](deleteitemresponse.md) <br/> |DeleteItem 要求への応答を定義します。  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |EmptyFolder 要求への応答を定義します。  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |ExpandDL 要求への応答を定義します。  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |1 つの ExportItems 要求への応答を表します。  <br/> |
|[FindFolderResponse](findfolderresponse.md) <br/> |FindFolder 要求への応答を定義します。  <br/> |
|[FindItemResponse](finditemresponse.md) <br/> |FindItem 要求への応答を定義します。  <br/> |
|[GetAttachmentResponse](getattachmentresponse.md) <br/> |GetAttachment 要求への応答を定義します。  <br/> |
|[GetEventsResponse](geteventsresponse.md) <br/> |GetEvents 要求への応答を定義します。  <br/> |
|[GetStreamingEventsResponse](getstreamingeventsresponse.md) <br/> |GetStreamingEvents 要求への応答を定義します。  <br/> |
|[GetFolderResponse](getfolderresponse.md) <br/> |GetFolder 要求への応答を定義します。  <br/> |
|[GetItemResponse](getitemresponse.md) <br/> |GetItem 要求への応答を定義します。  <br/> |
|[MoveFolderResponse](movefolderresponse.md) <br/> |MoveFolder 要求への応答を定義します。  <br/> |
|[MoveItemResponse](moveitemresponse.md) <br/> |MoveItem 要求への応答を定義します。  <br/> |
|[ResolveNamesResponse](resolvenamesresponse.md) <br/> |ResolveNames 要求への応答を定義します。  <br/> |
|[SendItemResponse](senditemresponse.md) <br/> |SendItem 要求への応答を定義します。  <br/> |
|[SendNotificationResult](sendnotificationresult.md) <br/> |SendNotification 要求への応答を定義します。  <br/> |
|[SubscribeResponse](subscriberesponse.md) <br/> |Subscribe 要求への応答を定義します。  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |SyncFolderHierarchy 要求への応答を定義します。  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |SyncFolderItems 要求への応答を定義します。  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |購読中止要求への応答を定義します。  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |UpdateFolder 要求への応答を定義します。  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |UpdateItem 要求への応答を定義します。  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |ConvertId 要求への応答が含まれています。  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |GetServerTimeZones 要求への応答を定義します。  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |CreateUserConfiuration 要求への応答を定義します。  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |DeleteUserConfiguration 要求への応答を定義します。  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |GetUserConfiguration 要求への応答を定義します。  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |UpdateUserConfiguration 要求への応答を定義します。  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |[ApplyConversationAction 操作](applyconversationaction-operation.md)要求への応答を定義します。  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)の操作要求に対する応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md) 
- [UploadItems 操作](uploaditems-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

