---
title: Contains
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
description: 含まれる要素は、指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。
ms.openlocfilehash: b25b69aadf2c331527a17ad81ed46f61aa7b93c2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354289"
---
# <a name="contains"></a>Contains

**含まれる**要素は、指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ContainmentMode** <br/> |検索の範囲を識別します。  <br/> |
|**ContainmentComparison** <br/> |検索には、ケースとのスペースが無視されるかどうかを決定します。  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>ContainmentMode 属性の値

|**値**|**説明**|
|:-----|:-----|
|プリフィックス  <br/> |比較では、完全な文字列と定数との間です。 プロパティの値と指定された定数は正確に同じです。  <br/> |
|プレフィックス  <br/> |比較は文字列のプレフィックスと定数との間です。  <br/> |
|部分文字列  <br/> |比較は、文字列の部分文字列と定数との間です。  <br/> |
|PrefixOnWords  <br/> |比較は文字列内の各単語のプレフィックスと定数との間です。  <br/> |
|ExactPhrase  <br/> |比較は、文字列の完全一致のフレーズと定数との間です。  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>ContainmentComparison 属性の値

|**値**|**説明**|
|:-----|:-----|
|Exact  <br/> |比較は正確である必要があります。  <br/> |
|IgnoreCase  <br/> |比較は、大文字と小文字を無視します。  <br/> |
|IgnoreNonSpacingCharacters  <br/> |比較では、空白でない文字を無視します。  <br/> |
|広く  <br/> |削除します。  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |比較は、大文字と非空白文字を無視します。  <br/> |
|LooseAndIgnoreCase  <br/> |削除します。  <br/> |
|LooseAndIgnoreNonSpace  <br/> |削除します。  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |削除します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[定数](constant.md) <br/> |制限における定数値を識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。 **すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理 OR を実行する検索式を表します。 その子のいずれかの**場合は true**を返す場合、要素[または](or.md)要素は**true**を返します。  <br/> |
   
## <a name="remarks"></a>注釈

属性を使用すると、要素を照合する方法を決定します。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

