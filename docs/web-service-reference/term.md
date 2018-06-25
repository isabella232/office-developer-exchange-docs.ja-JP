---
title: 用語
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a796535-7e83-4aa8-850a-d217059050f8
description: 用語の要素は、FindConversation または FindItem 応答で強調表示されている用語を指定します。
ms.openlocfilehash: cef2ecd7c51b61ccff2c7261a7a612095047956c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839665"
---
# <a name="term"></a>用語

**用語**の要素は、 **FindConversation**または**FindItem**応答で強調表示されている用語を指定します。 
  
```XML
<Term>
   <Scope/>
   <Value/>
</Term>
```

 **HighlightTermType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[スコープ (HighlightTermType)](scope-highlighttermtype.md) | [の値](value.md)
  
### <a name="parent-elements"></a>親要素

[HighlightTerms](highlightterms.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

