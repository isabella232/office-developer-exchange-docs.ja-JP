---
title: Importance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Importance
api_type:
- schema
ms.assetid: 1557f59a-41f2-43fb-9ded-88f3ec5c76cb
description: 重要度要素は、現在のフォルダー内のスレッドの重要度またはスレッドのすべてのアイテムの集約された重要度を表します。
ms.openlocfilehash: c49d6e84a41f1eb546eef19e2e7279fdb30b48e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464792"
---
# <a name="importance"></a><span data-ttu-id="6ddda-103">Importance</span><span class="sxs-lookup"><span data-stu-id="6ddda-103">Importance</span></span>

<span data-ttu-id="6ddda-104">**重要度**要素は、現在のフォルダー内のスレッドの重要度またはスレッドのすべてのアイテムの集約された重要度を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-104">The **Importance** element describes the importance of an item or the aggregated importance of all items in a conversation in the current folder.</span></span> 
  
```XML
<Importance/>
```

 <span data-ttu-id="6ddda-105">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="6ddda-105">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ddda-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6ddda-106">Attributes and elements</span></span>

<span data-ttu-id="6ddda-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ddda-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ddda-108">Attributes</span></span>

<span data-ttu-id="6ddda-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6ddda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ddda-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6ddda-110">Child elements</span></span>

<span data-ttu-id="6ddda-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6ddda-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ddda-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6ddda-112">Parent elements</span></span>

|<span data-ttu-id="6ddda-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ddda-113">**Element**</span></span>|<span data-ttu-id="6ddda-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ddda-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ddda-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="6ddda-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6ddda-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-117">条件</span><span class="sxs-lookup"><span data-stu-id="6ddda-117">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6ddda-118">そのルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-118">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6ddda-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6ddda-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-120">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-121">連絡先</span><span class="sxs-lookup"><span data-stu-id="6ddda-121">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6ddda-122">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-122">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="6ddda-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="6ddda-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-125">例外</span><span class="sxs-lookup"><span data-stu-id="6ddda-125">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6ddda-126">受信トレイルールの使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-126">Represents the exceptions that represent all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-127">アイテム</span><span class="sxs-lookup"><span data-stu-id="6ddda-127">Item</span></span>](item.md) <br/> |<span data-ttu-id="6ddda-128">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-128">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="6ddda-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6ddda-130">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-131">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="6ddda-131">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6ddda-132">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-132">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-133">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6ddda-133">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6ddda-134">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-134">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-135">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6ddda-135">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6ddda-136">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-136">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-137">Message</span><span class="sxs-lookup"><span data-stu-id="6ddda-137">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6ddda-138">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-138">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-139">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="6ddda-139">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="6ddda-140">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-140">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6ddda-141">Task</span><span class="sxs-lookup"><span data-stu-id="6ddda-141">Task</span></span>](task.md) <br/> |<span data-ttu-id="6ddda-142">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="6ddda-142">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ddda-143">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6ddda-143">Text value</span></span>

<span data-ttu-id="6ddda-144">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="6ddda-144">A text value is required.</span></span> <span data-ttu-id="6ddda-145">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6ddda-145">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="6ddda-146">低</span><span class="sxs-lookup"><span data-stu-id="6ddda-146">Low</span></span>
    
- <span data-ttu-id="6ddda-147">標準</span><span class="sxs-lookup"><span data-stu-id="6ddda-147">Normal</span></span>
    
- <span data-ttu-id="6ddda-148">高</span><span class="sxs-lookup"><span data-stu-id="6ddda-148">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6ddda-149">注釈</span><span class="sxs-lookup"><span data-stu-id="6ddda-149">Remarks</span></span>

<span data-ttu-id="6ddda-150">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6ddda-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ddda-151">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6ddda-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ddda-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ddda-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ddda-153">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6ddda-153">Schema Name</span></span>  <br/> |<span data-ttu-id="6ddda-154">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6ddda-154">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ddda-155">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6ddda-155">Validation File</span></span>  <br/> |<span data-ttu-id="6ddda-156">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6ddda-156">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ddda-157">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6ddda-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ddda-158">正しくない</span><span class="sxs-lookup"><span data-stu-id="6ddda-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ddda-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ddda-159">See also</span></span>



- [<span data-ttu-id="6ddda-160">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6ddda-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

