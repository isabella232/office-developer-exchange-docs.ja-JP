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
description: PlayOnPhoneResponse 要素は、PlayOnPhone の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832832"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (UM web サービス)

**PlayOnPhoneResponse**要素は、 [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)要求に対する応答を定義します。 
  
[PlayOnPhoneResponse (UM web サービス)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、 [GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)の要求または[切断の操作 (UM web サービス)](disconnect-operation-um-web-service.md)要求の[CallId (UM web サービス)](callid-um-web-service.md)の値を使用する呼び出しの id です。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)

