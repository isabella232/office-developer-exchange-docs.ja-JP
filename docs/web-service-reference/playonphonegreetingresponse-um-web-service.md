---
title: PlayOnPhoneGreetingResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreetingResponse
api_type:
- schema
ms.assetid: 7189d69a-9288-4fc8-8d78-4977ee1a7253
description: PlayOnPhoneGreetingResponse 要素は、Playon電話案内応答操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: ca448860ef0e59607f73421c71d9c8f75c740773
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528854"
---
# <a name="playonphonegreetingresponse-um-web-service"></a>PlayOnPhoneGreetingResponse (UM web サービス)

**PlayOnPhoneGreetingResponse**要素は、 [Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)要求への応答を定義します。 
  
[PlayOnPhoneGreetingResponse (UM web サービス)](playonphonegreetingresponse-um-web-service.md)
  
```xml
<PlayOnPhoneGreetingResponse />
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

テキスト値は必須です。 テキスト値には、 [Getcallinfo 操作 (um web](getcallinfo-operation-um-web-service.md)サービス) 要求または[切断操作 (um web サービス)](disconnect-operation-um-web-service.md)要求の[callid (um web サービス)](callid-um-web-service.md)の値として使用する値が含まれています。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)
  
[CallId (UM web サービス)](callid-um-web-service.md)
  
[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[Disconnect 操作 (UM web サービス)](disconnect-operation-um-web-service.md)

