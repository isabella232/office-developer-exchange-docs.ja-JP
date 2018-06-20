---
title: MissedCallNotificationEnabled (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- MissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 8e6bf0b1-ff76-474c-ac0f-621b6ab89212
description: MissedCallNotificationEnabled 要素には、GetUMProperties (UM web サービス) の操作の要求への応答の不在着信通知が有効になっているかどうかを示す値が含まれています。
ms.openlocfilehash: 6bebbe6eeb40a259f0c51355a3fea838e8671706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832477"
---
# <a name="missedcallnotificationenabled-um-web-service"></a>MissedCallNotificationEnabled (UM web サービス)

**MissedCallNotificationEnabled**要素には、 [GetUMProperties 操作 (UM web サービス](getumproperties-operation-um-web-service.md)要求への応答の不在着信通知が有効になっているかどうかを示す値が含まれています。 
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)
  
[MissedCallNotificationEnabled (UM web サービス)](missedcallnotificationenabled-um-web-service.md)
  
```xml
<MissedCallNotificationEnabled/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md) <br/> |[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値のテキスト値は、必要があります。 指定可能な値は次のいずれかです。
  
- True
    
- False
    
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)
  
[SetMissedCallNotificationEnabled 操作 (UM web サービス)](setmissedcallnotificationenabled-operation-um-web-service.md)

