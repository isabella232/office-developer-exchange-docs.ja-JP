---
title: AggregationRestriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d05044f9-d2ff-4aca-956c-20c9cb2f7709
description: AggregationRestriction 要素は、FindPeople の要求に起因するペルソナ プロパティのセットに適用され、指定した制限に従って結果をフィルター処理する値を指定します。
ms.openlocfilehash: 8b4d5952dedb4de0201d2ecf2219c69f65f7dc09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759309"
---
# <a name="aggregationrestriction"></a>AggregationRestriction

**AggregationRestriction**要素は、FindPeople の要求に起因するペルソナ プロパティのセットに適用され、指定した制限に従って結果をフィルター処理する値を指定します。 
  
```XML
<AggregationRestriction>
   <SearchExpression/>
</AggregationRestriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[SearchExpression](searchexpression.md)
  
### <a name="parent-elements"></a>親要素

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>備考

**AggregationRestriction**要素は、 **SearchExpression**の代替グループを使用する任意の子要素を含めることができます。 **SearchExpression**代替グループの一部になっている要素:[含む](contains.md)、[除外](excludes.md)、 [Exists](exists.md)、[しない](not.md)、[または](or.md)、[および](and.md)、 [IsEqualTo](isequalto.md)、 [IsNotEqualTo](isnotequalto.md)、 [IsGreaterThan](isgreaterthan.md)、 [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)、 [IsLessThan](islessthan.md)、および[IsLessThanOrEqualTo](islessthanorequalto.md)。
  
この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

