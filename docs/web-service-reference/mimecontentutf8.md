---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: MimeContentUTF8 要素には、base64Binary の形式で表されるオブジェクトの UTF-8 の MIME ストリームが含まれているし、e メール アドレスの国際化をサポートし、[RFC6530]。
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832466"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

**MimeContentUTF8**要素には、base64Binary の形式で表され、 [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt)電子メール アドレスの国際化をサポートしているオブジェクトの UTF-8 の MIME ストリームが含まれています。
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**文字セット** <br/> |かどうか、この属性の値は無視されます、サーバーがします。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[カレンダー項目](calendaritem.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md) | [アイテム](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md) | [メッセージ](message-ex15websvcsotherref.md) | [での RemoveItem](removeitem.md) | [タスク](task.md)
  
## <a name="text-value"></a>テキスト値

Base64binary の MIME ストリームを表すテキスト値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

メッセージの内容は次の 3 つのレベルの**MimeContentUTF8**の値に格納される前にエンコードします。 
  
1. メッセージ テキスト、本文のエンコーディングには、iso 2022 の jp 日本語の文字などは、これ。
    
2. MIME ストリーム-これは、UTF8 エンコーディングのメッセージ要素のテキスト、 **MimeContentUTF8** 、または[MimeContent](mimecontent.md)要素のメッセージ テキストの ASCII エンコードします。 
    
3. XML ドキュメント-これは、常に base64 でエンコードされた ASCII ストリーム、MIME ストリームの場所などの文字 '\<'、XML パーサーから非表示には、xml では、意味のあります。
    
各レベルでは、その前にあるレベルの独立しています。
  
**MimeContentUTF8**要素には、アイテムが返されるその他のプロパティが含まれている同じデータが含まれて可能性があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
### <a name="version-differences"></a>バージョンの相違点

この要素は、Exchange のビルド 15.00.0986.00 以降のバージョンで利用できます。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

