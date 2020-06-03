---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: MimeContent 要素には、base64Binary 形式で表され、[RFC2045] をサポートするオブジェクトの ASCII MIME ストリームが含まれています。
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530437"
---
# <a name="mimecontent"></a>MimeContent

**MimeContent**要素には、base64Binary 形式で表され、 [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt)をサポートするオブジェクトの ASCII MIME ストリームが含まれています。
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**CharacterSet** <br/> |設定した場合、この属性の値はサーバーによって無視されます。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Calendaritem](calendaritem.md)  | [連絡先](contact.md)  | [DistributionList](distributionlist.md)  | [アイテム](item.md)  | [会議のキャンセル](meetingcancellation.md)  | [会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [メッセージ](message-ex15websvcsotherref.md)  | [Removeitem](removeitem.md)  | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、base64Binary MIME ストリームを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

メッセージコンテンツは、 **MimeContent**値に格納される前に、次の3つのエンコードレベルで行われます。 
  
1. メッセージテキスト: これは、日本語の文字の iso-2022-jp などの本文のエンコードです。
    
2. MIME ストリーム—これは、 **MimeContent**要素のメッセージテキストの ASCII エンコード、または[MimeContentUTF8](mimecontentutf8.md)要素のメッセージテキストの UTF8 エンコードです。 
    
3. XML ドキュメント—これは常に MIME ストリームの base64 でエンコードされた ASCII ストリームです。これは、XML に意味のある ' ' のような文字 \< が xml パーサーに表示されません。
    
各レベルは、その前にあるレベルから独立しています。
  
**MimeContent**要素には、アイテムによって返されるその他のプロパティと同じデータが含まれている場合があります。 
  
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

