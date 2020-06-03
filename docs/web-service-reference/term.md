---
title: 用語
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a796535-7e83-4aa8-850a-d217059050f8
description: Term 要素は、FindConversation または FindItem 応答で強調表示された用語を指定します。
ms.openlocfilehash: fb102e21d6e7866110735cacd60cd2c3c68a9675
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459491"
---
# <a name="term"></a>用語

**Term**要素は、 **Findconversation**または**FindItem**応答で強調表示された用語を指定します。 
  
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

[範囲 (HighlightTermType)](scope-highlighttermtype.md)  | [値](value.md)
  
### <a name="parent-elements"></a>親要素

[HighlightTerms](highlightterms.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

