---
title: 切断 (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: Disconnect 要素は、呼び出しを切断する要求を定義します。
ms.openlocfilehash: 6aaff910d85a963a926e7c2a74a91963b120392c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538374"
---
# <a name="disconnect-um-web-service"></a>切断 (UM Web サービス)

**Disconnect 要素は**、呼び出しを切断する要求を定義します。 
  
- [切断 (UM Web サービス)](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 **complexType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CallId (UM Web サービス)](callid-um-web-service.md) <br/> |切断する呼び出しの識別子。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [切断操作 (UM Web サービス)](disconnect-operation-um-web-service.md)  
- [PlayOnPhone 操作 (UM Web サービス)](playonphone-operation-um-web-service.md) 
- [PlayOnPhoneGreeting 操作 (UM Web サービス)](playonphonegreeting-operation-um-web-service.md)  
- [CallId (UM Web サービス)](callid-um-web-service.md)

