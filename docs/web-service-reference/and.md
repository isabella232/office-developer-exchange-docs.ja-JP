---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: 要素は、2 つまたは複数の検索式間で論理 AND 演算を実行できるようにする検索式を表します。 AND 演算の結果では、要素内に含まれるすべての検索式に該当する場合は true です。
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759323"
---
# <a name="and"></a>And

**および**要素は、2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。 ****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **実際**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | 制限内での式の基本クラスを表します。 And 演算では、2 つまたは複数の検索式を入力する必要があります。<br/><br/>  次の要素の 1 つは、 **SearchExpression**要素に置き換えられる必要があります。<ul><li> [存在します。](exists.md)</li><li>[除外](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[内容](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|**And** <br/> |2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。 ****および**要素内に含まれている検索式のすべてに**該当**する場合は、 **AND**演算の結果は**  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理**OR**演算を実行する検索式を表します。 **または** **true**を返します**true**を返す任意の子の場合。 **または**2 つ以上の子が必要です。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

