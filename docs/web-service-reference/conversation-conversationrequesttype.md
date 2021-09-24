---
title: Conversation (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: Conversation 要素は、GetConversationItems 応答で返される 1 つの会話を表します。
ms.openlocfilehash: 9c7faf9c06c1476bca688e831f452e711a89f10f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533894"
---
# <a name="conversation-conversationrequesttype"></a>Conversation (ConversationRequestType)

**Conversation 要素** は **、GetConversationItems** 応答で返される 1 つの会話を表します。 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ConversationId](conversationid.md)  | [SyncState (base64Binary)](syncstate-base64binary.md)
  
### <a name="parent-elements"></a>親要素

[会話](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

