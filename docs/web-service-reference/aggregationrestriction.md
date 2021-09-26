---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: AggregationRestriction 要素は、FindPeople 要求から生じる一連の Persona プロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。
ms.openlocfilehash: 6a00035f87e0f365f4551df1a6ff570e01761770
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546792"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

**AggregationRestriction** 要素は、FindPeople 要求から生じる一連の Persona プロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>親要素

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>注釈

**AggregationRestriction 要素には****、SearchExpression** 置換グループを使用する任意の子要素を含めできます。 **SearchExpression** 置換グループの一部である要素は [、Contains](contains.md)、 [Excludes](excludes.md)、 [Exists](exists.md)、 [Not](not.md)、 [Or](or.md) [、](and.md)And 、 [IsEqualTo](isequalto.md)、 [IsNotEqualTo](isnotequalto.md)、 [IsGreaterThan](isgreaterthan.md)、 [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)、 [IsLessThan](islessthan.md)、[および IsLessThanOrEqualTo](islessthanorequalto.md)です。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

