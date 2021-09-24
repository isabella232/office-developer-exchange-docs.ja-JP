---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: ConversationLastSyncTime 要素には、会話が最後に同期された日時が含まれる。 この要素は、指定した時間まで受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。
ms.openlocfilehash: d71f455fa00226c84b157ba04b391b80df95f1bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536669"
---
# <a name="conversationlastsynctime"></a>ConversationLastSyncTime

**ConversationLastSyncTime** 要素には、会話が最後に同期された日時が含まれる。 この要素は、指定した時間まで受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ConversationLastSyncTime](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 **xs:dateTime**
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

**ConversationLastSyncTime のテキスト値は**、会話が最後に同期された時刻を示します。 
  
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

