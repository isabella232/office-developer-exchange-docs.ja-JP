---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: ConversationNode 要素は、会話内のノードを指定します。
ms.openlocfilehash: 2668d3cfaa8b43812a4a20ab8d92f419d636e368
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510359"
---
# <a name="conversationnode"></a>ConversationNode

**ConversationNode 要素** は、会話内のノードを指定します。 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 **ConversationNodeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[InternetMessageId](internetmessageid.md) <br/> |アイテムのインターネット メッセージ識別子を表します。  <br/> |
|[ParentInternetMessageId](parentinternetmessageid.md) <br/> |親インターネット メッセージの識別子を指定します。  <br/> |
|[ItemIds (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |会話ノード内のすべての項目を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationNodes](conversationnodes.md) <br/> |会話ノードのコレクションを指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

