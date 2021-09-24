---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: AllowExternalOof 要素には、外部外部アウト オブ Office (OOF) メッセージの送信先を識別する値が含まれます。
ms.openlocfilehash: 7d2e34797af8a9e9d11570a5ea2e618db7630f0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523225"
---
# <a name="allowexternaloof"></a>AllowExternalOof

**AllowExternalOof** 要素には、外部外部アウト オブ Office (OOF) メッセージの送信先を識別する値が含まれます。 
  
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
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの OOF 設定が含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には、テキスト値が必要です。 次の表に、この要素に使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|**なし** <br/> |ユーザーにメッセージを送信するメールボックス ユーザーの組織外の電子メール送信者は、外部の OOF メッセージ応答を受信しません。  <br/> |
|**既知** <br/> |ユーザーにメッセージを送信するメールボックス ユーザーの組織外の電子メール送信者は、送信者がユーザーのストア連絡先リスト内にある場合にのみ、外部 OOF メッセージ応答Exchange受信します。  <br/> |
|**All** <br/> |ユーザーにメッセージを送信するメールボックス ユーザーの組織外の電子メール送信者は、外部の OOF メッセージ応答を受信します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は [ExternalAudience 要素と同じ型を共有](externalaudience.md) します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md) 
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

