---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Contains 要素は、指定されたプロパティに指定された定数文字列値が含まれているかどうかを決定する検索式を表します。
ms.openlocfilehash: 6e36ede6a10c64a4aa53e68721d9edf7893c4c05
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547548"
---
# <a name="contains"></a>Contains

**Contains 要素** は、指定されたプロパティに指定された定数文字列値が含まれているかどうかを決定する検索式を表します。 
  
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


**ContainsExpressionType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ContainmentMode** <br/> |検索の境界を識別します。  <br/> |
|**ContainmentComparison** <br/> |検索で大文字と小文字とスペースを無視するかどうかを指定します。  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>ContainmentMode 属性値

|**値**|**説明**|
|:-----|:-----|
|FullString  <br/> |比較は、完全な文字列と定数の間です。 プロパティ値と指定された定数は正確に同じです。  <br/> |
|プレフィックス  <br/> |比較は、文字列プレフィックスと定数の間です。  <br/> |
|Substring  <br/> |比較は、文字列の部分文字列と定数の間です。  <br/> |
|PrefixOnWords  <br/> |比較は、文字列内の個々の単語のプレフィックスと定数の間です。  <br/> |
|ExactPhrase  <br/> |比較は、文字列内の正確な語句と定数の間です。  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>ContainmentComparison 属性値

|**値**|**説明**|
|:-----|:-----|
|Exact  <br/> |比較は正確である必要があります。  <br/> |
|IgnoreCase  <br/> |比較では大文字小文字の区別は無視されます。  <br/> |
|IgnoreNonSpacingCharacters  <br/> |この比較では、スペース以外の文字は無視されます。  <br/> |
|広く  <br/> |削除する。  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |この比較では、大文字と小文字を区別しない文字は無視されます。  <br/> |
|LooseAndIgnoreCase  <br/> |削除する。  <br/> |
|LooseAndIgnoreNonSpace  <br/> |削除する。  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |削除する。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[定数](constant.md) <br/> |制限内の定数値を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値をネゲートする検索式を表します。  <br/> |
|[And](and.md) <br/> |2 つ以上の検索式の間で Boolean And 操作を実行できる検索式を表します。 And に含まれるすべての検索式が **true** の場合、And 操作の結果は true **です**。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 OR を実行する検索式を表します。 [Or 要素は](or.md)、その子 **が true** を返す場合に true を返 **します**。  <br/> |
   
## <a name="remarks"></a>注釈

属性は、要素の一致方法を決定するために使用されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

