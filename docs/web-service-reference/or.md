---
title: Or
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: Or 要素が含まれている検索式に対して論理 OR を実行する検索式を表します。 またはその子のいずれかの場合は true を返す場合は true を返します。 または 2 つ以上の子を持つ必要があります。
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832661"
---
# <a name="or"></a>Or

要素**または**要素が含まれている検索式に対して、論理 **、または**を実行する検索式を表します。 **または** **true**を返します**true**を返す任意の子の場合。 **または**2 つ以上の子が必要です。 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 **OrType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | 制限内での式の基本クラスを表します。 <br/><br/>次の要素の 1 つは、 **SearchExpression**要素に置き換えられる必要があります。 <br/> <br/>- [存在します。](exists.md) <br/>- [除外](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [含まれています](contains.md) <br/>- [じゃない](not.md) <br/>- [そして](and.md) <br/>- **または** <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。 ****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**  <br/> |
|**Or** <br/> |含まれている検索式に対して論理**OR**演算を実行する検索式を表します。 **または** **true**を返します**true**を返す任意の子の場合。 **または**2 つ以上の子が必要です。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

