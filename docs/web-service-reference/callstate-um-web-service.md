---
title: CallState (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: CallState 要素には、呼び出しのステータスを示す値が含まれています。
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759605"
---
# <a name="callstate-um-web-service"></a>CallState (UM web サービス)

**CallState**要素には、呼び出しのステータスを示す値が含まれています。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
[CallState (UM web サービス)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md) <br/> |[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)への応答を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- アイドル
    
- Connecting
    
- 警告を表示
    
- Connected
    
- Disconnected
    
- 受信
    
- 転送します。
    
- 転送
    
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)

