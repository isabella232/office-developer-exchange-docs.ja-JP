---
title: dialString (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- dialString
api_type:
- schema
ms.assetid: d1e3cd23-48fe-4ebc-a5c5-2226d223f800
description: DialString 要素には、ダイヤルする電話番号の値が含まれています。
ms.openlocfilehash: f27934fa73ead75ab50e99a79c01cb6a1062e3d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760036"
---
# <a name="dialstring-um-web-service"></a>dialString (UM web サービス)

**DialString**要素には、ダイヤルする電話番号の値が含まれています。 
  
- [PlayOnPhone (UM web サービス)](playonphone-um-web-service.md) 
- [dialString (UM web サービス)](dialstring-um-web-service.md) 
- [PlayOnPhoneGreeting (UM web サービス)](playonphonegreeting-um-web-service.md) 
- [dialString (UM web サービス)](dialstring-um-web-service.md)
  
```xml
<dialString/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PlayOnPhone (UM web サービス)](playonphone-um-web-service.md) <br/> |電話でメッセージを再生する要求を定義します。  <br/> |
|[PlayOnPhoneGreeting (UM web サービス)](playonphonegreeting-um-web-service.md) <br/> |電話に応答メッセージを再生する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、有効なダイヤル番号を含める必要があります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [PlayOnPhone (UM web サービス)](playonphone-um-web-service.md)  
- [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)  
- [PlayOnPhoneGreeting (UM web サービス)](playonphonegreeting-um-web-service.md)  
- [PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)

