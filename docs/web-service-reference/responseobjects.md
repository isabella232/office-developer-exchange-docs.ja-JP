---
title: ResponseObjects
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseObjects
api_type:
- schema
ms.assetid: ad29e064-3f3d-4b7b-aa4c-9ec27326381d
description: ResponseObjects 要素には、アイテム ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションExchangeされます。
ms.openlocfilehash: 65676bba6a78ce4533eb4dabab51106f9799d625
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544802"
---
# <a name="responseobjects"></a>ResponseObjects

**ResponseObjects 要素** には、アイテム ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションがExchangeされます。 
  
```XML
<ResponseObjects>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <ProposeNewTime>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</ResponseObjects>
```

 **NonEmptyArrayOfResponseObjectsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼に対する Accept 返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[ProposeNewTime](proposenewtime.md) <br/> |会議の出席者が新しい会議時間を提案できる状態を示します。 この要素は、2013 Microsoft Exchange Server Service Pack 1 (SP1) で導入されました。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |ストア内のアイテムの作成者への返信Exchangeします。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送Exchangeストア アイテムを格納します。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |アイテムストア内のアイテムの識別された受信者全員に対する返信Exchangeします。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議のキャンセルに使用される応答オブジェクトを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信を含む。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |読み取り受信要求を抑制するために使用します。  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |別のユーザーの予定表または連絡先データへのアクセスを許可する招待を受け入れる場合に使用します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[項目](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

