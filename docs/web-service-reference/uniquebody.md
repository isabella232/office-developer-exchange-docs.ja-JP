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
description: UniqueBody 要素は、html またはこのスレッドの一意の本文を表すテキストを表します。
ms.openlocfilehash: 49d3607926e0b985074d79cde76cad084f537f01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839789"
---
# <a name="uniquebody"></a><span data-ttu-id="57e59-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="57e59-103">UniqueBody</span></span>

<span data-ttu-id="57e59-104">**UniqueBody**要素は、html またはこのスレッドの一意の本文を表すテキストを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="57e59-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="57e59-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57e59-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57e59-106">Attributes and elements</span></span>

<span data-ttu-id="57e59-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57e59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57e59-108">属性</span><span class="sxs-lookup"><span data-stu-id="57e59-108">Attributes</span></span>

|<span data-ttu-id="57e59-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="57e59-109">**Attribute**</span></span>|<span data-ttu-id="57e59-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="57e59-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57e59-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="57e59-111">**BodyType**</span></span> <br/> |<span data-ttu-id="57e59-112">アイテムにアイテムの本文を格納する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="57e59-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="57e59-113">BodyType 属性</span><span class="sxs-lookup"><span data-stu-id="57e59-113">BodyType Attribute</span></span>

|<span data-ttu-id="57e59-114">**値**</span><span class="sxs-lookup"><span data-stu-id="57e59-114">**Value**</span></span>|<span data-ttu-id="57e59-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="57e59-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57e59-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="57e59-116">**HTML**</span></span> <br/> |<span data-ttu-id="57e59-117">すべての本文を HTML に変換します。</span><span class="sxs-lookup"><span data-stu-id="57e59-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="57e59-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="57e59-118">**Text**</span></span> <br/> |<span data-ttu-id="57e59-119">すべての本文をテキスト形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="57e59-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="57e59-120">子要素</span><span class="sxs-lookup"><span data-stu-id="57e59-120">Child elements</span></span>

<span data-ttu-id="57e59-121">なし。</span><span class="sxs-lookup"><span data-stu-id="57e59-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57e59-122">親要素</span><span class="sxs-lookup"><span data-stu-id="57e59-122">Parent elements</span></span>

|<span data-ttu-id="57e59-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="57e59-123">**Element**</span></span>|<span data-ttu-id="57e59-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="57e59-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57e59-125">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="57e59-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="57e59-126">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="57e59-127">Contact</span><span class="sxs-lookup"><span data-stu-id="57e59-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="57e59-128">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="57e59-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="57e59-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="57e59-130">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="57e59-131">アイテム</span><span class="sxs-lookup"><span data-stu-id="57e59-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="57e59-132">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="57e59-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="57e59-134">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="57e59-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="57e59-136">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="57e59-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="57e59-138">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="57e59-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="57e59-140">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-141">Message</span><span class="sxs-lookup"><span data-stu-id="57e59-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="57e59-142">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="57e59-143">PostItem</span><span class="sxs-lookup"><span data-stu-id="57e59-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="57e59-144">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="57e59-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="57e59-146">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="57e59-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="57e59-147">タスク</span><span class="sxs-lookup"><span data-stu-id="57e59-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="57e59-148">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="57e59-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57e59-149">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57e59-149">Text value</span></span>

<span data-ttu-id="57e59-150">なし。</span><span class="sxs-lookup"><span data-stu-id="57e59-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57e59-151">備考</span><span class="sxs-lookup"><span data-stu-id="57e59-151">Remarks</span></span>

<span data-ttu-id="57e59-152">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57e59-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57e59-153">要素情報</span><span class="sxs-lookup"><span data-stu-id="57e59-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57e59-154">名前空間</span><span class="sxs-lookup"><span data-stu-id="57e59-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57e59-155">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57e59-155">Schema Name</span></span>  <br/> |<span data-ttu-id="57e59-156">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="57e59-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="57e59-157">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57e59-157">Validation File</span></span>  <br/> |<span data-ttu-id="57e59-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57e59-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57e59-159">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57e59-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="57e59-160">False</span><span class="sxs-lookup"><span data-stu-id="57e59-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57e59-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="57e59-161">See also</span></span>



- [<span data-ttu-id="57e59-162">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="57e59-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

