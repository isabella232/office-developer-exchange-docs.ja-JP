---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Action 要素には、ConversationId 要素で指定された会話に対して実行するアクションが含まれる。
ms.openlocfilehash: e75d9d5df75894d1de9831b0022269e7ace4fa63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514894"
---
# <a name="action-conversationactiontypetype"></a>Action (ConversationActionTypeType)

**Action 要素には、ConversationId** 要素で指定された会話に対して実行する [アクションが含](conversationid.md)まれる。 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [Action (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
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

Action 要素のテキスト **値は** 、会話に対して実行されるアクションを示します。 使用できるテキスト値と対応するアクションを次に示します。 
  
- **AlwaysCategorize** - 会話の現在のアイテムと新しいアイテムは [、Categories](categories-ex15websvcsotherref.md) 要素で識別されるカテゴリで自動的に設定されます。 
    
- **AlwaysDelete** - 会話内の現在のアイテムと新しいアイテムは自動的に削除されます。 削除モードは [DeleteType 要素によって設定](deletetype.md) されます。 
    
- **AlwaysMove** - 会話内の現在のアイテムと新しいアイテムは [、DestinationFolderId](destinationfolderid.md) 要素によって識別されるフォルダーに自動的に移動されます。 
    
- **[削除** ] - 会話内の現在のアイテムが削除されます。 会話内の後続のアイテムは削除されません。 削除モードは [DeleteType 要素によって設定](deletetype.md) されます。 
    
- **Move** - スレッド内の現在のアイテムは [、DestinationFolderId](destinationfolderid.md) 要素によって識別されるフォルダーに移動されます。 会話内の後続のアイテムは移動されません。 
    
- **Copy** - スレッド内の現在のアイテムは [、DestinationFolderId](destinationfolderid.md) 要素によって識別されるフォルダーにコピーされます。 会話内の後続のアイテムはコピーされません。 
    
- **SetReadState** - 会話内の現在のアイテムの読み取り状態が設定されます。 読み取り状態は [IsRead 要素によって設定](isread.md) されます。 
    
- **フラグ** - 会話内の現在のアイテムには、Flag 要素で定義されたフラグが [設定](flag.md) されます。 
    
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

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

