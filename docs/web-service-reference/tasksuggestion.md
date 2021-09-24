---
title: TaskSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ade9ea3b-bdf1-4999-ac7d-44c6452cef36
description: TaskSuggestion 要素には、アイテムから抽出されたエンティティから発生したタスク候補が含まれる。
ms.openlocfilehash: a7d74523b57825b97c6c6d9c2194d84af3f38d5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538878"
---
# <a name="tasksuggestion"></a>TaskSuggestion

**TaskSuggestion 要素** には、アイテムから抽出されたエンティティから発生したタスク候補が含まれる。 
  
```XML
<TaskSuggestion>
   <Position/>
   <TaskString/>
   <Assignees/>
</TaskSuggestion>
```

**TaskSuggestionType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[位置](position.md)  | [TaskString](taskstring.md)  | [割り当て人](assignees.md)
  
### <a name="parent-elements"></a>親要素

[TaskSuggestions](tasksuggestions.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

