---
title: 集約 Ationrestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: 集約 Ationrestriction 要素は、FindPeople 要求の結果として得られる一連のペルソナプロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。
ms.openlocfilehash: f07e54235cf13b43da26ed1c56596d3c7c357bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463525"
---
# <a name="aggregationrestriction"></a>集約 Ationrestriction

**集約 Ationrestriction**要素は、findpeople 要求の結果として得られる一連のペルソナプロパティに適用される値を指定し、指定された制限に従って結果をフィルター処理します。 
  
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

**集約 Ationrestriction**要素には、 **searchexpression** substitution グループを使用する子要素を含めることができます。 **Searchexpression**置換グループの一部である要素は次のとおりです[。 Contains](contains.md)、[除外](excludes.md)、 [Exists](exists.md)、 [Not](not.md)、 [and](and.md) [、](or.md) [IsEqualTo](isequalto.md)、IsNotEqualTo、 [IsGreaterThan](isgreaterthan.md)、 [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)、 [is](isnotequalto.md)、および[IsLessThan](islessthan.md) [IsLessThanOrEqualTo](islessthanorequalto.md)。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

