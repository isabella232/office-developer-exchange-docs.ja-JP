---
title: カテゴリ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Categories
api_type:
- schema
ms.assetid: d84d4927-b524-4e62-bf3d-1f12fec8c21a
description: Categories 要素には、メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。
ms.openlocfilehash: 0d9f7068aa81306a10436ed0ca0d45f6d3b2c3a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462214"
---
# <a name="categories"></a><span data-ttu-id="b0918-103">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b0918-103">Categories</span></span>

<span data-ttu-id="b0918-104">**Categories**要素には、メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0918-104">The **Categories** element contains a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span> 
  
```XML
<Categories>
   <String/>
</Categories>
```

 <span data-ttu-id="b0918-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="b0918-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0918-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b0918-106">Attributes and elements</span></span>

<span data-ttu-id="b0918-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0918-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0918-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0918-108">Attributes</span></span>

<span data-ttu-id="b0918-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b0918-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0918-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b0918-110">Child elements</span></span>

|<span data-ttu-id="b0918-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b0918-111">**Element**</span></span>|<span data-ttu-id="b0918-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0918-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0918-113">String</span><span class="sxs-lookup"><span data-stu-id="b0918-113">String</span></span>](string.md) <br/> |<span data-ttu-id="b0918-114">1つのカテゴリを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="b0918-114">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0918-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b0918-115">Parent elements</span></span>

|<span data-ttu-id="b0918-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0918-116">**Element**</span></span>|<span data-ttu-id="b0918-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0918-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0918-118">Item</span><span class="sxs-lookup"><span data-stu-id="b0918-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="b0918-119">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-119">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b0918-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="b0918-121">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="b0918-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-122">Message</span><span class="sxs-lookup"><span data-stu-id="b0918-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0918-123">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b0918-124">タスク</span><span class="sxs-lookup"><span data-stu-id="b0918-124">Task</span></span>](task.md) <br/> |<span data-ttu-id="b0918-125">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-125">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b0918-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b0918-127">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b0918-128">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b0918-128">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b0918-129">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-129">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="b0918-130">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b0918-130">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b0918-131">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-131">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-132">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0918-132">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b0918-133">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-133">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-134">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0918-134">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b0918-135">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-135">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b0918-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b0918-137">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0918-138">Contact</span><span class="sxs-lookup"><span data-stu-id="b0918-138">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b0918-139">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-139">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="b0918-140">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b0918-140">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b0918-141">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-141">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="b0918-142">条件</span><span class="sxs-lookup"><span data-stu-id="b0918-142">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="b0918-143">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-143">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="b0918-144">例外</span><span class="sxs-lookup"><span data-stu-id="b0918-144">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="b0918-145">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="b0918-145">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="b0918-146">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="b0918-146">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="b0918-147">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b0918-147">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0918-148">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b0918-148">Text value</span></span>

<span data-ttu-id="b0918-149">なし。</span><span class="sxs-lookup"><span data-stu-id="b0918-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0918-150">注釈</span><span class="sxs-lookup"><span data-stu-id="b0918-150">Remarks</span></span>

<span data-ttu-id="b0918-151">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b0918-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0918-152">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b0918-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0918-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0918-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0918-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b0918-154">Schema Name</span></span>  <br/> |<span data-ttu-id="b0918-155">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b0918-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0918-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b0918-156">Validation File</span></span>  <br/> |<span data-ttu-id="b0918-157">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b0918-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0918-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b0918-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0918-159">正しくない</span><span class="sxs-lookup"><span data-stu-id="b0918-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0918-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0918-160">See also</span></span>



- [<span data-ttu-id="b0918-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0918-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

