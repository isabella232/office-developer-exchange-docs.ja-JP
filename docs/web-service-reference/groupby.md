---
title: GroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupBy
api_type:
- schema
ms.assetid: 9728619b-4674-4b9d-9f6c-e75c6165966c
description: GroupBy 要素は、FindItem クエリの任意のグループ化を指定します。
ms.openlocfilehash: 0d681e5376e4dd71921cc97f270211e49179db85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530100"
---
# <a name="groupby"></a>GroupBy

**GroupBy**要素は、FindItem クエリの任意のグループ化を指定します。 
  
- [FindItem](finditem.md)
- [GroupBy](groupby.md)
  
```xml
<GroupBy Order="">
   <FieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <ExtendededFieldURI/>
   <AggregateOn/>
</GroupBy>
```

```xml
<GroupBy Order="">
   <IndexedFieldURI/>
   <AggregateOn/>
</GroupBy>
```

**GroupByType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Order** <br/> | 応答で返されるグループ化されたアイテムの配列内のグループの順序を指定します。 この属性の型は Sortdirection 型です。  <br/> |
   
#### <a name="order-attribute-values"></a>Order 属性の値

|**値**|**説明**|
|:-----|:-----|
|Ascending/昇順  <br/> |グループは昇順で並べ替えられます。  <br/> |
|Descending/降順  <br/> |グループは、降順で順序付けられます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI で頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |取得、設定、または作成する拡張 MAPI プロパティを識別します。  <br/> |
|[AggregateOn](aggregateon.md) <br/> |応答内のグループの順序を決定するために使用されるフィールドを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/><br/> この要素の XPath 式を次に示します。`/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

FindItem 応答には、グループのコレクションが含まれています。 各グループには、 **GroupBy**プロパティに一致する値を持つすべてのアイテムが含まれます。 グループ化を決定するプロパティは、 [FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素で識別されます。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindItem 操作](finditem-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

