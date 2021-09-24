---
title: DescriptiveLinkKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DescriptiveLinkKey
api_type:
- schema
ms.assetid: f7f36749-00f3-4915-b17c-e3caa0af6e67
description: DescriptiveLinkKey 要素は現在使用されていないので、将来使用するために予約されています。 値 0 が含まれる。
ms.openlocfilehash: fe646275bae3c533ee68d5137b019ea7a715c762
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519808"
---
# <a name="descriptivelinkkey"></a>DescriptiveLinkKey

**DescriptiveLinkKey 要素** は現在使用されていないので、将来使用するために予約されています。 値 0 が含まれる。 
  
```XML
<DescriptiveLinkKey/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 応答の状態に関する説明情報を提供します。  <br/><br/>この要素で使用できる XPath 式を次に示します。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>`/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>`/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |1 つの DeleteItem 要求の状態と結果 **を格納** します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |1 つの SendItem 要求の状態と結果 **を格納** します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |1 つの **DeleteFolder** 要求の状態と結果を格納します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |単一の **DeleteAttachment** 要求の状態と結果を格納します。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |1 つの Unsubscribe 要求の状態と結果 **を格納** します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |1 つの CreateFolder 要求の状態と **結果を格納** します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1 つの **GetFolder** 要求の状態と結果を格納します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |単一の **UpdateFolder** 要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1 つの **MoveFolder** 要求の状態と結果を格納します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1 つの **CopyFolder** 要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |1 つの **CreateManagedFolder** 要求の状態と結果を格納します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |1 つの **FindFolder** 要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |1 つの CreateItem 要求の状態と **結果を格納** します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |1 つの GetItem 要求の状態と **結果を格納** します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |単一の UpdateItem 要求の状態と結果 **を格納** します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1 つの MoveItem 要求の状態と結果 **を格納** します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |単一の CopyItem 要求の状態と結果 **を格納** します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1 つの **CreateAttachment 要求の状態と結果を格納** します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1 つの **GetAttachment** 要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1 つの FindItem 要求の状態と結果 **を格納** します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |ResolveNames 要求の状態と **結果を格納** します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1 つの ExpandDL 要求の状態と **結果を格納** します。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |1 つのサブスクライブ要求の状態と結果 **を格納** します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |1 つの **GetEvents** 要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1 つの **SendNotification** 要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |**SyncFolderHierarchy 要求の状態と結果を格納** します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |**SyncFolderItems** 要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |ConvertId 要求の状態と結果 **を格納** します。  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |**AddDelegate** 要求の状態と結果を格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |**GetServerTimeZones** 要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |**GetSharingFolder 要求の状態と結果を格納** します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |**GetSharingFolder 要求に対する応答を定義** します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |**GetSharingMetadata** 要求の状態と結果を格納します。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |**GetSharingMetadata 要求への応答を定義** します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |**RefreshSharingFolder** 要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |**RefreshSharingFolder 要求に対する応答を定義** します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |**FindConversation 応答の状態と結果を格納** します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |1 つの EmptyFolder 要求の状態と **結果を格納** します。  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |**UpdateInboxRules 要求の状態と結果を格納** します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |**UploadItemsResponse** 要求の状態と結果を格納します。  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |**GetInboxRules 要求に対する応答を含** む。  <br/> |
|GetServiceConfigurationResponse  <br/> |**GetServiceConfiguration 要求に対する応答を含** む。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成設定が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、テキスト値が必要です。 この要素は読み取り専用です。
  
## <a name="remarks"></a>注釈

この要素は必須ではなく、すべての応答に含まれるとは言えありません。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md) 
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

