---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: SortBy 要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468398"
---
# <a name="sortby"></a><span data-ttu-id="6f302-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="6f302-103">SortBy</span></span>

<span data-ttu-id="6f302-104">**SortBy**要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f302-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="6f302-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="6f302-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f302-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6f302-106">Attributes and elements</span></span>

<span data-ttu-id="6f302-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f302-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f302-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f302-108">Attributes</span></span>

|<span data-ttu-id="6f302-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6f302-109">**Attribute**</span></span>|<span data-ttu-id="6f302-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f302-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f302-111">Order</span><span class="sxs-lookup"><span data-stu-id="6f302-111">Order</span></span>  <br/> |<span data-ttu-id="6f302-112">**Order**属性のテキスト値は、並べ替えの順序です。</span><span class="sxs-lookup"><span data-stu-id="6f302-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="6f302-113">テキスト値が**昇順**の場合は、結果が昇順になることを示します。</span><span class="sxs-lookup"><span data-stu-id="6f302-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="6f302-114">テキスト値が**降順**の場合は、結果が降順であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6f302-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6f302-115">子要素</span><span class="sxs-lookup"><span data-stu-id="6f302-115">Child elements</span></span>

<span data-ttu-id="6f302-116">[FieldURI](fielduri.md)  | [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="6f302-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f302-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6f302-117">Parent elements</span></span>

[<span data-ttu-id="6f302-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="6f302-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="6f302-119">注釈</span><span class="sxs-lookup"><span data-stu-id="6f302-119">Remarks</span></span>

<span data-ttu-id="6f302-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6f302-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6f302-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6f302-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f302-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6f302-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f302-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f302-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6f302-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f302-124">Schema name</span></span>  <br/> |<span data-ttu-id="6f302-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6f302-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6f302-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f302-126">Validation file</span></span>  <br/> |<span data-ttu-id="6f302-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6f302-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6f302-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f302-128">Can be empty</span></span>  <br/> ||
   

