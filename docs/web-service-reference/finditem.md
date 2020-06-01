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
description: FindItem 要素は、メールボックス内のアイテムを検索する要求を定義します。
ms.openlocfilehash: 3aeda1cffc03292734a91bc3fff3289d51c9b445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460996"
---
# <a name="finditem"></a>FindItem

**FindItem**要素は、メールボックス内のアイテムを検索する要求を定義します。 
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**走査** <br/> |検索でフォルダー内のアイテムとフォルダーの dumpsters を検索するかどうかを定義します。 この属性は必須です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>トラバース属性値

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |フォルダー内のアイテムの id のみを返します。  <br/> |
|削除済み (回復可能)  <br/> |フォルダーの収集に含まれるアイテムの id のみを返します。 検索条件に一致するアイテムが存在する場合でも、回復可能な削除によって削除された検査によって返されるアイテムが0個になることに注意してください。  <br/> |
|関連  <br/> |フォルダー内の関連付けられたアイテムの id のみを返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |[FindItem 操作](finditem-operation.md)応答に含めるアイテムのプロパティとコンテンツを識別します。  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |**FindItem**要求に対して、ページングされたアイテムの情報を返す方法について説明します。 この要素は省略できます。  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |ページビューの開始位置と、 **FindItem**要求で返されるアイテムの最大数を指定します。 検索されたアイテムのセットの先頭からのページビューオフセットは、分数で示されます。 この要素は省略できます。  <br/> |
|[CalendarView](calendarview.md) <br/> |予定表アイテムの検索を定義するための時間範囲制限を指定します。 この要素は省略できます。  <br/> |
|[ContactsView](contactsview.md) <br/> |アルファベットの表示名に基づいて、連絡先アイテムの検索を定義します。 この要素は省略できます。  <br/> |
|[GroupBy](groupby.md) <br/> |**FindItem**クエリの任意のグループを指定します。 この要素は省略できます。  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |**FindItem**クエリの標準的なグループを提供します。 この要素は省略できます。  <br/> |
|[Restriction](restriction.md) <br/> |**FindItem** /  **findfolder**および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを定義します。 この要素は省略できます。  <br/> |
|[SortOrder](sortorder.md) <br/> |FindItem 要求でのアイテムの並べ替え方法を定義します。 この要素は省略できます。  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |FindItem および FindFolder 操作を検索するフォルダーを指定します。  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列が格納されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

**FindItem**要求に含めることができるのは、 [Indexedpageitemview](indexedpageitemview.md)、 [FractionalPageItemView](fractionalpageitemview.md)、 [CalendarView](calendarview.md)、または[ContactsView](contactsview.md)要素のいずれか1つだけです。 **FindItem**要求に含めることができるのは、 [GroupBy](groupby.md)または[DistinguishedGroupBy](distinguishedgroupby.md)要素のいずれか1つだけです。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

