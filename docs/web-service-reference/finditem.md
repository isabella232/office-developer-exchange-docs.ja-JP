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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460996"
---
# <a name="finditem"></a><span data-ttu-id="ed55a-103">FindItem</span><span class="sxs-lookup"><span data-stu-id="ed55a-103">FindItem</span></span>

<span data-ttu-id="ed55a-104">**FindItem**要素は、メールボックス内のアイテムを検索する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-104">The **FindItem** element defines a request to find items in a mailbox.</span></span> 
  
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


<span data-ttu-id="ed55a-105">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="ed55a-105">**FindItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ed55a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ed55a-106">Attributes and elements</span></span>

<span data-ttu-id="ed55a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed55a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed55a-108">Attributes</span></span>

|<span data-ttu-id="ed55a-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ed55a-109">**Attribute**</span></span>|<span data-ttu-id="ed55a-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed55a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed55a-111">**走査**</span><span class="sxs-lookup"><span data-stu-id="ed55a-111">**Traversal**</span></span> <br/> |<span data-ttu-id="ed55a-112">検索でフォルダー内のアイテムとフォルダーの dumpsters を検索するかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-112">Defines whether the search finds items in folders or the folders' dumpsters.</span></span> <span data-ttu-id="ed55a-113">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="ed55a-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="ed55a-114">トラバース属性値</span><span class="sxs-lookup"><span data-stu-id="ed55a-114">Traversal attribute values</span></span>

|<span data-ttu-id="ed55a-115">**値**</span><span class="sxs-lookup"><span data-stu-id="ed55a-115">**Value**</span></span>|<span data-ttu-id="ed55a-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed55a-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed55a-117">浅い</span><span class="sxs-lookup"><span data-stu-id="ed55a-117">Shallow</span></span>  <br/> |<span data-ttu-id="ed55a-118">フォルダー内のアイテムの id のみを返します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-118">Returns only the identities of items in the folder.</span></span>  <br/> |
|<span data-ttu-id="ed55a-119">削除済み (回復可能)</span><span class="sxs-lookup"><span data-stu-id="ed55a-119">SoftDeleted</span></span>  <br/> |<span data-ttu-id="ed55a-120">フォルダーの収集に含まれるアイテムの id のみを返します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-120">Returns only the identities of items that are in a folder's dumpster.</span></span> <span data-ttu-id="ed55a-121">検索条件に一致するアイテムが存在する場合でも、回復可能な削除によって削除された検査によって返されるアイテムが0個になることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ed55a-121">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned even if there are items that match the search criteria.</span></span>  <br/> |
|<span data-ttu-id="ed55a-122">関連</span><span class="sxs-lookup"><span data-stu-id="ed55a-122">Associated</span></span>  <br/> |<span data-ttu-id="ed55a-123">フォルダー内の関連付けられたアイテムの id のみを返します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-123">Returns only the identities of associated items in the folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ed55a-124">子要素</span><span class="sxs-lookup"><span data-stu-id="ed55a-124">Child elements</span></span>

|<span data-ttu-id="ed55a-125">**Element**</span><span class="sxs-lookup"><span data-stu-id="ed55a-125">**Element**</span></span>|<span data-ttu-id="ed55a-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed55a-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed55a-127">ItemShape</span><span class="sxs-lookup"><span data-stu-id="ed55a-127">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="ed55a-128">[FindItem 操作](finditem-operation.md)応答に含めるアイテムのプロパティとコンテンツを識別します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-128">Identifies the item properties and content to include in a [FindItem operation](finditem-operation.md) response.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-129">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="ed55a-129">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="ed55a-130">**FindItem**要求に対して、ページングされたアイテムの情報を返す方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-130">Describes how paged item information is returned for a **FindItem** request.</span></span> <span data-ttu-id="ed55a-131">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-131">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-132">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="ed55a-132">FractionalPageItemView</span></span>](fractionalpageitemview.md) <br/> |<span data-ttu-id="ed55a-133">ページビューの開始位置と、 **FindItem**要求で返されるアイテムの最大数を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-133">Describes where the paged view starts and the maximum number of items returned in a **FindItem** request.</span></span> <span data-ttu-id="ed55a-134">検索されたアイテムのセットの先頭からのページビューオフセットは、分数で示されます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-134">The paged view offset from the beginning of the set of found items is described by a fraction.</span></span> <span data-ttu-id="ed55a-135">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-136">CalendarView</span><span class="sxs-lookup"><span data-stu-id="ed55a-136">CalendarView</span></span>](calendarview.md) <br/> |<span data-ttu-id="ed55a-137">予定表アイテムの検索を定義するための時間範囲制限を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-137">Provides time span limits to define a search for calendar items.</span></span> <span data-ttu-id="ed55a-138">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-139">ContactsView</span><span class="sxs-lookup"><span data-stu-id="ed55a-139">ContactsView</span></span>](contactsview.md) <br/> |<span data-ttu-id="ed55a-140">アルファベットの表示名に基づいて、連絡先アイテムの検索を定義します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-140">Defines a search for contact items based on alphabetical display names.</span></span> <span data-ttu-id="ed55a-141">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-141">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-142">GroupBy</span><span class="sxs-lookup"><span data-stu-id="ed55a-142">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="ed55a-143">**FindItem**クエリの任意のグループを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-143">Specifies arbitrary groupings for **FindItem** queries.</span></span> <span data-ttu-id="ed55a-144">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-144">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-145">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="ed55a-145">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="ed55a-146">**FindItem**クエリの標準的なグループを提供します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-146">Provides standard groupings for **FindItem** queries.</span></span> <span data-ttu-id="ed55a-147">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-147">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-148">制限</span><span class="sxs-lookup"><span data-stu-id="ed55a-148">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="ed55a-149">**FindItem** /  **findfolder**および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを定義します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-149">Defines the restriction or query that is used to filter items or folders in **FindItem**/ **FindFolder** and search folder operations.</span></span> <span data-ttu-id="ed55a-150">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-150">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-151">SortOrder</span><span class="sxs-lookup"><span data-stu-id="ed55a-151">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="ed55a-152">FindItem 要求でのアイテムの並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-152">Defines how items are sorted in a FindItem request.</span></span> <span data-ttu-id="ed55a-153">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="ed55a-153">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-154">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="ed55a-154">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="ed55a-155">FindItem および FindFolder 操作を検索するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed55a-155">Identifies folders to search for the FindItem and FindFolder operations.</span></span>  <br/> |
|[<span data-ttu-id="ed55a-156">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="ed55a-156">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="ed55a-157">高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列が格納されています。</span><span class="sxs-lookup"><span data-stu-id="ed55a-157">Contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed55a-158">親要素</span><span class="sxs-lookup"><span data-stu-id="ed55a-158">Parent elements</span></span>

<span data-ttu-id="ed55a-159">なし。</span><span class="sxs-lookup"><span data-stu-id="ed55a-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed55a-160">注釈</span><span class="sxs-lookup"><span data-stu-id="ed55a-160">Remarks</span></span>

<span data-ttu-id="ed55a-161">**FindItem**要求に含めることができるのは、 [Indexedpageitemview](indexedpageitemview.md)、 [FractionalPageItemView](fractionalpageitemview.md)、 [CalendarView](calendarview.md)、または[ContactsView](contactsview.md)要素のいずれか1つだけです。</span><span class="sxs-lookup"><span data-stu-id="ed55a-161">Only one of the [IndexedPageItemView](indexedpageitemview.md), [FractionalPageItemView](fractionalpageitemview.md), [CalendarView](calendarview.md), or [ContactsView](contactsview.md) elements can be included in a **FindItem** request.</span></span> <span data-ttu-id="ed55a-162">**FindItem**要求に含めることができるのは、 [GroupBy](groupby.md)または[DistinguishedGroupBy](distinguishedgroupby.md)要素のいずれか1つだけです。</span><span class="sxs-lookup"><span data-stu-id="ed55a-162">Only one of the [GroupBy](groupby.md) or [DistinguishedGroupBy](distinguishedgroupby.md) elements can be included in a **FindItem** request.</span></span> 
  
<span data-ttu-id="ed55a-163">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ed55a-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed55a-164">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ed55a-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed55a-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed55a-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed55a-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed55a-166">Schema Name</span></span>  <br/> |<span data-ttu-id="ed55a-167">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ed55a-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ed55a-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed55a-168">Validation File</span></span>  <br/> |<span data-ttu-id="ed55a-169">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ed55a-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed55a-170">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed55a-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed55a-171">正しくない</span><span class="sxs-lookup"><span data-stu-id="ed55a-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed55a-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed55a-172">See also</span></span>

- [<span data-ttu-id="ed55a-173">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="ed55a-173">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="ed55a-174">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="ed55a-174">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

