---
title: (UM web サービス) に接続を切断します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: 切断要素は、呼び出しの切断要求を定義します。
ms.openlocfilehash: 764532bdadd69caaa68406c84277197def3160af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760093"
---
# <a name="disconnect-um-web-service"></a>(UM web サービス) に接続を切断します。

**切断**要素は、呼び出しの切断要求を定義します。 
  
- [(UM web サービス) に接続を切断します。](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 **complexType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CallId (UM web サービス)](callid-um-web-service.md) <br/> |切断するのには、呼び出しの id。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [操作 (UM web サービス) に接続を切断します。](disconnect-operation-um-web-service.md)  
- [PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md) 
- [PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)  
- [CallId (UM web サービス)](callid-um-web-service.md)

