---
title: 用語
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1a796535-7e83-4aa8-850a-d217059050f8
description: Term 要素は、FindConversation または FindItem 応答で強調表示されている用語を指定します。
ms.openlocfilehash: 12aba499ebfcad392a4e72b29a8cb3522a4f964f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522538"
---
# <a name="term"></a>用語

**Term 要素** は **、FindConversation** または FindItem 応答で強調表示されている **用語を指定** します。 
  
```XML
<Term>
   <Scope/>
   <Value/>
</Term>
```

 **HighlightTermType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Scope (HighlightTermType)](scope-highlighttermtype.md)  | [値](value.md)
  
### <a name="parent-elements"></a>親要素

[HighlightTerms](highlightterms.md)
  
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
   

