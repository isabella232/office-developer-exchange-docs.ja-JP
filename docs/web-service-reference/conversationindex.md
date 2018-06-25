---
title: ConversationIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationIndex
api_type:
- schema
ms.assetid: fdf47e22-8d93-4ae4-883b-0c9f07f48724
description: ConversationIndex 要素には、このメッセージが属するスレッドを表すバイナリの ID が含まれています。
ms.openlocfilehash: 3f4f72224269717325d2fbf56f0a25fab20352a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759755"
---
# <a name="conversationindex"></a>ConversationIndex

**ConversationIndex**要素には、このメッセージが属するスレッドを表すバイナリの ID が含まれています。 
  
```xml
<ConversationIndex/>
```

 **Base64Binary**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼、承諾の返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に仮承諾の返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼を辞退の返信を表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの作成者に返信が含まれています。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送するのには、Exchange ストアの項目が含まれています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議をキャンセルするために使用される応答オブジェクトを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、 **Base64Binary**形式でバイナリの識別子を表します。 
  
## <a name="remarks"></a>備考

EWS 仮想ディレクトリのクライアント アクセス サーバーの役割がインストールされている Exchange サーバーには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

