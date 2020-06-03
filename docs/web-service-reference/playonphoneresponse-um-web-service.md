---
title: PlayOnPhoneResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: PlayOnPhoneResponse 要素は、PlayOnPhone 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: ddb9cc9a8feaeb476e6502339fdc74d024797b9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459617"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (UM web サービス)

**PlayOnPhoneResponse**要素は、 [playonphone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)要求への応答を定義します。 
  
[PlayOnPhoneResponse (UM web サービス)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、 [Getcallinfo 操作 (um web](getcallinfo-operation-um-web-service.md)サービス) 要求または[切断操作 (um web サービス)](disconnect-operation-um-web-service.md)要求の[callid (um web サービス)](callid-um-web-service.md)の値として使用する呼び出し識別子です。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)

