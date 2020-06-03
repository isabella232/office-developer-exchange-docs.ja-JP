---
title: 内容
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Contains 要素は、指定したプロパティに指定の定数文字列値が含まれているかどうかを決定する検索式を表します。
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527118"
---
# <a name="contains"></a>内容

**Contains**要素は、指定したプロパティに指定の定数文字列値が含まれているかどうかを決定する検索式を表します。 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


**型**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**このモード** <br/> |検索の境界を識別します。  <br/> |
|**式の比較** <br/> |検索でケースとスペースを無視するかどうかを指定します。  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>指定した要素の属性値

|**値**|**説明**|
|:-----|:-----|
|FullString  <br/> |完全な文字列と定数の間の比較があります。 プロパティの値と指定された定数は正確に同じです。  <br/> |
|固定長  <br/> |文字列プレフィックスと定数の間に比較があります。  <br/> |
|副  <br/> |文字列の部分文字列と定数の間の比較。  <br/> |
|PrefixOnWords  <br/> |文字列内の個々の単語のプレフィックスと定数の間の比較が比較されます。  <br/> |
|ExactPhrase  <br/> |文字列内の完全に一致する語句と定数の間に比較があります。  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>要素の比較属性値

|**値**|**説明**|
|:-----|:-----|
|ニーズ  <br/> |比較は厳密でなければなりません。  <br/> |
|IgnoreCase  <br/> |比較では大文字と小文字は区別されません。  <br/> |
|Ignorenon文字  <br/> |比較では、スペース以外の文字は無視されます。  <br/> |
|広く  <br/> |を削除します。  <br/> |
|Ignorecaseandnon文字  <br/> |比較では大文字と小文字は区別されません。  <br/> |
|LooseAndIgnoreCase  <br/> |を削除します。  <br/> |
|LooseAndIgnoreNonSpace  <br/> |を削除します。  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |を削除します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI で頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[定数](constant.md) <br/> |制限で定数値を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[制限](restriction.md) <br/> |FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。 And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 OR を実行する検索式を表します。 [または](or.md)のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。  <br/> |
   
## <a name="remarks"></a>注釈

これらの属性は、要素の照合方法を決定するために使用されます。
  
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

