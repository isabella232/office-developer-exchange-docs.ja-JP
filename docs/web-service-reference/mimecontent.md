---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: MimeContent 要素には、base64Binary 形式で表され、[RFC2045] をサポートするオブジェクトの ASCII MIME ストリームが含まれます。
ms.openlocfilehash: 43040f241008010620ff4f1018cc5410a7a00e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542072"
---
# <a name="mimecontent"></a>MimeContent

**MimeContent** 要素には、base64Binary 形式で表され [、[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt)をサポートするオブジェクトの ASCII MIME ストリームが含まれます。
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**CharacterSet** <br/> |設定すると、この属性の値はサーバーによって無視されます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[CalendarItem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [アイテム](item.md)  | [MeetingCancellation](meetingcancellation.md)  | [MeetingMessage](meetingmessage.md)  | [MeetingRequest](meetingrequest.md)  | [MeetingResponse](meetingresponse.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [RemoveItem](removeitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、base64Binary MIME ストリームを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

メッセージのコンテンツは **、MimeContent** 値に格納される前に、次の 3 つのレベルのエンコードを行います。 
  
1. メッセージ テキスト - 日本語の文字の iso-2022-jp などの本文エンコードです。
    
2. MIME ストリーム - MimeContent 要素のメッセージ テキストの ASCII エンコード、または[MimeContentUTF8](mimecontentutf8.md)要素のメッセージ テキストの UTF8 エンコードです。  
    
3. XML ドキュメント - これは常に MIME ストリームの base64 エンコード ASCII ストリームで、XML にとって意味のある ' などの文字は XML パーサーから非表示 \< になります。
    
各レベルは、その前のレベルとは独立しています。
  
**MimeContent 要素には**、アイテムに含まれる他のプロパティと同じデータが含まれている場合があります。 
  
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

