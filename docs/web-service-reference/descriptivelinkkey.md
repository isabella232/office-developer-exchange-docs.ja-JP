---
title: DescriptiveLinkKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DescriptiveLinkKey
api_type:
- schema
ms.assetid: f7f36749-00f3-4915-b17c-e3caa0af6e67
description: DescriptiveLinkKey 要素は現在未使用で、今後の使用のために予約されています。 このプロパティには0の値が含まれています。
ms.openlocfilehash: e078d4ef4a629ea06bab0c2eb02b4f67b4fbf651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467873"
---
# <a name="descriptivelinkkey"></a>DescriptiveLinkKey

**DescriptiveLinkKey**要素は現在未使用で、今後の使用のために予約されています。 このプロパティには0の値が含まれています。 
  
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
|[ResponseMessage](responsemessage.md) <br/> | 応答状態に関する説明情報を提供します。  <br/><br/>この要素には、次のような XPath 式があります。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>`/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>`/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |単一の**DeleteItem**要求の状態と結果を格納します。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |単一の**SendItem**要求の状態と結果を格納します。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |単一の**Deletefolder**要求の状態と結果を格納します。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |1回の**Deleteattachment**要求の状態と結果を格納します。  <br/> |
|[非表示の表示/非表示のメッセージ](unsubscriberesponsemessage.md) <br/> |単一の登録**取り消し**要求の状態と結果を格納します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の**CreateFolder**要求の状態と結果を格納します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |1つの**Getfolder**要求の状態と結果を格納します。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |1つの**Updatefolder**要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |1つの**Movefolder**要求の状態と結果を格納します。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1つの**Copyfolder**要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |単一の**CreateManagedFolder**要求の状態と結果を格納します。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |単一の**Findfolder**要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |単一の**CreateItem**要求の状態と結果を格納します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |単一の**GetItem**要求の状態と結果を格納します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |1つの**Updateitem**要求の状態と結果を格納します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |1つの**Moveitem**要求の状態と結果を格納します。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |1つの**Copyitem**要求の状態と結果を格納します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1つの**Createattachment**要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |1つの**Getattachment**要求の状態と結果を格納します。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |1つの**FindItem**要求の状態と結果を格納します。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |**ResolveNames**要求の状態と結果を格納します。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1つの**Expanddl**要求の状態と結果を格納します。  <br/> |
|[メッセージの表示](subscriberesponsemessage.md) <br/> |1つの**Subscribe**要求の状態と結果を格納します。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |単一の**GetEvents**要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1回の**Sendnotification**要求の状態と結果を格納します。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |**Syncfolderhierarchy**要求の状態と結果を格納します。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |**Syncfolderitems**要求の状態と結果を格納します。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |[**コンバーター** ] 要求の状態と結果を格納します。  <br/> |
|[含む adddelegateresponse](adddelegateresponse.md) <br/> |**Adddelegate**要求の状態と結果を格納します。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |**GetServerTimeZones**要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |**Getsharingfolder**要求の状態と結果を格納します。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |**Getsharingfolder**要求への応答を定義します。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |**Getsharingmetadata**要求の状態と結果を格納します。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |**Getsharingmetadata**要求への応答を定義します。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |**Refreshsharingfolder**要求の状態と結果を格納します。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |**Refreshsharingfolder**要求への応答を定義します。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |**Findconversation**応答の状態と結果を格納します。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |単一の**Emptyfolder**要求の状態と結果を格納します。  <br/> |
|[Update受信トレイルールの応答](updateinboxrulesresponse.md) <br/> |**Update受信トレイルール**要求の状態と結果を格納します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |**UploadItemsResponse**要求の状態と結果を格納します。  <br/> |
|[Get受信規則の応答](getinboxrulesresponse.md) <br/> |**Get受信トレイ**の要求への応答を含みます。  <br/> |
|GetServiceConfigurationResponse  <br/> |**GetServiceConfiguration**要求への応答を含みます。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |サービス構成の設定が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、テキスト値が必要です。 この要素は値の取得のみ可能です。
  
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

- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md) 
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

