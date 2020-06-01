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
description: GetCallInfoResponse 要素は、GetCallInfo 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461206"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (UM web サービス)

**GetCallInfoResponse**要素は、 [Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求への応答を定義します。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|CallState  <br/> |[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した通話の状態を示す値を格納します。  <br/> |
|イベント原因  <br/> |[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した呼び出しに対するイベントの原因を示す値を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[CallState (UM web サービス)](callstate-um-web-service.md)
  
[EventCause (UM web サービス)](eventcause-um-web-service.md)

