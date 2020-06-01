---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: SortBy 要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468398"
---
# <a name="sortby"></a>SortBy

**SortBy**要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Order  <br/> |**Order**属性のテキスト値は、並べ替えの順序です。 テキスト値が**昇順**の場合は、結果が昇順になることを示します。 テキスト値が**降順**の場合は、結果が降順であることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

[FieldURI](fielduri.md)  | [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxes](searchmailboxes.md)
  
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
   

