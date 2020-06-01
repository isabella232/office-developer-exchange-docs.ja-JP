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
description: EventCause 要素には、GetCallInfo 操作 (UM web サービス) 要求に対する応答の呼び出しイベントの原因を示す値が含まれています。
ms.openlocfilehash: 9d49fd4b16236d0dd87889fbbd039f2e271a5968
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458678"
---
# <a name="eventcause-um-web-service"></a>EventCause (UM web サービス)

**Eventcause**要素には、 [Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答の呼び出しイベントの原因を示す値が含まれています。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
[EventCause (UM web サービス)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md) <br/> |[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求への応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- なし
    
- UserBusy
    
- NoAnswer
    
- その他
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)

