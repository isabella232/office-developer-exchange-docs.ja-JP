---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: SearchExpression 要素は、制限内の置換された要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 この要素は、XML インスタンス ドキュメントでは使用されません。
ms.openlocfilehash: e8047d333b36d77bc6823efd6488a15a6d2501a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517848"
---
# <a name="searchexpression"></a>SearchExpression

**SearchExpression 要素** は、制限内の置換された要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 この要素は、XML インスタンス ドキュメントでは使用されません。 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値をネゲートする検索式を表します。  <br/> |
|[And](and.md) <br/> |2 つ以上の検索式の間で **ブール型 AND** 演算を実行できる検索式を表します。 **And** 要素に含まれるすべての検索式が true の場合 **、AND** 操作の結果は true **です**。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 **OR** 操作を実行する検索式を表します。 **または** 、子が **true** を返す場合は true を **返します**。 **または、2** つ以上の子が必要です。  <br/> |
   
## <a name="remarks"></a>注釈

SearchExpression 置換グループの一部であるフィルター要素は、SearchExpression 要素の代に表示できます。
  
> [!NOTE]
> この要素は、インスタンス ドキュメント内で直接発生しません。 
  
次の要素は、SearchExpression 置換グループのメンバーです。
  
- [Exists](exists.md)
    
- [Excludes](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contains](contains.md)
    
- [Not](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

