---
title: ReplyAllToItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyAllToItem
api_type:
- schema
ms.assetid: 8ca970ca-ca73-40db-9233-7b271cc5f44f
description: ReplyToAllItem 要素には、Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。
ms.openlocfilehash: 99ee3427babba2c91c7c3b4ad5a750fddca6cbfd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833129"
---
# <a name="replyalltoitem"></a>ReplyAllToItem

**ReplyToAllItem**要素には、Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。 
  
```xml
<ReplyAllToItem>
   <Subject/>
   <Body/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <From/>
   <ReferenceItemId/>
   <NewBodyContent/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</ReplyAllToItem>
```

 **ReplyAllToItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Subject](subject.md) <br/> |Exchange ストアのアイテムの subject プロパティを表します。  <br/> |
|[Body/本文](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[ToRecipients](torecipients.md) <br/> |アイテムの受信者のセットが含まれています。 これらは、アイテムの主な受信者です。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受け取る受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メール メッセージのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |アイテムの送信者が開封確認メッセージを要求するかどうかを示します。  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |アイテムの送信者が配信済みメッセージを要求するかどうかを示します。  <br/> |
|[From](from.md) <br/> |メッセージの送信元アドレスを表します。  <br/> |
|[ReferenceItemId](referenceitemid.md) <br/> |応答オブジェクトが参照する項目を識別します。  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |メッセージの新しい本文の内容を表します。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセス シナリオでは、デリゲートを識別します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセスのシナリオでプリンシパルを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> | 会議の時刻に隣接しているすべての項目について説明します。  <br/><br/>  以下は、この要素への XPath 式の一部です。  <br/><br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> | 会議の時間と競合するすべての項目について説明します。  <br/><br/>  以下は、この要素への XPath 式の一部です。 <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で指定されたフォルダーに作成する項目の配列が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

要素[から](from.md)設定してください、プリンシパルの電子メール アドレスにアイテムが返信の場合代理人によって。 代理人が、 [From](from.md)プロパティを設定していない場合、代理人のメールボックスから直接送信されたアイテムが表示されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

