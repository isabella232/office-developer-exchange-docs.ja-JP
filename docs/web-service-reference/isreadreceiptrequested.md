---
title: IsReadReceiptRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceiptRequested
api_type:
- schema
ms.assetid: 7ab6edd5-c7ed-4701-8de3-d7dc7ecfa9c2
description: IsReadReceiptRequested 要素は、アイテムの送信者が開封確認メッセージを要求するかどうかを示します。
ms.openlocfilehash: ff0c512ef23b315d4de1194432408f5b408029d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457789"
---
# <a name="isreadreceiptrequested"></a>IsReadReceiptRequested

**IsReadReceiptRequested**要素は、アイテムの送信者が開封確認メッセージを要求するかどうかを示します。 
  
```xml
<IsReadReceiptRequested/>
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
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼への返信を承諾するかを表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮の返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼への返信を拒否することを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの作成者への返信を含みます。  <br/> |
|[Replyalltoitem と](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。  <br/> |
|[Forwarditem と](forwarditem.md) <br/> |受信者に転送するための Exchange ストアアイテムが保存されています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議の取り消しに使用される response オブジェクト thatis を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、アイテムの受信者が開封確認メッセージを要求していることを示します。 
  
## <a name="remarks"></a>注釈

**IsReadReceiptRequested**が**true**の場合、 [isread](isread.md)を**true**に設定すると開封確認メッセージが送信されます。 受信者は、 **isread**プロパティを設定する前に、 [SuppressReadReceipt](suppressreadreceipt.md) response オブジェクトを送信することによって、開封確認メッセージを抑制することができます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

