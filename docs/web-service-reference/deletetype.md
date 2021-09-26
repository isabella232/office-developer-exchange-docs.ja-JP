---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: DeleteType 要素は、会話内のアイテムを削除する方法を示します。
ms.openlocfilehash: 828950e72179c17cd3efaa78df677bb7f15789c2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543402"
---
# <a name="deletetype"></a>DeleteType

**DeleteType 要素** は、会話内のアイテムを削除する方法を示します。 
  
- [ApplyConversationAction](applyconversationaction.md)  
- [ConversationActions](conversationactions.md)  
- [ConversationAction](conversationaction.md)  
- [DeleteType](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 **DisposalType**
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

DeleteType 要素の **テキスト値** は、会話内のアイテムを削除する方法を示します。 使用できるテキスト値は次のとおりです。 
  
- HardDelete - 会話内のアイテムがメールボックス データベースから完全に削除されるかどうかを示します。
    
- MoveToDeleteItems - 会話内のアイテムが [削除済みアイテム] フォルダーに移動されます。
    
- SoftDelete - ゴミ箱が有効になっている場合、会話内のアイテムがゴミ箱に移動されます。
    
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

