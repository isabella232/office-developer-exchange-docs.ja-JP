---
title: 添付ファイル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Attachments
api_type:
- schema
ms.assetid: b470e614-34bb-44f0-8790-7ddbdcbbd29d
description: Attachments 要素には、アイテム ストア内のアイテムに添付されているアイテムまたはファイルExchangeされます。
ms.openlocfilehash: e37ff7710aaa08f3caabcecb056331091e50933c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531202"
---
# <a name="attachments"></a>Attachments

**Attachments 要素** には、アイテム ストア内のアイテムに添付されているアイテムまたはファイルExchangeされます。 
  
```xml
<Attachments>
   <ItemAttachment/>
   <FileAttachment/>
</Attachments>
```

 **ArrayOfAttachmentsType** と **NonEmptyArrayOfAttachmentsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |別のアイテムExchange付けられたアイテムを表Exchangeします。  <br/> |
|[FileAttachment](fileattachment.md) <br/> |アイテム ストア内のアイテムに添付されているファイルをExchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |アイテムストア内のアイテムへの添付ファイルを作成する要求をExchangeします。<br/><br/> 次に、この要素の XPath 式を示します。  `/CreateAttachment` <br/> |
|[AcceptItem](acceptitem.md) <br/> | 会議出席依頼に対する Accept 返信を表します。<br/><br/>次に、この要素の XPath 式の一部を示します。<ul><li>`/CreateItem/Items`</li><li>`/MeetingRequest/ConflictingMeetings` </li><li>`/SetItemField/CalendarItem/ConflictingMeetings`</li><li>`/AppendToItemField/CalendarItem/ConflictingMeetings`</li><li>`/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings`</li><li>`/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings`</li><li>`/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li><li>`/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings`</li></ul> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮返信を表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[項目](item.md) <br/> |アイテムの一般的なExchangeを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |1 つの CreateAttachment 要求の状態と結果を格納します。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |GetAttachment 要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

**Attachments 要素** は同じ子要素を持っていますが、**配列OfAttachmentsType** と **NonEmptyArrayOfAttachmentsType** の異なる型に基づいて作成されます。 型は、子要素が必要かどうかを定義します。 **ArrayOfAttachmentsType は** 応答メッセージでのみ使用されます。 これらの要素は、メッセージ名前空間と型名前空間の両方で発生します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

