---
title: 並べ替え
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: 並べ替えの要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833518"
---
# <a name="sortby"></a><span data-ttu-id="2793d-103">並べ替え</span><span class="sxs-lookup"><span data-stu-id="2793d-103">SortBy</span></span>

<span data-ttu-id="2793d-104">**並べ替え**の要素には、検索結果の並べ替えに使用されるアイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2793d-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="2793d-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="2793d-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2793d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2793d-106">Attributes and elements</span></span>

<span data-ttu-id="2793d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2793d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2793d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2793d-108">Attributes</span></span>

|<span data-ttu-id="2793d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2793d-109">**Attribute**</span></span>|<span data-ttu-id="2793d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2793d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2793d-111">Order</span><span class="sxs-lookup"><span data-stu-id="2793d-111">Order</span></span>  <br/> |<span data-ttu-id="2793d-112">**順序**属性のテキスト値は、並べ替え順序です。</span><span class="sxs-lookup"><span data-stu-id="2793d-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="2793d-113">**昇順**のテキスト値は、結果を昇順であることを示します。</span><span class="sxs-lookup"><span data-stu-id="2793d-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="2793d-114">**降順**のテキスト値は、結果が降順であることを示します。</span><span class="sxs-lookup"><span data-stu-id="2793d-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2793d-115">子要素</span><span class="sxs-lookup"><span data-stu-id="2793d-115">Child elements</span></span>

<span data-ttu-id="2793d-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="2793d-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2793d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2793d-117">Parent elements</span></span>

[<span data-ttu-id="2793d-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="2793d-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="2793d-119">備考</span><span class="sxs-lookup"><span data-stu-id="2793d-119">Remarks</span></span>

<span data-ttu-id="2793d-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2793d-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2793d-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2793d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2793d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="2793d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2793d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="2793d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2793d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2793d-124">Schema name</span></span>  <br/> |<span data-ttu-id="2793d-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2793d-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2793d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2793d-126">Validation file</span></span>  <br/> |<span data-ttu-id="2793d-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2793d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2793d-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2793d-128">Can be empty</span></span>  <br/> ||
   

