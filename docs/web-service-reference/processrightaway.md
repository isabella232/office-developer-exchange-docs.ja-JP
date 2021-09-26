---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: ProcessRightAway 要素は、アクションがサーバーで処理を開始した直後に応答が送信されるかどうか、またはアクションが完了した後に応答が送信されるかどうかを示します。 要求されたアクションに非同期で送信される応答には、この要素が存在する必要があります。
ms.openlocfilehash: 5546bbff4e1e1ef17eee94f1f42492fbf070fe59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542996"
---
# <a name="processrightaway"></a>ProcessRightAway

**ProcessRightAway** 要素は、アクションがサーバーで処理を開始した直後に応答が送信されるかどうか、またはアクションが完了した後に応答が送信されるかどうかを示します。 要求されたアクションに非同期で送信される応答には、この要素が存在する必要があります。 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ProcessRightAway](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |1 つの会話に適用する 1 つのアクションが含まれる。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が **true の場合** は、アクションがサーバーで処理を開始するとすぐに応答が送信されます。 テキスト値 **false** は、アクションが完了した後に応答が送信されます。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ApplyConversationAction 操作](applyconversationaction-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

