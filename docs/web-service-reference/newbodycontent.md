---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: NewBodyContent 要素は、メッセージの新しい本文コンテンツを表します。
ms.openlocfilehash: 48f6a12e0492249d239196ca3be19857e34e0099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509517"
---
# <a name="newbodycontent"></a>NewBodyContent

**NewBodyContent 要素は**、メッセージの新しい本文コンテンツを表します。 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**BodyType** <br/> |メッセージの実際の本文の内容を表します。  <br/> |
   
#### <a name="bodytype-attribute"></a>BodyType 属性

|**値**|**説明**|
|:-----|:-----|
|**HTML** <br/> |すべてのボディを HTML に変換します。  <br/> |
|**Text** <br/> |すべての本文をプレーン テキストに変換します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |ストア内のアイテムの送信者に対する返信Exchangeします。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |送信者への返信と、ユーザー ストア内のアイテムの識別された受信者Exchangeします。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送Exchangeストア アイテムを格納します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議のキャンセルに使用される応答オブジェクトを表します。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信を含む。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、メッセージの新しい本文コンテンツを表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchangeサーバーの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

