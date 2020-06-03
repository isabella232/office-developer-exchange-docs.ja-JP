---
title: 未サポート
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: Not 要素は、それに含まれる検索式の Boolean 値を否定する検索式を表します。
ms.openlocfilehash: 84c64a6d9d39f260d416fc32e4e5f5fcdef027e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466718"
---
# <a name="not"></a>未サポート

**Not**要素は、それに含まれる検索式の Boolean 値を否定する検索式を表します。 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 **NotType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | 制限内の式の基本クラスを表します。 <br/><br/>**Searchexpression**要素には、次のいずれかの要素を置き換える必要があります。 <br/> <br/>- [ある](exists.md) <br/>- [除外](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [Isna](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [含み](contains.md) <br/>- **じゃない** <br/>- [そして](and.md) <br/>- [や](or.md) <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[制限](restriction.md) <br/> |FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|**Not** <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。 And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理**OR**演算を実行する検索式を表します。 **または**、いずれかの子が**true**を返した場合は**true**を返します。 **または、** 2 つ以上の子を持つ必要があります。  <br/> |
   
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

