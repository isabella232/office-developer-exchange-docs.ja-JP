---
title: アイテム (NonEmptyArrayOfAllItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: d61ef1cc-ddfc-480a-9625-7b436cb33ae0
description: 項目要素には、作成するアイテムのセットが含まれています。
ms.openlocfilehash: 3b1ce7092bb6d37f23792fbf1ecb1f77b63f2afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832160"
---
# <a name="items-nonemptyarrayofallitemstype"></a>アイテム (NonEmptyArrayOfAllItemsType)

**項目**要素には、作成するアイテムのセットが含まれています。 
  
```XML
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <ReplyToItem/>
   <ForwardItem/>
   <ReplyAllToItem/>
   <AcceptItem/>
   <TentativelyAcceptItem/>
   <DeclineItem/>
   <CancelCalendarItem/>
   <RemoveItem/>
   <PostReplyItem/>
   <SuppressReadReceipt/>
   <AcceptSharingInvitation/>
</Items>
```

 **NonEmptyArrayOfAllItemsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議のメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの送信者への返信が含まれています。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送するのには、Exchange ストアの項目が含まれています。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼、承諾の返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |仮の予定を表しますが、会議出席依頼に返信します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼を辞退の返信を表します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議をキャンセルするために使用される応答オブジェクトを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信が含まれています。  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |開封確認メッセージを非表示にするために使用します。  <br/> |
|[AcceptSharingInvitation](acceptsharinginvitation.md) <br/> |別のユーザーの予定表や連絡先のデータへのアクセスを可能にするための招待を承諾する場合に使用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Exchange ストア内のアイテムを作成する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。`/CreateItem` <br/> |
|[ConversationNode](conversationnode.md) <br/> |会話で 1 つのノードを識別します。  <br/> |
   
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




  [CreateFolder 操作](createfolder-operation.md)
  

  [CreateItem 操作](createitem-operation.md)


[フォルダー (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

