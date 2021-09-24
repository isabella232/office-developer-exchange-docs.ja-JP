---
title: PlayOnPhoneGreetingResponse (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreetingResponse
api_type:
- schema
ms.assetid: 7189d69a-9288-4fc8-8d78-4977ee1a7253
description: PlayOnPhoneGreetingResponse 要素は、PlayOnPhoneGreeting 操作 (UM Web サービス) 要求への応答を定義します。
ms.openlocfilehash: f8370d8ed93cc18eb29df100e68bddaa22c35fca
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512633"
---
# <a name="playonphonegreetingresponse-um-web-service"></a>PlayOnPhoneGreetingResponse (UM Web サービス)

**PlayOnPhoneGreetingResponse** 要素は [、PlayOnPhoneGreeting 操作 (UM Web サービス)](playonphonegreeting-operation-um-web-service.md)要求への応答を定義します。 
  
[PlayOnPhoneGreetingResponse (UM Web サービス)](playonphonegreetingresponse-um-web-service.md)
  
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

テキスト値は必須です。 テキスト値には[、GetCallInfo](getcallinfo-operation-um-web-service.md)操作 (UM Web サービス) 要求または切断操作[(UM Web](disconnect-operation-um-web-service.md)サービス) 要求の[CallId (UM](callid-um-web-service.md) Web サービス) の値に使用する値が含まれる。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[PlayOnPhoneGreeting 操作 (UM Web サービス)](playonphonegreeting-operation-um-web-service.md)
  
[CallId (UM Web サービス)](callid-um-web-service.md)
  
[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)
  
[切断操作 (UM Web サービス)](disconnect-operation-um-web-service.md)

