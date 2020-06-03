---
title: ソート順序 (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: 並べ替え要素は、GetConversationItems 要求の結果に使用される並べ替え順序を指定します。
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530966"
---
# <a name="sortorder-conversationnodesortorder"></a>ソート順序 (ConversationNodeSortOrder)

並べ替え**要素は、** **GetConversationItems**要求の結果に使用される並べ替え順序を指定します。 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>テキスト値

**ソート**順序要素のテキスト値は、会話が並べ替えられる順序です。 **Treeorderascending**のテキスト値は、会話が会話ツリーに従って昇順で並べ替えられることを示します。 **Treeorderdescending**のテキスト値は、会話が会話ツリーに従って降順に並べ替えられていることを示します。 **Dateorderascending**のテキスト値は、会話の日付に従って、会話が昇順で並べ替えられることを示します。 **Dateorderdescending**のテキスト値は、会話の日付に基づいて、会話が降順で並べ替えられることを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

