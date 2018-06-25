---
title: 制限
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: 制限要素は、制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。
ms.openlocfilehash: 6b5702696db29910ae476a370bf362fe6a036ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833213"
---
# <a name="restriction"></a>制限

**制限**要素は、制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[And](and.md) <br/> |使用すると、2 つまたは複数の検索式間でブール型の**AND**操作を実行する検索式を表します。  <br/> |
|[内容](contains.md) <br/> |指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。  <br/> |
|[除外](excludes.md) <br/> |プロパティのビットごとのマスクを実行します。  <br/> |
|[存在します。](exists.md) <br/> |**True**を返す指定されたプロパティが存在する場合、アイテムの検索式を表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティを比較し、これらが等しい場合**は true**に評価する検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |最初のプロパティの値やプロパティよりも大きい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |最初のプロパティは、以上の値またはプロパティに値がある場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |最初のプロパティの値やプロパティよりも小さい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |最初のプロパティの値またはプロパティに等しいかそれより小さい場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |値が同じではない場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理**OR**演算を実行する検索式を表します。 その子のいずれかの**場合は true**を返す場合、要素**または**要素は**true**を返します。  <br/> |
|[SearchExpression](searchexpression.md) <br/> |制限内の代替要素を表します。 XML インスタンス ドキュメントでは、この要素は使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> |
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> |
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
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

