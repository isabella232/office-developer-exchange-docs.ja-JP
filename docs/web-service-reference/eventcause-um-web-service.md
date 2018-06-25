---
title: EventCause (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: EventCause 要素には、GetCallInfo 操作 (UM web サービス) 要求に対する応答で呼び出しイベントの原因を示す値が含まれています。
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760335"
---
# <a name="eventcause-um-web-service"></a>EventCause (UM web サービス)

**EventCause**要素には、 [GetCallInfo 操作 (UM web サービス](getcallinfo-operation-um-web-service.md)要求への応答で呼び出しイベントの原因を示す値が含まれています。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
[EventCause (UM web サービス)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md) <br/> |[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- なし
    
- UserBusy
    
- NoAnswer
    
- その他
    
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)

