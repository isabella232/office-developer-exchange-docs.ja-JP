---
title: 会話 (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: テーマ要素は、GetConversationItems 応答で返される 1 つのテーマを表します。
ms.openlocfilehash: ef56e26fda7d2bf6556069355918aa576ce14cb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759746"
---
# <a name="conversation-conversationrequesttype"></a>会話 (ConversationRequestType)

**テーマ**要素は、 **GetConversationItems**応答で返される 1 つのテーマを表します。 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ConversationId](conversationid.md) | [同期状態 (base64Binary)](syncstate-base64binary.md)
  
### <a name="parent-elements"></a>親要素

[スレッド](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

