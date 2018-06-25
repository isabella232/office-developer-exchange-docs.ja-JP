---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: MessageXml 要素は、追加のエラー応答情報を提供します。
ms.openlocfilehash: 8b6d201fe35c99a65f920ed7f60c33a2271fbd2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832470"
---
# <a name="messagexml"></a>MessageXml

**MessageXml**要素は、追加のエラー応答情報を提供します。 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **xs: 任意**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 応答ステータスに関する説明情報を提供します。 <br/> <br/>  以下は、この要素に使用可能な XPath 式の一部です。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |状態および 1 つの DeleteItem 要求の結果が含まれています。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |状態および 1 つの SendItem 要求の結果が含まれています。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |状態および 1 つの DeleteFolder 要求の結果が含まれています。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |状態および 1 つの DeleteAttachment 要求の結果が含まれています。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |状態および 1 つの購読の取り消し要求の結果が含まれています。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |CreateFolder 要求を 1 つの結果には状態が含まれます。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |状態および 1 つの GetFolder 要求の結果が含まれています。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |状態および 1 つの UpdateFolder 要求の結果が含まれています。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |状態および 1 つの MoveFolder 要求の結果が含まれています。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |状態および 1 つの CopyFolder 要求の結果が含まれています。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |状態および 1 つの CreateManagedFolder 要求の結果が含まれています。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |状態および 1 つの FindFolder 要求の結果が含まれています。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |状態および 1 つの CreateItem 要求の結果が含まれています。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |状態および 1 つの GetItem 要求の結果が含まれています。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |状態および 1 つの UpdateItem 要求の結果が含まれています。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |状態および 1 つの MoveItem 要求の結果が含まれています。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |状態および 1 つの CopyItem 要求の結果が含まれています。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |状態および 1 つの CreateAttachment 要求の結果が含まれています。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |状態および 1 つの GetAttachment 要求の結果が含まれています。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |状態および 1 つの FindItem 要求の結果が含まれています。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の結果ステータスを格納します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |状態および 1 つの ExpandDL 要求の結果が含まれています。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |状態および 1 つの購読要求の結果が含まれています。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |状態および 1 つの GetEvents 要求の結果が含まれています。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |状態および 1 つの SendNotification 要求の結果が含まれています。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の結果ステータスを格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |SyncFolderItems 要求の結果ステータスを格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |状態および ConvertId の要求の結果が含まれています。  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |AddDelegate 要求の結果ステータスを格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |状態および GetServerTimeZones の要求の結果が含まれています。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |状態および GetSharingFolder の要求の結果が含まれています。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |GetSharingFolder 要求への応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |状態および GetSharingMetadata の要求の結果が含まれています。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |GetSharingMetadata 要求への応答を定義します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |状態および RefreshSharingFolder の要求の結果が含まれています。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |RefreshSharingFolder 要求への応答を定義します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |状態と**FindConversation**の応答の結果が含まれています。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |**EmptyFolder**要求の結果ステータスを格納します。  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |状態および**UpdateInboxRules**の要求の結果が含まれています。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |状態および**UploadItemsResponse**の要求の結果が含まれています。  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |**GetInboxRules**要求への応答が含まれています。  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |**GetServiceConfiguration**要求への応答が含まれています。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素は必須ではなく、すべての応答に含まれません。 エラー メッセージに含まれます。 フォルダーまたはアイテムは、 **MessageXML**要素を含むクエリでエラーが発生したプロパティへの Uri を含む 1 つまたは複数の要素が含まれます。 この例は、 [FieldURI](fielduri.md)要素です。 
  
型の**MessageXML**要素は、 **x:**、任意の整形式の XML が、これの有効なコンテンツであることを意味する要素です。
  
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

