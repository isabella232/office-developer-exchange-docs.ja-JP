---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: FindItem 要素では、メールボックス内のアイテムを検索するための要求を定義します。
ms.openlocfilehash: 6664cd91007f1d39db7e8d446e0135f47d5ab932
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353925"
---
# <a name="finditem"></a>FindItem

**FindItem**要素では、メールボックス内のアイテムを検索するための要求を定義します。 
  
```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <IndexedPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <ContactsView/> 
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <CalendarView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <GroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```

```xml
<FindItem Traversal="">
   <ItemShape/>
   <FractionalPageItemView/>
   <DistinguishedGroupBy/>
   <Restriction/>
   <SortOrder/>
   <ParentFolderIds/>
   <QueryString/>
</FindItem>
```


**FindItemType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**トラバーサル** <br/> |検索がフォルダーまたはフォルダーの dumpsters でアイテムを検索するかどうかを定義します。 この属性は、必要があります。  <br/> |
   
#### <a name="traversal-attribute-values"></a>検査の属性値

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |フォルダー内のアイテムの id だけを返します。  <br/> |
|削除済み (回復可能)  <br/> |フォルダーの内にあるアイテムの id だけを返します。 ごみ箱をあさる。 ノートの検索の制限と組み合わせて、ソフト削除走査返される項目が 0 の原因になる場合でも、検索条件に一致する項目があります。  <br/> |
|関連  <br/> |フォルダーに関連付けられているアイテムの id だけを返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |[FindItem 操作](finditem-operation.md)の応答に含めるコンテンツ アイテムのプロパティを識別します。  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |どのページの項目の情報について説明します**FindItem**要求に対して返されます。 この要素はオプションです。  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |ページ ビューが開始され**FindItem**要求内のアイテムの最大数が返されるをについて説明します。 見つかった項目のセットの先頭からのページ ビュー オフセットは、分数で表されます。 この要素はオプションです。  <br/> |
|[CalendarView](calendarview.md) <br/> |時間は、予定表アイテムの検索を定義する制限に 。 この要素はオプションです。  <br/> |
|[ContactsView](contactsview.md) <br/> |連絡先アイテムをアルファベット順の表示名を基に検索を定義します。 この要素はオプションです。  <br/> |
|[GroupBy](groupby.md) <br/> |**FindItem**クエリの任意のグループを指定します。 この要素はオプションです。  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |**FindItem**クエリの標準的なグループ化を提供します。 この要素はオプションです。  <br/> |
|[Restriction](restriction.md) <br/> |制限またはアイテムや**FindItem**内のフォルダーにフィルターを使用するクエリを定義する/ **FindFolder**検索フォルダーの操作です。 この要素はオプションです。  <br/> |
|[SortOrder](sortorder.md) <br/> |FindItem 要求内のアイテムの並べ替え方法を定義します。 この要素はオプションです。  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |FindItem と FindFolder 操作を検索するフォルダーを識別します。  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

**FindItem**要求で、 [IndexedPageItemView](indexedpageitemview.md)、 [FractionalPageItemView](fractionalpageitemview.md)、[予定表ビュー](calendarview.md)、または[ContactsView](contactsview.md)要素の 1 つだけ含まれていることができます。 **FindItem**要求で[GroupBy](groupby.md)または[DistinguishedGroupBy](distinguishedgroupby.md)要素の 1 つだけ含まれていることができます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
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
- [項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

