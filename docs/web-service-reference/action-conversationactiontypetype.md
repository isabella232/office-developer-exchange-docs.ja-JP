---
title: アクション (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Action 要素には、ConversationId 要素によって指定された会話に対して実行するアクションが含まれています。
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527545"
---
# <a name="action-conversationactiontypetype"></a>アクション (ConversationActionTypeType)

**Action**要素には、 [ConversationId](conversationid.md)要素によって指定された会話に対して実行するアクションが含まれています。 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [アクション (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
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
|[ConversationAction](conversationaction.md) <br/> |単一の会話に適用される1つのアクションが含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Action**要素のテキスト値は、会話に対して実行されるアクションを示します。 可能なテキスト値とそれに対応するアクションを次に示します。 
  
- **AlwaysCategorize** -会話内の現在のアイテムと新しいアイテムは、 [categories](categories-ex15websvcsotherref.md)要素で識別されるカテゴリで自動的に設定されます。 
    
- **Always delete** -現在のアイテムとスレッドの新しいアイテムは自動的に削除されます。 削除モードは[Deletetype](deletetype.md)要素によって設定されます。 
    
- **Always move** -現在のアイテムとスレッド内の新しいアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーに自動的に移動されます。 
    
- **Delete** -スレッド内の現在のアイテムは削除されます。 スレッド内の後続のアイテムは削除されません。 削除モードは[Deletetype](deletetype.md)要素によって設定されます。 
    
- **Move** -スレッド内の現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーに移動されます。 スレッド内の後続のアイテムは移動されません。 
    
- **Copy** -スレッド内の現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーにコピーされます。 スレッド内の後続のアイテムはコピーされません。 
    
- **Setreadstate** -会話内の現在のアイテムの読み取り状態が設定されます。 読み取り状態は、 [isread](isread.md)要素によって設定されます。 
    
- **Flag** -スレッド内の現在のアイテムには、 [flag](flag.md)要素で定義されているフラグが設定されます。 
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

