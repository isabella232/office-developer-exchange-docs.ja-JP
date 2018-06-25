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
description: AllowExternalOof 要素には、外部の Office (OOF) メッセージを送信するを識別する値が含まれています。
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759316"
---
# <a name="allowexternaloof"></a>AllowExternalOof

**AllowExternalOof**要素には、外部の Office (OOF) メッセージを送信するを識別する値が含まれています。 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |応答結果とユーザーの不在時の設定が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、この要素の必要があります。 次の表は、この要素の有効な値を一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|**None** <br/> |メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者は、外部の OOF メッセージの応答を受信しません。  <br/> |
|**呼ばれる** <br/> |メールボックス ユーザーの組織の外部ユーザーへのメッセージのみが表示されます、外部の OOF メッセージ応答送信者がユーザーの Exchange の場合に送信したメールの送信者は、連絡先リストを保存します。  <br/> |
|**All** <br/> |メールボックス ユーザーの組織外のユーザーにメッセージを送信するメールの送信者が外部の OOF メッセージの応答を受け取ります。  <br/> |
   
## <a name="remarks"></a>備考

この要素は、 [ExternalAudience](externalaudience.md)要素と同じ型を共有します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md) 
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

