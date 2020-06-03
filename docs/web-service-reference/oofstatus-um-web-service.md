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
description: OofStatus 要素には、GetUMProperties 操作 (UM web サービス) 要求を作成しているユーザーに対して、ユニファイドメッセージングの不在状態を indicaties する値が含まれています。
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460576"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (UM web サービス)

**Oofstatus**要素には、 [getumproperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求を作成しているユーザーに対して、ユニファイドメッセージングの不在状態を indicaties する値が含まれています。 
  
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
  
[GetUMPropertiesResponse (UM web サービス)](getumpropertiesresponse-um-web-service.md)

