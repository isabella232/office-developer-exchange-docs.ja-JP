---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: MimeContentUTF8 要素には、base64Binary 形式で表され、電子メールアドレスの国際化および [RFC6530] をサポートするオブジェクトの UTF-8 MIME ストリームが含まれています。
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530430"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

**MimeContentUTF8**要素には、base64Binary 形式で表され、電子メールアドレスの国際化および[[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt)をサポートするオブジェクトの utf-8 MIME ストリームが含まれています。
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

この要素を使用する場合は、base64binary MIME ストリームを表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

メッセージコンテンツは、 **MimeContentUTF8**値に格納される前に、次の3つのエンコードレベルで行われます。 
  
1. メッセージテキスト: これは、日本語の文字の iso-2022-jp などの本文のエンコードです。
    
2. MIME ストリーム— **MimeContentUTF8**要素のメッセージテキストの UTF8 エンコード、または[MimeContent](mimecontent.md)要素のメッセージテキストの ASCII エンコーディングです。 
    
3. XML ドキュメント—これは常に MIME ストリームの base64 でエンコードされた ASCII ストリームです。これは、XML に意味のある ' ' のような文字 \< が xml パーサーに表示されません。
    
各レベルは、その前にあるレベルから独立しています。
  
**MimeContentUTF8**要素には、アイテムによって返されるその他のプロパティと同じデータが含まれている場合があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
### <a name="version-differences"></a>バージョンの相違点

この要素は、build 15.00.0986.00 以降のバージョンの Exchange で使用できます。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

