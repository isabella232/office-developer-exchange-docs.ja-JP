---
title: CallState (UM Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: CallState 要素には、呼び出しの状態を示す値が含まれる。
ms.openlocfilehash: 9435124e98cfb75beab5917c1e832096ca193e0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519969"
---
# <a name="callstate-um-web-service"></a>CallState (UM Web サービス)

**CallState 要素** には、呼び出しの状態を示す値が含まれる。 
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)
  
[CallState (UM Web サービス)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md) <br/> |[GetCallInfo 操作 (UM Web サービス) への応答を定義します](getcallinfo-operation-um-web-service.md)。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- アイドル状態
    
- 接続中
    
- アラート
    
- 接続しました
    
- Disconnected
    
- 受信
    
- 転送
    
- 転送
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM Web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM Web サービス)](getcallinforesponse-um-web-service.md)

