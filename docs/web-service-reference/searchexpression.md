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
description: SearchExpression 要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 XML インスタンス ドキュメントでは、この要素は使用されません。
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833286"
---
# <a name="searchexpression"></a>SearchExpression

**SearchExpression**要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 XML インスタンス ドキュメントでは、この要素は使用されません。 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。 ****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理**OR**演算を実行する検索式を表します。 **または** **true**を返します**true**を返す任意の子の場合。 **または**2 つ以上の子が必要です。  <br/> |
   
## <a name="remarks"></a>備考

SearchExpression 代替グループの一部である任意のフィルター要素は、SearchExpression 要素の代わりに表示できます。
  
> [!NOTE]
> この要素は、インスタンス ドキュメント内で直接は発生しません。 
  
次の要素は、SearchExpression 代替グループのメンバーです。
  
- [存在します。](exists.md)
    
- [除外](excludes.md)
    
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

