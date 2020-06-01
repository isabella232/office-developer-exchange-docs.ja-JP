---
title: IsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRead
api_type:
- schema
ms.assetid: 161455d5-a870-4c99-b2eb-c759c538f1bc
description: IsRead 要素は、メッセージが開封されたかどうかを示します。
ms.openlocfilehash: b6f2c2d72dd550f7ec8ed9a3415dc0715b3e376f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460373"
---
# <a name="isread"></a>IsRead

**Isread**要素は、メッセージが開封されたかどうかを示します。 
  
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
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
|[ConversationAction](conversationaction.md) <br/> |単一の会話に適用される1つのアクションが含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、メッセージが開封されたことを示します。 テキスト値が**false**の場合は、メッセージが開封されていないことを示します。 
  
## <a name="remarks"></a>注釈

[IsReadReceiptRequested](isreadreceiptrequested.md)が**true**の場合、 **isread**を**true**に設定すると開封確認メッセージが送信されます。 受信者は、 **isread**プロパティを設定する前に、 [SuppressReadReceipt](suppressreadreceipt.md) response オブジェクトを送信することによって、開封確認メッセージを抑制することができます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

