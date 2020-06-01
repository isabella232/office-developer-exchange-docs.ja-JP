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
ms.openlocfilehash: 180b447874523742a1d29d457c4ef020e4124f7c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466277"
---
# <a name="messagexml"></a>MessageXml

**MessageXml**要素は、追加のエラー応答情報を提供します。 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **xs: any**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 応答状態に関する説明情報を提供します。 <br/> <br/>  この要素に使用できる XPath 式の一部を次に示します。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |単一の DeleteItem 要求の状態と結果を格納します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |単一の SendItem 要求の状態と結果を格納します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |単一の DeleteFolder 要求の状態と結果を格納します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |1回の DeleteAttachment 要求の状態と結果を格納します。  <br/> |
|[非表示の表示/非表示のメッセージ](unsubscriberesponsemessage.md) <br/> |単一の登録取り消し要求の状態と結果を格納します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の CreateFolder 要求の状態と結果を格納します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1つの GetFolder 要求の状態と結果を格納します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |1つの UpdateFolder 要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1つの MoveFolder 要求の状態と結果を格納します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1つの CopyFolder 要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |単一の CreateManagedFolder 要求の状態と結果を格納します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |単一の FindFolder 要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |単一の CreateItem 要求の状態と結果を格納します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |単一の GetItem 要求の状態と結果を格納します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |1つの UpdateItem 要求の状態と結果を格納します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1つの MoveItem 要求の状態と結果を格納します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |1つの CopyItem 要求の状態と結果を格納します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1つの CreateAttachment 要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1つの GetAttachment 要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1つの FindItem 要求の状態と結果を格納します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の状態と結果を格納します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1つの ExpandDL 要求の状態と結果を格納します。  <br/> |
|[メッセージの表示](subscriberesponsemessage.md) <br/> |1つの Subscribe 要求の状態と結果を格納します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |単一の GetEvents 要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1回の SendNotification 要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |SyncFolderHierarchy 要求の状態と結果を格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |SyncFolderItems 要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |[コンバーター] 要求の状態と結果を格納します。  <br/> |
|[含む adddelegateresponse](adddelegateresponse.md) <br/> |AddDelegate 要求の状態と結果を格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |GetServerTimeZones 要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |GetSharingFolder 要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |GetSharingFolder 要求への応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |GetSharingMetadata 要求の状態と結果を格納します。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |GetSharingMetadata 要求への応答を定義します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |RefreshSharingFolder 要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |RefreshSharingFolder 要求への応答を定義します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |**Findconversation**応答の状態と結果を格納します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |**Emptyfolder**要求の状態と結果を格納します。  <br/> |
|[Update受信トレイルールの応答](updateinboxrulesresponse.md) <br/> |**Update受信トレイルール**要求の状態と結果を格納します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |**UploadItemsResponse**要求の状態と結果を格納します。  <br/> |
|[Get受信規則の応答](getinboxrulesresponse.md) <br/> |**Get受信トレイ**の要求への応答を含みます。  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |**GetServiceConfiguration**要求への応答を含みます。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は必須ではなく、すべての応答に含まれているわけではありません。 エラーメッセージには含まれています。 フォルダーまたはアイテムに関連する要求では、 **MessageXML**要素には、エラーの原因となったプロパティへの uri を含む1つ以上の要素が含まれます。 この例は、 [FieldURI](fielduri.md)要素です。 
  
**MessageXML**要素の型は**xs: any**で、適切な形式の XML はこの要素の有効なコンテンツであることを意味します。
  
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

