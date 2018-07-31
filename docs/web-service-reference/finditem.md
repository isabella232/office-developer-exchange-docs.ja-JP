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
# <a name="finditem"></a><span data-ttu-id="66d8c-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="66d8c-103">FindItem</span></span>

<span data-ttu-id="66d8c-104">**FindItem**要素では、メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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


<span data-ttu-id="66d8c-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="66d8c-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66d8c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="66d8c-106">Attributes and elements</span></span>

<span data-ttu-id="66d8c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66d8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="66d8c-108">Attributes</span></span>

|<span data-ttu-id="66d8c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="66d8c-109">**Attribute**</span></span>|<span data-ttu-id="66d8c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="66d8c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66d8c-111">**トラバーサル**</span><span class="sxs-lookup"><span data-stu-id="66d8c-111">**Traversal**</span></span> <br/> |<span data-ttu-id="66d8c-112">検索がフォルダーまたはフォルダーの dumpsters でアイテムを検索するかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="66d8c-113">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="66d8c-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="66d8c-114">検査の属性値</span><span class="sxs-lookup"><span data-stu-id="66d8c-114">Traversal attribute values</span></span>

|<span data-ttu-id="66d8c-115">**値**</span><span class="sxs-lookup"><span data-stu-id="66d8c-115">**Value**</span></span>|<span data-ttu-id="66d8c-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="66d8c-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66d8c-117">浅い</span><span class="sxs-lookup"><span data-stu-id="66d8c-117">Shallow</span></span>  <br/> |<span data-ttu-id="66d8c-118">フォルダー内のアイテムの id だけを返します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="66d8c-119">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="66d8c-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="66d8c-120">フォルダーの内にあるアイテムの id だけを返します。 ごみ箱をあさる。</span><span class="sxs-lookup"><span data-stu-id="66d8c-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="66d8c-121">ノートの検索の制限と組み合わせて、ソフト削除走査返される項目が 0 の原因になる場合でも、検索条件に一致する項目があります。</span><span class="sxs-lookup"><span data-stu-id="66d8c-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="66d8c-122">関連</span><span class="sxs-lookup"><span data-stu-id="66d8c-122">Associated</span></span>  <br/> |<span data-ttu-id="66d8c-123">フォルダーに関連付けられているアイテムの id だけを返します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66d8c-124">子要素</span><span class="sxs-lookup"><span data-stu-id="66d8c-124">Child elements</span></span>

|<span data-ttu-id="66d8c-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="66d8c-125">**Element**</span></span>|<span data-ttu-id="66d8c-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="66d8c-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66d8c-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="66d8c-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="66d8c-128">[FindItem 操作](finditem-operation.md)の応答に含めるコンテンツ アイテムのプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="66d8c-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="66d8c-130">どのページの項目の情報について説明します**FindItem**要求に対して返されます。</span><span class="sxs-lookup"><span data-stu-id="66d8c-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="66d8c-131">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="66d8c-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="66d8c-133">ページ ビューが開始され**FindItem**要求内のアイテムの最大数が返されるをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="66d8c-134">見つかった項目のセットの先頭からのページ ビュー オフセットは、分数で表されます。</span><span class="sxs-lookup"><span data-stu-id="66d8c-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="66d8c-135">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="66d8c-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="66d8c-137">時間は、予定表アイテムの検索を定義する制限に 。</span><span class="sxs-lookup"><span data-stu-id="66d8c-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="66d8c-138">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="66d8c-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="66d8c-140">連絡先アイテムをアルファベット順の表示名を基に検索を定義します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="66d8c-141">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="66d8c-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="66d8c-143">**FindItem**クエリの任意のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="66d8c-144">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="66d8c-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="66d8c-146">**FindItem**クエリの標準的なグループ化を提供します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="66d8c-147">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-148">Restriction</span><span class="sxs-lookup"><span data-stu-id="66d8c-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="66d8c-149">制限またはアイテムや**FindItem**内のフォルダーにフィルターを使用するクエリを定義する/ **FindFolder**検索フォルダーの操作です。</span><span class="sxs-lookup"><span data-stu-id="66d8c-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="66d8c-150">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="66d8c-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="66d8c-152">FindItem 要求内のアイテムの並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="66d8c-153">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="66d8c-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="66d8c-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="66d8c-155">FindItem と FindFolder 操作を検索するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="66d8c-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="66d8c-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="66d8c-157">ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66d8c-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66d8c-158">親要素</span><span class="sxs-lookup"><span data-stu-id="66d8c-158">Parent elements</span></span>

<span data-ttu-id="66d8c-159">なし。</span><span class="sxs-lookup"><span data-stu-id="66d8c-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66d8c-160">注釈</span><span class="sxs-lookup"><span data-stu-id="66d8c-160">Remarks</span></span>

<span data-ttu-id="66d8c-161">**FindItem**要求で、 [IndexedPageItemView](indexedpageitemview.md)、 [FractionalPageItemView](fractionalpageitemview.md)、[予定表ビュー](calendarview.md)、または[ContactsView](contactsview.md)要素の 1 つだけ含まれていることができます。</span><span class="sxs-lookup"><span data-stu-id="66d8c-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="66d8c-162">**FindItem**要求で[GroupBy](groupby.md)または[DistinguishedGroupBy](distinguishedgroupby.md)要素の 1 つだけ含まれていることができます。</span><span class="sxs-lookup"><span data-stu-id="66d8c-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="66d8c-163">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="66d8c-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66d8c-164">要素情報</span><span class="sxs-lookup"><span data-stu-id="66d8c-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66d8c-165">名前空間</span><span class="sxs-lookup"><span data-stu-id="66d8c-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66d8c-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66d8c-166">Schema Name</span></span>  <br/> |<span data-ttu-id="66d8c-167">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="66d8c-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66d8c-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66d8c-168">Validation File</span></span>  <br/> |<span data-ttu-id="66d8c-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66d8c-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66d8c-170">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="66d8c-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="66d8c-171">False</span><span class="sxs-lookup"><span data-stu-id="66d8c-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66d8c-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="66d8c-172">See also</span></span>

- <span data-ttu-id="66d8c-173">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="66d8c-173">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="66d8c-174">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="66d8c-174">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

