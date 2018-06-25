---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: NewBodyContent 要素は、メッセージの新しい本文の内容を表します。
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832516"
---
# <a name="newbodycontent"></a>NewBodyContent

**NewBodyContent**要素は、メッセージの新しい本文の内容を表します。 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**BodyType** <br/> |メッセージの実際の本文の内容を表します。  <br/> |
   
#### <a name="bodytype-attribute"></a>BodyType 属性

|**値**|**説明**|
|:-----|:-----|
|**HTML** <br/> |すべての本文を HTML に変換します。  <br/> |
|**Text** <br/> |すべての本文をテキスト形式に変換します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの送信者への返信が含まれています。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送するのには、Exchange ストアの項目が含まれています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議をキャンセルするために使用される応答オブジェクトを表します。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、新しいメッセージの本文の内容を表します。
  
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

