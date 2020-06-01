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
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466858"
---
# <a name="newbodycontent"></a>NewBodyContent

**Newbodycontent**要素は、メッセージの新しい本文の内容を表します。 
  
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
|**HTML** <br/> |すべての本文を HTML に変換します。  <br/> |
|**Text** <br/> |すべての本文をテキスト形式に変換します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの送信者への返信を含みます。  <br/> |
|[Replyalltoitem と](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの送信者および特定の受信者への返信を含みます。  <br/> |
|[Forwarditem と](forwarditem.md) <br/> |受信者に転送するための Exchange ストアアイテムが保存されています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議の取り消しに使用される response オブジェクトを表します。  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |投稿アイテムへの返信を含みます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

Text 値は、メッセージの新しい本文の内容を表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange サーバーの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

