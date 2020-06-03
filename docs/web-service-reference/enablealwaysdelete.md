---
title: Enablealways Delete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EnableAlwaysDelete
api_type:
- schema
ms.assetid: 7753aec5-3f93-4aeb-a28e-8b9b42ca7f9b
description: Enablealways Delete 要素は、スレッド内のすべての新しいアイテムの削除を有効にするフラグを指定します。
ms.openlocfilehash: 14784d3a6ba52c76b64b81e15c0522d66d125cbf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526208"
---
# <a name="enablealwaysdelete"></a>Enablealways Delete

**Enablealways delete**要素は、スレッド内のすべての新しいアイテムの削除を有効にするフラグを指定します。 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[Enablealways Delete](enablealwaysdelete.md)
  
```XML
<EnableAlwaysDelete/>
```

 **xs: boolean**
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

**Enablealways delete**要素のテキスト値は、スレッド内のすべてのアイテムの削除を有効にする**場合は true**です。それ以外の場合は**false**。
  
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



[ApplyConversationAction 操作](applyconversationaction-operation.md)

