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
ms.openlocfilehash: d85c0fddec244c99dfbea1f85da331fc5319536d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831753"
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

 **GroupByType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Order** <br/> | 応答で返されるグループ化されたアイテムの配列内のグループの順序を決定します。 この属性は、型 SortDirectionType のです。  <br/> |
   
#### <a name="order-attribute-values"></a>順序属性の値

|**値**|**説明**|
|:-----|:-----|
|Ascending/昇順  <br/> |グループは昇順で並べ替えられます。  <br/> |
|降順  <br/> |グループは降順で並べ替えられます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |取得、設定、または作成する拡張の MAPI プロパティを識別します。  <br/> |
|[AggregateOn](aggregateon.md) <br/> |応答内のグループの順序を決定するために使用されるフィールドを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/><br/> この要素への XPath 式は、次のようにします。`/FindItem` <br/> |
   
## <a name="remarks"></a>備考

FindItem 応答グループのコレクションが含まれます。 **GroupBy**プロパティの値が一致するすべての項目は、各グループが含まれます。 [FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素のグループ化を決定するプロパティが識別されます。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [FindItem 操作](finditem-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

