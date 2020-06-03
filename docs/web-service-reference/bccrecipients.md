---
title: BccRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipients
api_type:
- schema
ms.assetid: c4e05168-d36b-4740-a526-4b7da53553c1
description: BccRecipients 要素は、電子メールメッセージのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。
ms.openlocfilehash: 96070415c6d92a893f6c560884d9d191c7d5f15b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529505"
---
# <a name="bccrecipients"></a>BccRecipients

**Bccrecipients**要素は、電子メールメッセージのブラインドカーボンコピー (bcc) を受信する受信者のコレクションを表します。 
  
```xml
<BccRecipients>
   <Mailbox/>
</BccRecipients>
```

 **Arrayof受信者 Stype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。  <br/> |
   
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
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮承諾の返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼への返信を拒否することを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの作成者への返信を含みます。  <br/> |
|[Replyalltoitem と](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。  <br/> |
|[Forwarditem と](forwarditem.md) <br/> |受信者に転送するための Exchange ストアアイテムが保存されています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議の取り消しに使用される response オブジェクトを表します。  <br/> |
   
## <a name="remarks"></a>注釈

FindItem 要求を使用して**Bccrecipients**れたイベントを取得することはできません。 GetItem 要求を使用して、 **Bccrecipients**イベントを取得します。
  
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

