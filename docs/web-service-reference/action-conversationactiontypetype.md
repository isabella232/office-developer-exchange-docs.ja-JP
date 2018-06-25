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
description: Action 要素には、ConversationId 要素で指定されたスレッド上で実行するアクションが含まれています。
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759265"
---
# <a name="action-conversationactiontypetype"></a>アクション (ConversationActionTypeType)

**Action**要素には、 [ConversationId](conversationid.md)要素で指定されたスレッド上で実行するアクションが含まれています。 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [ConversationActions](conversationactions.md)
  
- [ConversationAction](conversationaction.md)
  
- [アクション (ConversationActionTypeType)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **ConversationActionTypeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |1 つのテーマを適用する 1 つのアクションが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Action**要素のテキスト値では、会話するアクションが実行されますを示します。 可能なテキスト値と対応するアクションを次に示します。 
  
- **AlwaysCategorize** - 現在の項目との会話では、[カテゴリ](categories-ex15websvcsotherref.md)の要素で識別されるカテゴリを使用して自動的に設定されます。 
    
- **AlwaysDelete** - 現在の項目との会話に新しいアイテムが自動的に削除されます。 削除モードは、[削除の種類](deletetype.md)の要素によって設定されます。 
    
- **AlwaysMove** - 現在の項目との会話では、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーに自動的に移動されます。 
    
- **削除**・ スレッドの現在のアイテムは削除されます。 会話でそれ以降の項目は削除されません。 削除モードは、[削除の種類](deletetype.md)の要素によって設定されます。 
    
- **移動**- スレッドの現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーに移動されます。 スレッドのそれ以降のアイテムは移動されません。 
    
- **コピー** - スレッドの現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーにコピーされます。 スレッドのそれ以降のアイテムはコピーされません。 
    
- **SetReadState**のスレッドの現在のアイテムの読み取り状態の設定があります。 [IsRead](isread.md)要素によって、読み取りの状態が設定されています。 
    
- **フラグ**スレッドの現在のアイテムは、フラグが設定されている[フラグ](flag.md)の要素で定義されているがあります。 
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

