---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: SearchExpression 要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 この要素は、XML インスタンスドキュメントでは使用されません。
ms.openlocfilehash: db06ce8e2faa0f2589963d58aab55073c618c171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530353"
---
# <a name="searchexpression"></a>SearchExpression

**Searchexpression**要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 この要素は、XML インスタンスドキュメントでは使用されません。 
  
```xml
<SearchExpression/>
```

 **Search式の種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[制限](restriction.md) <br/> |FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。 And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理**OR**演算を実行する検索式を表します。 **または**、いずれかの子が**true**を返した場合は**true**を返します。 **または、** 2 つ以上の子を持つ必要があります。  <br/> |
   
## <a name="remarks"></a>注釈

SearchExpression 置換グループの一部であるすべての filter 要素は、SearchExpression 要素の代わりに表示できます。
  
> [!NOTE]
> この要素は、インスタンスドキュメント内で直接発生することはありません。 
  
次の要素は、SearchExpression 置換グループのメンバーです。
  
- [Exists](exists.md)
    
- [Excludes](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [内容](contains.md)
    
- [Not](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
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

