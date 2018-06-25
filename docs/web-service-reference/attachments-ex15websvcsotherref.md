---
title: 添付ファイル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: 添付ファイルの要素には、アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。
ms.openlocfilehash: 8aa5c0849122f5ca83485459fce5d0fea449c974
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759456"
---
# <a name="attachments"></a>添付ファイル

**添付ファイル**の要素には、アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 **ArrayOfAttachmentsType**と**NonEmptyArrayOfAttachmentsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに関連付けられているファイルを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Exchange ストア内のアイテムに添付ファイルを作成する要求を定義します。<br/><br/> この要素への XPath 式は、次のようにします。`/CreateAttachment` <br/> |
|[AcceptItem](acceptitem.md) <br/> | 会議出席依頼、承諾の返信を表します。<br/><br/>以下は、この要素への XPath 式の一部です。<ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼を辞退の返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |仮の予定を表しますが、会議出席依頼に返信します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[アイテム](item.md) <br/> |一般的な Exchange アイテムを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |状態および 1 つの CreateAttachment 要求の結果が含まれています。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |GetAttachment 要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

**添付ファイル**の要素が同じの子要素を持つが、さまざまな種類に基づいています: **ArrayOfAttachmentsType**と**NonEmptyArrayOfAttachmentsType**。 型では、子要素が必要かどうかを定義します。 **ArrayOfAttachmentsType**は、応答メッセージにのみ使用されます。 メッセージと型の両方の名前空間でこれらの要素が発生することに注意する必要もします。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

