---
title: 本文
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Body 要素は、アイテムの本文を指定します。
ms.openlocfilehash: c565c5701ae5bc210cf0a9dc694108752860e24b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529491"
---
# <a name="body"></a><span data-ttu-id="1ca48-103">本文</span><span class="sxs-lookup"><span data-stu-id="1ca48-103">Body</span></span>

<span data-ttu-id="1ca48-104">**Body**要素は、アイテムの本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-104">The **Body** element specifies the body of an item.</span></span> 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 <span data-ttu-id="1ca48-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="1ca48-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ca48-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1ca48-106">Attributes and elements</span></span>

<span data-ttu-id="1ca48-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ca48-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ca48-108">Attributes</span></span>

|<span data-ttu-id="1ca48-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1ca48-109">**Attribute**</span></span>|<span data-ttu-id="1ca48-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ca48-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ca48-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="1ca48-111">BodyType</span></span>  <br/> |<span data-ttu-id="1ca48-112">本文の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-112">Specifies the type of the body.</span></span>  <br/> |
|<span data-ttu-id="1ca48-113">Istrがありません</span><span class="sxs-lookup"><span data-stu-id="1ca48-113">IsTruncated</span></span>  <br/> |<span data-ttu-id="1ca48-114">本文が切り捨てられるかどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="1ca48-114">Boolean value that indicates whether the body is truncated.</span></span>  <br/> |
   
#### <a name="bodytype"></a><span data-ttu-id="1ca48-115">BodyType</span><span class="sxs-lookup"><span data-stu-id="1ca48-115">BodyType</span></span>

|<span data-ttu-id="1ca48-116">**値**</span><span class="sxs-lookup"><span data-stu-id="1ca48-116">**Value**</span></span>|<span data-ttu-id="1ca48-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ca48-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ca48-118">HTML</span><span class="sxs-lookup"><span data-stu-id="1ca48-118">HTML</span></span>  <br/> |<span data-ttu-id="1ca48-119">本文が HTML 形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-119">Indicates that the body is in HTML.</span></span>  <br/> |
|<span data-ttu-id="1ca48-120">テキスト</span><span class="sxs-lookup"><span data-stu-id="1ca48-120">Text</span></span>  <br/> |<span data-ttu-id="1ca48-121">本文がテキストにあることを示します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-121">Indicates that the body is in text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1ca48-122">子要素</span><span class="sxs-lookup"><span data-stu-id="1ca48-122">Child elements</span></span>

<span data-ttu-id="1ca48-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1ca48-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ca48-124">親要素</span><span class="sxs-lookup"><span data-stu-id="1ca48-124">Parent elements</span></span>

|<span data-ttu-id="1ca48-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ca48-125">**Element**</span></span>|<span data-ttu-id="1ca48-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ca48-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ca48-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="1ca48-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="1ca48-128">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-129">Contact</span><span class="sxs-lookup"><span data-stu-id="1ca48-129">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="1ca48-130">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-130">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-131">DistributionList</span><span class="sxs-lookup"><span data-stu-id="1ca48-131">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="1ca48-132">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-132">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-133">Item</span><span class="sxs-lookup"><span data-stu-id="1ca48-133">Item</span></span>](item.md) <br/> |<span data-ttu-id="1ca48-134">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-134">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-135">Message</span><span class="sxs-lookup"><span data-stu-id="1ca48-135">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1ca48-136">Microsoft Exchange の電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-136">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-137">PostItem</span><span class="sxs-lookup"><span data-stu-id="1ca48-137">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="1ca48-138">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-138">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1ca48-139">タスク</span><span class="sxs-lookup"><span data-stu-id="1ca48-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="1ca48-140">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca48-140">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ca48-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1ca48-141">Text value</span></span>

<span data-ttu-id="1ca48-142">**Body**要素のテキスト値は、アイテムの本文の内容です。</span><span class="sxs-lookup"><span data-stu-id="1ca48-142">The text value of the **Body** element is the body content of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1ca48-143">注釈</span><span class="sxs-lookup"><span data-stu-id="1ca48-143">Remarks</span></span>

<span data-ttu-id="1ca48-144">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1ca48-144">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1ca48-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ca48-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ca48-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1ca48-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ca48-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ca48-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ca48-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ca48-148">Schema Name</span></span>  <br/> |<span data-ttu-id="1ca48-149">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1ca48-149">Type schema</span></span>  <br/> |
|<span data-ttu-id="1ca48-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ca48-150">Validation File</span></span>  <br/> |<span data-ttu-id="1ca48-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1ca48-151">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ca48-152">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1ca48-152">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1ca48-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ca48-153">See also</span></span>



- [<span data-ttu-id="1ca48-154">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ca48-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

