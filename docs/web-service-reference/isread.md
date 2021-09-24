---
title: IsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRead
api_type:
- schema
ms.assetid: 161455d5-a870-4c99-b2eb-c759c538f1bc
description: IsRead 要素は、メッセージが読み取りされているかどうかを示します。
ms.openlocfilehash: cbd2fb90a413e1ec700cf07a11e0082a985545b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539396"
---
# <a name="isread"></a>IsRead

**IsRead 要素** は、メッセージが読み取りされているかどうかを示します。 
  
```XML
<IsRead/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[PostItem](postitem.md) <br/> |ストア内の投稿アイテムをExchangeします。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
|[ConversationAction](conversationaction.md) <br/> |1 つの会話に適用する 1 つのアクションが含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が **true の場合** は、メッセージが読み取りされたかどうかを示します。 テキスト値 false **は、** メッセージが読み取りされていないかどうかを示します。 
  
## <a name="remarks"></a>注釈

[IsReadReceiptRequested](isreadreceiptrequested.md)が **true** の場合 **、IsRead** を true に設定 **すると**、読み取りレシートが送信されます。 受信者は **、IsRead** プロパティを設定する前に [SuppressReadReceipt](suppressreadreceipt.md)応答オブジェクトを送信することで、読み取り受信を抑制できます。 
  
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

