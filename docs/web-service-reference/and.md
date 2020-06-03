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
description: And 要素は、2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。 And 操作の結果は、And 要素に含まれるすべての検索式が true である場合に true となります。
ms.openlocfilehash: f5239f19c2b5a931eefa9ff4a9dd8ed9d775bae2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464722"
---
# <a name="and"></a>And

**And**要素は、2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。 And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **AndType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | 制限内の式の基本クラスを表します。 And 操作には、2つ以上の検索式を指定する必要があります。<br/><br/>  **Searchexpression**要素には、次のいずれかの要素を置き換える必要があります。<ul><li> [Exists](exists.md)</li><li>[Excludes](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[内容](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[制限](restriction.md) <br/> |FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|**And** <br/> |2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。 And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理**OR**演算を実行する検索式を表します。 **または**、いずれかの子が**true**を返した場合は**true**を返します。 **または、** 2 つ以上の子を持つ必要があります。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

