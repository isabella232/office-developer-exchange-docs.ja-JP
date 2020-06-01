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
description: MissedCallNotificationEnabled 要素には、GetUMProperties 操作 (UM web サービス) 要求に対する応答で不在着信通知が有効になっているかどうかを示す値が含まれています。
ms.openlocfilehash: e2f18027c56be1408c27d5f687fe90f8ffd724db
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468657"
---
# <a name="missedcallnotificationenabled-um-web-service"></a>MissedCallNotificationEnabled (UM web サービス)

**MissedCallNotificationEnabled**要素には、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答で不在着信通知が有効になっているかどうかを示す値が含まれています。 
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)
  
[MissedCallNotificationEnabled (UM web サービス)](missedcallnotificationenabled-um-web-service.md)
  
```xml
<MissedCallNotificationEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md) <br/> |[Getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求への応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール型のテキスト値が必要です。 指定可能な値は次のいずれかです。
  
- True
    
- False
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)
  
[SetMissedCallNotificationEnabled 操作 (UM web サービス)](setmissedcallnotificationenabled-operation-um-web-service.md)

