---
title: EventCause (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: EventCause 要素には、GetCallInfo 操作 (UM Web サービス) 要求への応答で呼び出しイベントの原因を示す値が含まれる。
ms.openlocfilehash: 203cefa1a70294bec4d6f4b41aa157da6e639fce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546575"
---
# <a name="eventcause-um-web-service"></a>EventCause (UM Web サービス)

**EventCause 要素** には [、GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)要求への応答で呼び出しイベントの原因を示す値が含まれる。 
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)
  
[EventCause (UM Web サービス)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEvent 理由**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md) <br/> |[GetCallInfo 操作 (UM Web サービス) 要求への応答を定義](getcallinfo-operation-um-web-service.md)します。  <br/> |
   
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
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)

