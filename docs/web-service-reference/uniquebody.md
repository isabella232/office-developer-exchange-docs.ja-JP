---
title: UniqueBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueBody
api_type:
- schema
ms.assetid: 06bc95d7-121c-433b-bd27-c2b0eb8c011f
description: UniqueBody 要素は、この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。
ms.openlocfilehash: 0a8d52c7d4eb8bda9fd41c4c25e448523185df93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461920"
---
# <a name="uniquebody"></a><span data-ttu-id="d414f-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="d414f-103">UniqueBody</span></span>

<span data-ttu-id="d414f-104">**UniqueBody**要素は、この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="d414f-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="d414f-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d414f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d414f-106">Attributes and elements</span></span>

<span data-ttu-id="d414f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d414f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d414f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d414f-108">Attributes</span></span>

|<span data-ttu-id="d414f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d414f-109">**Attribute**</span></span>|<span data-ttu-id="d414f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d414f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d414f-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="d414f-111">**BodyType**</span></span> <br/> |<span data-ttu-id="d414f-112">アイテムにアイテムの本文を格納する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d414f-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="d414f-113">BodyType 属性</span><span class="sxs-lookup"><span data-stu-id="d414f-113">BodyType Attribute</span></span>

|<span data-ttu-id="d414f-114">**値**</span><span class="sxs-lookup"><span data-stu-id="d414f-114">**Value**</span></span>|<span data-ttu-id="d414f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d414f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d414f-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="d414f-116">**HTML**</span></span> <br/> |<span data-ttu-id="d414f-117">すべての本文を HTML に変換します。</span><span class="sxs-lookup"><span data-stu-id="d414f-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="d414f-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="d414f-118">**Text**</span></span> <br/> |<span data-ttu-id="d414f-119">すべての本文をテキスト形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="d414f-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d414f-120">子要素</span><span class="sxs-lookup"><span data-stu-id="d414f-120">Child elements</span></span>

<span data-ttu-id="d414f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="d414f-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d414f-122">親要素</span><span class="sxs-lookup"><span data-stu-id="d414f-122">Parent elements</span></span>

|<span data-ttu-id="d414f-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="d414f-123">**Element**</span></span>|<span data-ttu-id="d414f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="d414f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d414f-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d414f-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d414f-126">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d414f-127">Contact</span><span class="sxs-lookup"><span data-stu-id="d414f-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d414f-128">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d414f-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d414f-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d414f-130">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d414f-131">Item</span><span class="sxs-lookup"><span data-stu-id="d414f-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="d414f-132">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d414f-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d414f-134">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d414f-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d414f-136">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d414f-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d414f-138">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d414f-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d414f-140">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-141">Message</span><span class="sxs-lookup"><span data-stu-id="d414f-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d414f-142">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d414f-143">PostItem</span><span class="sxs-lookup"><span data-stu-id="d414f-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="d414f-144">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d414f-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d414f-146">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="d414f-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d414f-147">タスク</span><span class="sxs-lookup"><span data-stu-id="d414f-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="d414f-148">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d414f-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d414f-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d414f-149">Text value</span></span>

<span data-ttu-id="d414f-150">なし。</span><span class="sxs-lookup"><span data-stu-id="d414f-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d414f-151">注釈</span><span class="sxs-lookup"><span data-stu-id="d414f-151">Remarks</span></span>

<span data-ttu-id="d414f-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d414f-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d414f-153">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d414f-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d414f-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="d414f-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d414f-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d414f-155">Schema Name</span></span>  <br/> |<span data-ttu-id="d414f-156">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d414f-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="d414f-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d414f-157">Validation File</span></span>  <br/> |<span data-ttu-id="d414f-158">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d414f-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d414f-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d414f-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="d414f-160">正しくない</span><span class="sxs-lookup"><span data-stu-id="d414f-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d414f-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d414f-161">See also</span></span>



- [<span data-ttu-id="d414f-162">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d414f-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

