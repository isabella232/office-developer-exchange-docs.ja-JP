---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'FindPeople 要素は、FindPeople 要求で使用されるデータのセットを指定します。 次の要素の 0 個以上のデータが含まれています: ペルソナの図形 (オプション)、ページのインデックス付きのアイテム ビュー、制限 (省略可能) に集約が制限 (省略可能)、(省略可能) の並べ替え順序、親フォルダー Id、およびクエリ文字列 (省略可能)。'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760531"
---
# <a name="findpeople"></a>FindPeople

**FindPeople**要素は、FindPeople 要求で使用されるデータのセットを指定します。 次の要素の 0 個以上のデータが含まれています: ペルソナの図形 (オプション)、ページのインデックス付きのアイテム ビュー、制限 (省略可能) に集約が制限 (省略可能)、(省略可能) の並べ替え順序、親フォルダー Id、およびクエリ文字列 (省略可能)。 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 **FindPeopleType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [制限](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [ソート順序](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [クエリ文字列 (QueryStringType)](querystring-querystringtype.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

