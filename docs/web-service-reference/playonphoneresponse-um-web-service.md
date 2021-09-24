---
title: PlayOnPhoneResponse (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: PlayOnPhoneResponse 要素は、PlayOnPhone 操作 (UM Web サービス) 要求への応答を定義します。
ms.openlocfilehash: 9c2893837a1bc9c4836dc3cab6fb14e0d1fd611b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516525"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (UM Web サービス)

**PlayOnPhoneResponse** 要素は [、PlayOnPhone 操作 (UM Web サービス)](playonphone-operation-um-web-service.md)要求への応答を定義します。 
  
[PlayOnPhoneResponse (UM Web サービス)](playonphoneresponse-um-web-service.md)
  
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

テキスト値は必須です。 テキスト値は[、GetCallInfo](getcallinfo-operation-um-web-service.md)操作 (UM Web サービス) 要求または切断操作[(UM Web](disconnect-operation-um-web-service.md)サービス) 要求の[CallId (UM](callid-um-web-service.md) Web サービス) の値に使用する呼び出し識別子です。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[PlayOnPhone 操作 (UM Web サービス)](playonphone-operation-um-web-service.md)

