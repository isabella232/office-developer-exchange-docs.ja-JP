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
description: Restriction 要素は、FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。
ms.openlocfilehash: 6037ba15417d67d393ca70f3edf2248749c396e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465290"
---
# <a name="restriction"></a>制限

**Restriction**要素は、FindItem/findfolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[And](and.md) <br/> |2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。  <br/> |
|[内容](contains.md) <br/> |指定したプロパティに指定した定数文字列値が含まれているかどうかを決定する検索式を表します。  <br/> |
|[Excludes](excludes.md) <br/> |プロパティのビット単位のマスクを実行します。  <br/> |
|[Exists](exists.md) <br/> |指定されたプロパティがアイテムに存在する場合に**true**を返す検索式を表します。  <br/> |
|[IsEqualTo](isequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、等しい場合は**true**に評価される検索式を表します。  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティよりも大きい場合に**true**を返す検索式を表します。  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティよりも大きいか等しい場合に**true**を返す検索式を表します。  <br/> |
|[IsLessThan](islessthan.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティより小さい場合に**true**を返す検索式を表します。  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティ以下の場合に**true**を返す検索式を表します。  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |プロパティを定数値または別のプロパティと比較し、値が同じでない場合は**true**を返す検索式を表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理**OR**演算を実行する検索式を表します。 **または**のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。  <br/> |
|[SearchExpression](searchexpression.md) <br/> |制限内の代替要素を表します。 この要素は、XML インスタンスドキュメントでは使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別する要求を定義します。  <br/> |
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> |
|[SearchParameters](searchparameters.md) <br/> |検索フォルダーを定義するパラメーターを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

