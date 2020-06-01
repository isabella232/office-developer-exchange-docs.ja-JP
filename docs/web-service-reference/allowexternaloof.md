---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: AllowExternalOof 要素には、外部の不在時 (OOF) メッセージが送信されるユーザーを識別する値が含まれています。
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464813"
---
# <a name="allowexternaloof"></a>AllowExternalOof

**AllowExternalOof**要素には、外部の不在時 (OOF) メッセージが送信されるユーザーを識別する値が含まれています。 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの OOF 設定が含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素にはテキスト値が必要です。 次の表に、この要素で使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|**なし** <br/> |メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の不在時メッセージ応答を受信しません。  <br/> |
|**一般的** <br/> |メールボックスユーザーの組織外の電子メール送信者がユーザーにメッセージを送信すると、送信者がユーザーの Exchange ストアの連絡先リストにある場合にのみ、外部の OOF メッセージ応答が受信されます。  <br/> |
|**All** <br/> |メールボックスユーザーの組織外の電子メール送信者は、ユーザーにメッセージを送信すると、外部の OOF メッセージ応答を受信します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [Externalaudience](externalaudience.md)要素と同じ型を共有します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md) 
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

