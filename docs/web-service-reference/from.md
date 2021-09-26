---
title: From
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- From
api_type:
- schema
ms.assetid: 5a52d644-3677-4049-874c-12bd5c3080dc
description: From 要素は、メッセージの送信先アドレスを表します。
ms.openlocfilehash: 63f4e82a0f32d9d081d2ff6c7572b9b27bd3d2c0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546393"
---
# <a name="from"></a>From

**From 要素** は、メッセージの送信先アドレスを表します。 
  
```xml
<From>
   <Mailbox/>
</From>
```

 **SingleRecipientType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼に対する Accept 返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |ストア内のアイテムの作成者への返信Exchangeします。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |アイテムストア内のアイテムの識別された受信者全員に対する返信Exchangeします。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送Exchangeストア アイテムを格納します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議のキャンセルに使用される応答オブジェクトを表します。  <br/> |
|[PostItem](postitem.md) <br/> |ストア内の投稿アイテムをExchangeします。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、"代理送信" 電子メールに使用されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

