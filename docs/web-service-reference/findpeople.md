---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: FindPeople 要素は、FindPeople 要求で使用されるデータのセットを指定します。 データには、ペルサ図形 (オプション)、インデックス付きページ アイテム ビュー、制限 (オプション)、集計制限 (オプション)、並べ替え順序 (オプション)、親フォルダー ID、およびクエリ文字列 (オプション) の 0 個以上が含まれます。
ms.openlocfilehash: 44070c79ad5d1615929a6169d1808cf365b7cab4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535164"
---
# <a name="findpeople"></a>FindPeople

**FindPeople 要素は**、FindPeople 要求で使用されるデータのセットを指定します。 データには、ペルサ図形 (オプション)、インデックス付きページ アイテム ビュー、制限 (オプション)、集計制限 (オプション)、並べ替え順序 (オプション)、親フォルダー ID、およびクエリ文字列 (オプション) の 0 個以上が含まれます。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[PersonaShape](personashape.md)  | [IndexedPageItemView](indexedpageitemview.md)  | [制限](restriction.md)  | [AggregationRestriction](aggregationrestriction.md)  | [SortOrder](sortorder.md)  | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  | [QueryString (QueryStringType)](querystring-querystringtype.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

