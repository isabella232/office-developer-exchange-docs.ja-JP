---
title: OofStatus (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: OofStatus 要素には、その indicaties GetUMProperties 操作 (UM web サービス) 要求を行っているユーザーのメッセージングの Office を統合の状態の値が含まれています。
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832650"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (UM web サービス)

**OofStatus**要素には、その indicaties [GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求を行っているユーザーのメッセージングの Office を統合の状態の値が含まれています。 
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (UM web サービス)](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
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
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)

