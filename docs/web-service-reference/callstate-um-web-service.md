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
description: CallState 要素には、呼び出しの状態を示す値が含まれています。
ms.openlocfilehash: 44614c460286ff49ebc2373263c1827c6be5cc08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454611"
---
# <a name="callstate-um-web-service"></a>CallState (UM web サービス)

**Callstate**要素には、呼び出しの状態を示す値が含まれています。 
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)
  
[CallState (UM web サービス)](callstate-um-web-service.md)
  
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
|[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md) <br/> |Getcallinfo 操作への応答を定義します[(UM web サービス)](getcallinfo-operation-um-web-service.md)。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- アイドル
    
- 接続中
    
- 警告
    
- Connected
    
- Disconnected
    
- 読み込ま
    
- 渡す
    
- しよう
    
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|スキーマ名  <br/> |メッセージ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (UM web サービス)](getcallinforesponse-um-web-service.md)

