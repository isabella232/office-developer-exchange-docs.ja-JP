---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: DeleteType 要素は、スレッド内のアイテムが削除される方法を示します。
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442634"
---
# <a name="deletetype"></a>DeleteType

**Deletetype**要素は、スレッド内のアイテムが削除される方法を示します。 
  
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
|[ConversationAction](conversationaction.md) <br/> |単一の会話に適用される1つのアクションが含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Deletetype**要素のテキスト値は、スレッド内のアイテムが削除される方法を示します。 可能なテキスト値を次に示します。 
  
- ハード削除-会話内のアイテムがメールボックスデータベースから完全に削除されることを示します。
    
- MoveToDeleteItems-スレッド内のアイテムが [削除済みアイテム] フォルダーに移動されたことを示します。
    
- SoftDelete-メッセージの収集が有効になっている場合に、スレッド内のアイテムが収集に移動されることを示します。
    
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

