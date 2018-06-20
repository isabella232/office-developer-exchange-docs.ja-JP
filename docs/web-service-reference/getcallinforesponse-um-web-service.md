---
title: GetCallInfoResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: GetCallInfoResponse 要素は、GetCallInfo の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760653"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (UM web サービス)

**GetCallInfoResponse**要素は、 [GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答を定義します。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|CallState  <br/> |呼び出しのステータスを示す値が含まれています[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求します。  <br/> |
|EventCause  <br/> |呼び出しのイベントの原因を示す値が含まれています[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[CallState (UM web サービス)](callstate-um-web-service.md)
  
[EventCause (UM web サービス)](eventcause-um-web-service.md)

