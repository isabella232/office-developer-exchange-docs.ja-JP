---
title: アイテム (非 Emptyarrayofallitemstype)
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
description: Items 要素には、作成する一連のアイテムが含まれています。
ms.openlocfilehash: 0f70f1fe4348b5b74cef6be6414618af1e3de260
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459855"
---
# <a name="items-nonemptyarrayofallitemstype"></a>アイテム (非 Emptyarrayofallitemstype)

**Items**要素には、作成する一連のアイテムが含まれています。 
  
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

 **非 Emptyarrayofallitemstype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの送信者への返信を含みます。  <br/> |
|[Forwarditem と](forwarditem.md) <br/> |受信者に転送するための Exchange ストアアイテムが保存されています。  <br/> |
|[Replyalltoitem と](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの送信者および特定の受信者への返信を含みます。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼への返信を承諾するかを表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮の返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼への返信を拒否することを表します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議の取り消しに使用される response オブジェクトを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |会議の取り消しメッセージを受信したときに会議アイテムを削除するために使用される response オブジェクトを表します。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信を含みます。  <br/> |
|[SuppressReadReceipt](suppressreadreceipt.md) <br/> |開封確認メッセージを抑制するために使用します。  <br/> |
|[AcceptSharingInvitation 状](acceptsharinginvitation.md) <br/> |別のユーザーの予定表または連絡先データへのアクセスを許可する招待を承諾するために使用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Exchange ストアにアイテムを作成するための要求を定義します。  <br/> この要素の XPath 式を次に示します。`/CreateItem` <br/> |
|[ConversationNode](conversationnode.md) <br/> |会話内の1つのノードを識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [CreateFolder 操作](createfolder-operation.md)
  

  [CreateItem 操作](createitem-operation.md)


[フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

