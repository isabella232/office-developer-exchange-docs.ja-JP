---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: MimeContentUTF8 要素には、base64Binary 形式で表され、電子メール アドレスの国際化と [RFC6530] をサポートするオブジェクトの UTF-8 MIME ストリームが含まれます。
ms.openlocfilehash: f0ab38368d3a18be38f63c86183a238e2fd0a474
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540756"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

**MimeContentUTF8** 要素には、base64Binary 形式で表され、電子メール アドレスの国際化と [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt)をサポートするオブジェクトの UTF-8 MIME ストリームが含まれます。
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

この要素を使用する場合は、base64binary MIME ストリームを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

メッセージコンテンツは **、MimeContentUTF8** 値に格納される前に、次の 3 つのレベルのエンコードを通過します。 
  
1. メッセージ テキスト - 日本語の文字の iso-2022-jp などの本文エンコードです。
    
2. MIME ストリーム : **MimeContentUTF8** 要素のメッセージ テキストの UTF8 エンコード、または [MimeContent](mimecontent.md) 要素のメッセージ テキストの ASCII エンコードです。 
    
3. XML ドキュメント - これは常に MIME ストリームの base64 エンコード ASCII ストリームで、XML にとって意味のある ' などの文字は XML パーサーから非表示 \< になります。
    
各レベルは、その前のレベルとは独立しています。
  
**MimeContentUTF8** 要素には、アイテムに含まれる他のプロパティと同じデータが含まれている場合があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
### <a name="version-differences"></a>バージョンの相違点

この要素は、ビルド 15.00.0986.00 Exchangeのバージョンで使用できます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

