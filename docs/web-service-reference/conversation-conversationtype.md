---
title: 会話 (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: テーマ要素は、1 つのテーマを表します。
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759754"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="f099f-103">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f099f-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="f099f-104">**テーマ**要素は、1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="f099f-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="f099f-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="f099f-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f099f-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="f099f-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f099f-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f099f-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 <span data-ttu-id="f099f-108">**ConversationType**</span><span class="sxs-lookup"><span data-stu-id="f099f-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f099f-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f099f-109">Attributes and elements</span></span>

<span data-ttu-id="f099f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f099f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f099f-111">属性</span><span class="sxs-lookup"><span data-stu-id="f099f-111">Attributes</span></span>

<span data-ttu-id="f099f-112">なし。</span><span class="sxs-lookup"><span data-stu-id="f099f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f099f-113">子要素</span><span class="sxs-lookup"><span data-stu-id="f099f-113">Child elements</span></span>

|<span data-ttu-id="f099f-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="f099f-114">**Element**</span></span>|<span data-ttu-id="f099f-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="f099f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f099f-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="f099f-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="f099f-117">スレッドの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f099f-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="f099f-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="f099f-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="f099f-119">会話のトピックを表します。</span><span class="sxs-lookup"><span data-stu-id="f099f-119">Represents the conversation topic.</span></span> <span data-ttu-id="f099f-120">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f099f-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f099f-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="f099f-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="f099f-122">特定のフォルダーから集約された会話の宛先のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="f099f-123">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f099f-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f099f-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="f099f-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="f099f-125">メールボックス間で集計する対話の受信者のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="f099f-126">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f099f-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f099f-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="f099f-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="f099f-128">現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="f099f-129">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f099f-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f099f-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="f099f-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="f099f-131">現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="f099f-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="f099f-133">会話項目を現在のフォルダー内のすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="f099f-134">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f099f-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f099f-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="f099f-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="f099f-136">メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="f099f-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="f099f-138">現在のフォルダーには、この会話の最後に受信したメッセージの配信時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="f099f-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="f099f-140">メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-141">Categories</span><span class="sxs-lookup"><span data-stu-id="f099f-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f099f-142">現在のフォルダー内のすべての会話項目に適用されるカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="f099f-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="f099f-144">メールボックス内のすべての会話項目のカテゴリの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-145">フラグ</span><span class="sxs-lookup"><span data-stu-id="f099f-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="f099f-146">テーマ フォルダー内のアイテムの現在の集計のフラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="f099f-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="f099f-148">メールボックス内のすべての会話項目の集計のフラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-149">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="f099f-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="f099f-150">添付ファイルを現在のフォルダーに項目を少なくとも 1 つのテーマがあるかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="f099f-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="f099f-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="f099f-152">メールボックス内の少なくとも 1 つのテーマのアイテムに添付ファイルがあるかどうかを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="f099f-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="f099f-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="f099f-154">現在のフォルダー内の会話の項目の合計数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="f099f-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="f099f-156">会話メールボックス内のアイテムの合計数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="f099f-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="f099f-158">フォルダー内のアイテムを未読の会話の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="f099f-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="f099f-160">メールボックス内のすべての未読の会話項目の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-161">Size</span><span class="sxs-lookup"><span data-stu-id="f099f-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="f099f-162">現在のフォルダー内のすべての会話項目のサイズから計算された会話のサイズが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="f099f-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="f099f-164">メールボックス内のすべての会話アイテムのサイズから計算された会話のサイズが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-165">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="f099f-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="f099f-166">会話の項目の現在のフォルダーのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="f099f-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="f099f-168">会話内のアイテムをメールボックスのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-169">Importance</span><span class="sxs-lookup"><span data-stu-id="f099f-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="f099f-170">集計の重要性現在のフォルダー内のすべての会話項目にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="f099f-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="f099f-172">メールボックス内のすべての会話項目の集計の重要性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f099f-173">Itemid</span><span class="sxs-lookup"><span data-stu-id="f099f-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="f099f-174">現在のフォルダー内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f099f-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="f099f-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="f099f-176">メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f099f-177">親要素</span><span class="sxs-lookup"><span data-stu-id="f099f-177">Parent elements</span></span>

|<span data-ttu-id="f099f-178">**要素**</span><span class="sxs-lookup"><span data-stu-id="f099f-178">**Element**</span></span>|<span data-ttu-id="f099f-179">**説明**</span><span class="sxs-lookup"><span data-stu-id="f099f-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f099f-180">スレッド</span><span class="sxs-lookup"><span data-stu-id="f099f-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f099f-181">**FindConversation**の応答で返される会話の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f099f-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f099f-182">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f099f-182">Text value</span></span>

<span data-ttu-id="f099f-183">なし。</span><span class="sxs-lookup"><span data-stu-id="f099f-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f099f-184">備考</span><span class="sxs-lookup"><span data-stu-id="f099f-184">Remarks</span></span>

<span data-ttu-id="f099f-185">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f099f-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f099f-186">要素情報</span><span class="sxs-lookup"><span data-stu-id="f099f-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f099f-187">名前空間</span><span class="sxs-lookup"><span data-stu-id="f099f-187">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f099f-188">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f099f-188">Schema name</span></span>  <br/> |<span data-ttu-id="f099f-189">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f099f-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="f099f-190">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f099f-190">Validation file</span></span>  <br/> |<span data-ttu-id="f099f-191">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f099f-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f099f-192">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f099f-192">Can be empty</span></span>  <br/> |<span data-ttu-id="f099f-193">False</span><span class="sxs-lookup"><span data-stu-id="f099f-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f099f-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="f099f-194">See also</span></span>



<span data-ttu-id="f099f-195">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="f099f-195">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="f099f-196">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="f099f-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="f099f-197">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="f099f-197">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

