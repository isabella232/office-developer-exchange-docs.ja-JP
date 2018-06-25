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
description: カテゴリの要素には、メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。
ms.openlocfilehash: 8f112a9a736ff4f242b9dfb084b3ad7541cc493d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759615"
---
# <a name="categories"></a><span data-ttu-id="e1a86-103">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="e1a86-103">Categories</span></span>

<span data-ttu-id="e1a86-104">**カテゴリ**の要素には、メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1a86-104">The **Categories** element contains a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span> 
  
```XML
<Categories>
   <String/>
</Categories>
```

 <span data-ttu-id="e1a86-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e1a86-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1a86-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e1a86-106">Attributes and elements</span></span>

<span data-ttu-id="e1a86-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1a86-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1a86-108">Attributes</span></span>

<span data-ttu-id="e1a86-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e1a86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1a86-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e1a86-110">Child elements</span></span>

|<span data-ttu-id="e1a86-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1a86-111">**Element**</span></span>|<span data-ttu-id="e1a86-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1a86-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1a86-113">String</span><span class="sxs-lookup"><span data-stu-id="e1a86-113">String</span></span>](string.md) <br/> |<span data-ttu-id="e1a86-114">1 つのカテゴリを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1a86-114">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1a86-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e1a86-115">Parent elements</span></span>

|<span data-ttu-id="e1a86-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1a86-116">**Element**</span></span>|<span data-ttu-id="e1a86-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1a86-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1a86-118">Item</span><span class="sxs-lookup"><span data-stu-id="e1a86-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="e1a86-119">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-119">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e1a86-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e1a86-121">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-122">Message</span><span class="sxs-lookup"><span data-stu-id="e1a86-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e1a86-123">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-124">タスク</span><span class="sxs-lookup"><span data-stu-id="e1a86-124">Task</span></span>](task.md) <br/> |<span data-ttu-id="e1a86-125">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-125">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-126">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="e1a86-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e1a86-127">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-128">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e1a86-128">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e1a86-129">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-129">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-130">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e1a86-130">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e1a86-131">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-131">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-132">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e1a86-132">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e1a86-133">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-133">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-134">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e1a86-134">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e1a86-135">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-135">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e1a86-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e1a86-137">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-138">Contact</span><span class="sxs-lookup"><span data-stu-id="e1a86-138">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e1a86-139">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-139">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-140">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e1a86-140">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e1a86-141">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-141">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-142">条件</span><span class="sxs-lookup"><span data-stu-id="e1a86-142">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="e1a86-143">条件を表しますが、満たされるとときに、ルールのルールの処理をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="e1a86-143">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-144">Exceptions</span><span class="sxs-lookup"><span data-stu-id="e1a86-144">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="e1a86-145">受信トレイ ルールの使用可能なルールの例外条件をすべてを表します。</span><span class="sxs-lookup"><span data-stu-id="e1a86-145">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="e1a86-146">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="e1a86-146">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e1a86-147">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1a86-147">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1a86-148">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e1a86-148">Text value</span></span>

<span data-ttu-id="e1a86-149">なし。</span><span class="sxs-lookup"><span data-stu-id="e1a86-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1a86-150">備考</span><span class="sxs-lookup"><span data-stu-id="e1a86-150">Remarks</span></span>

<span data-ttu-id="e1a86-151">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e1a86-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1a86-152">要素情報</span><span class="sxs-lookup"><span data-stu-id="e1a86-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1a86-153">名前空間</span><span class="sxs-lookup"><span data-stu-id="e1a86-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1a86-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1a86-154">Schema Name</span></span>  <br/> |<span data-ttu-id="e1a86-155">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e1a86-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1a86-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1a86-156">Validation File</span></span>  <br/> |<span data-ttu-id="e1a86-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1a86-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1a86-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e1a86-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1a86-159">False</span><span class="sxs-lookup"><span data-stu-id="e1a86-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1a86-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1a86-160">See also</span></span>



- [<span data-ttu-id="e1a86-161">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e1a86-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

