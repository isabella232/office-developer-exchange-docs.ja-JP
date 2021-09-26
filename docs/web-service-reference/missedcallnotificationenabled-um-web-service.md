---
title: MissedCallNotificationEnabled (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- MissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 8e6bf0b1-ff76-474c-ac0f-621b6ab89212
description: MissedCallNotificationEnabled 要素には、GetUMProperties 操作 (UM Web サービス) 要求に対する応答で、欠けている呼び出し通知が有効になっているかどうかを示す値が含まれる。
ms.openlocfilehash: 0566312db672b3795e5f163a35e4c31ae6b26af4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542044"
---
# <a name="missedcallnotificationenabled-um-web-service"></a>MissedCallNotificationEnabled (UM Web サービス)

**MissedCallNotificationEnabled** 要素には [、GetUMProperties 操作 (UM Web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答で、欠けている呼び出し通知が有効になっているかどうかを示す値が含まれる。 
  
[GetUMPropertiesResponse (UM Web サービス)](getumpropertiesresponse-um-web-service.md)
  
[MissedCallNotificationEnabled (UM Web サービス)](missedcallnotificationenabled-um-web-service.md)
  
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
  
[SetMissedCallNotificationEnabled 操作 (UM Web サービス)](setmissedcallnotificationenabled-operation-um-web-service.md)

