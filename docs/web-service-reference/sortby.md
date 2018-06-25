---
title: 並べ替え
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: 並べ替えの要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833518"
---
# <a name="sortby"></a>並べ替え

**並べ替え**の要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Order  <br/> |**順序**属性のテキスト値は、並べ替え順序です。 **昇順**のテキスト値は、結果を昇順であることを示します。 **降順**のテキスト値は、結果が降順であることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxes](searchmailboxes.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

