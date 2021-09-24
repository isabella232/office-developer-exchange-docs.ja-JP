---
title: OofStatus (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: OofStatus 要素には、GetUMProperties 操作 (UM Web サービス) 要求を行っているユーザーのユニファイド メッセージングが Office から外れる状態を示す値が含まれている。
ms.openlocfilehash: 4e899317defdb4ac4c27c3fdc17d7b7222dff6a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539270"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (UM Web サービス)

**OofStatus** 要素には [、GetUMProperties 操作 (UM Web サービス)](getumproperties-operation-um-web-service.md)要求を行っているユーザーのユニファイド メッセージングの Office 状態を示す値が含まれる。 
  
[GetUMPropertiesResponse (UM Web サービス)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (UM Web サービス)](oofstatus-um-web-service.md)
  
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
|[GetUMPropertiesResponse (UM Web サービス)](getumpropertiesresponse-um-web-service.md) <br/> |[GetUMProperties 操作 (UM Web サービス) 要求への応答を定義](getumproperties-operation-um-web-service.md)します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール型 (Boolean) のテキスト値が必要です。 指定可能な値は次のいずれかです。
  
- True
    
- False
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUMProperties 操作 (UM Web サービス)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (UM Web サービス)](getumpropertiesresponse-um-web-service.md)

