---
title: FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindItem
api_type:
- schema
ms.assetid: f7624f5c-c390-4563-ab9a-08f1024fb914
description: FindItem 要素は、メールボックス内のアイテムを検索する要求を定義します。
ms.openlocfilehash: 7005b4a837c61ffa00a49b687e729de7ed769bcf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541316"
---
# <a name="finditem"></a>FindItem

**FindItem 要素は**、メールボックス内のアイテムを検索する要求を定義します。 
  
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
|**Traversal** <br/> |検索でフォルダー内のアイテムを検索するか、フォルダーのゴミ箱を検索するかを定義します。 この属性は必須です。  <br/> |
   
#### <a name="traversal-attribute-values"></a>Traversal 属性値

|**値**|**説明**|
|:-----|:-----|
|浅い  <br/> |フォルダー内のアイテムの ID のみを返します。  <br/> |
|削除済み (回復可能)  <br/> |フォルダーのゴミ箱にあるアイテムの ID のみを返します。 検索条件に一致するアイテムがある場合でも、ソフト削除されたトラバーサルと検索制限を組み合わせると、返されるアイテムは 0 になります。  <br/> |
|関連  <br/> |フォルダー内の関連アイテムの ID のみを返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |FindItem 操作応答に含めるアイテムのプロパティとコンテンツ [を識別](finditem-operation.md) します。  <br/> |
|[IndexedPageItemView](indexedpageitemview.md) <br/> |FindItem 要求に対してページアイテム情報がどのように返される **のかについて説明** します。 この要素は省略できます。  <br/> |
|[FractionalPageItemView](fractionalpageitemview.md) <br/> |ページ ビューの開始場所と **FindItem** 要求で返されるアイテムの最大数について説明します。 見つかった項目のセットの先頭からのページ ビューのオフセットは、分数で表されます。 この要素は省略できます。  <br/> |
|[CalendarView](calendarview.md) <br/> |予定表アイテムの検索を定義する期間の制限を提供します。 この要素は省略できます。  <br/> |
|[ContactsView](contactsview.md) <br/> |アルファベット順の表示名に基づいて連絡先アイテムの検索を定義します。 この要素は省略できます。  <br/> |
|[GroupBy](groupby.md) <br/> |FindItem クエリの任意のグループ **化を** 指定します。 この要素は省略できます。  <br/> |
|[DistinguishedGroupBy](distinguishedgroupby.md) <br/> |FindItem クエリの標準的な **グループ化を** 提供します。 この要素は省略できます。  <br/> |
|[Restriction](restriction.md) <br/> |**FindItem** FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用する制限または /  クエリを定義します。 この要素は省略できます。  <br/> |
|[SortOrder](sortorder.md) <br/> |FindItem 要求でアイテムを並べ替える方法を定義します。 この要素は省略できます。  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |FindItem および FindFolder 操作を検索するフォルダーを識別します。  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |高度なクエリ構文 (AQS) に基づくメールボックス クエリ文字列が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

[IndexedPageItemView、FractionalPageItemView、CalendarView、](indexedpageitemview.md)または [](calendarview.md) [ContactsView](contactsview.md)要素の 1 つのみを **FindItem 要求に含** めできます。 [](fractionalpageitemview.md) FindItem 要求に含めるのは [、GroupBy](groupby.md) 要素または [DistinguishedGroupBy](distinguishedgroupby.md) 要素 **の 1 つ** のみです。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

