---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: 除外要素は、指定されたプロパティと指定された値のビット単位のマスクを実行します。
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530615"
---
# <a name="excludes"></a>Excludes

**除外**要素は、指定されたプロパティと指定された値のビット単位のマスクを実行します。 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

**ExcludesType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI で頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[示す](bitmask.md) <br/> |[除外](excludes.md)制限操作で使用する16進数または10進数のマスクを表します。 ビットマスクが16進数を表す場合は、0x または0X でプレフィックスする必要があります。 それ以外の場合は、10進数値と見なされます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[制限](restriction.md) <br/> |FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。 And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 OR を実行する検索式を表します。 [または](or.md)のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。  <br/> |
   
## <a name="remarks"></a>注釈

を**除外**すると、次のように実行された AND 操作が0に解決される場合は**true**になります。 
  
1. プロパティのビット単位の値
    
2. プロパティのビットマスク値
    
**除外**は、整数値を持つプロパティにのみ適用できます。 プロパティの型が整数以外の場合は、エラーコード**Error、Supportedpathforquery**が応答で返されます。 
  
逆の操作を実行するには、Not (除外) を呼び出します。
  
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

