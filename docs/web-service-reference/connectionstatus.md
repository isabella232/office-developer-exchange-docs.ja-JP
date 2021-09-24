---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: ConnectionStatus 要素は、ストリーミング サブスクリプションの状態のテキストの説明を提供します。
ms.openlocfilehash: 05ff80ac3e6c3c8bf1341a179a14c9d052c9947f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536852"
---
# <a name="connectionstatus"></a>ConnectionStatus

**ConnectionStatus 要素** は、ストリーミング サブスクリプションの状態のテキストの説明を提供します。 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 **ConnectionStatusType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |1 つの [GetStreamingEvents](getstreamingevents-operation.md) 操作要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素で使用できるテキスト値を次に示します。
  
- OK
    
- クローズ
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetStreamingEvents の操作](getstreamingevents-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

