---
title: GetCallInfoResponse (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: GetCallInfoResponse 要素は、GetCallInfo 操作 (UM Web サービス) 要求への応答を定義します。
ms.openlocfilehash: 4b631bdee87e57c1612e906c725adabb9f9ce63e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526190"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (UM Web サービス)

**GetCallInfoResponse** 要素は [、GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)要求への応答を定義します。 
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)
  
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
|CallState  <br/> |[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した呼び出しの状態を示す値を格納します。  <br/> |
|イベント理由  <br/> |[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した呼び出しのイベントの原因を示す値を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)
  
[CallState (UM Web サービス)](callstate-um-web-service.md)
  
[EventCause (UM Web サービス)](eventcause-um-web-service.md)

