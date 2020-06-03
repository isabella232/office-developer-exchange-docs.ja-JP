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
description: 会話要素は、単一の会話を表します。
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458937"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="cdefb-103">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="cdefb-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="cdefb-104">**会話**要素は、単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="cdefb-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="cdefb-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="cdefb-106">会話</span><span class="sxs-lookup"><span data-stu-id="cdefb-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="cdefb-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="cdefb-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
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

 <span data-ttu-id="cdefb-108">**ConversationType**</span><span class="sxs-lookup"><span data-stu-id="cdefb-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cdefb-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cdefb-109">Attributes and elements</span></span>

<span data-ttu-id="cdefb-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdefb-111">属性</span><span class="sxs-lookup"><span data-stu-id="cdefb-111">Attributes</span></span>

<span data-ttu-id="cdefb-112">なし。</span><span class="sxs-lookup"><span data-stu-id="cdefb-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdefb-113">子要素</span><span class="sxs-lookup"><span data-stu-id="cdefb-113">Child elements</span></span>

|<span data-ttu-id="cdefb-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="cdefb-114">**Element**</span></span>|<span data-ttu-id="cdefb-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="cdefb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdefb-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="cdefb-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="cdefb-117">会話の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="cdefb-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="cdefb-119">会話のトピックを表します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-119">Represents the conversation topic.</span></span> <span data-ttu-id="cdefb-120">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cdefb-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="cdefb-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="cdefb-122">特定のフォルダーから集約された会話の受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="cdefb-123">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cdefb-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="cdefb-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="cdefb-125">メールボックス全体で集約された会話の受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="cdefb-126">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cdefb-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="cdefb-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="cdefb-128">現在のフォルダーで、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="cdefb-129">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cdefb-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="cdefb-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="cdefb-131">メールボックス内のすべてのフォルダーにわたって、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="cdefb-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="cdefb-133">現在のフォルダー内のスレッドアイテムのすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="cdefb-134">この要素は値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cdefb-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="cdefb-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="cdefb-136">メールボックス内のスレッドアイテムのすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="cdefb-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="cdefb-138">現在のフォルダーで、このスレッドで最後に受信したメッセージの配信時刻を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="cdefb-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="cdefb-140">メールボックス内のすべてのフォルダーにわたって、この会話で最後に受信したメッセージの配信時刻を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-141">Categories</span><span class="sxs-lookup"><span data-stu-id="cdefb-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cdefb-142">現在のフォルダー内のすべての会話アイテムに適用されるカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="cdefb-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="cdefb-144">メールボックス内のすべての会話アイテムのカテゴリリストが保存されています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="cdefb-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="cdefb-146">現在のフォルダー内のスレッドアイテムの集約フラグの状態を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="cdefb-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="cdefb-148">メールボックス内のすべての会話アイテムの集約フラグの状態を格納します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="cdefb-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="cdefb-150">現在のフォルダー内の1つ以上の会話アイテムに添付ファイルがあるかどうかを示す値を格納します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="cdefb-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="cdefb-152">メールボックス内の少なくとも1つの会話アイテムに添付ファイルがあるかどうかを示す値を格納します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="cdefb-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="cdefb-154">現在のフォルダー内の会話アイテムの合計数が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="cdefb-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="cdefb-156">メールボックス内の会話アイテムの合計数が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="cdefb-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="cdefb-158">フォルダー内の未読の会話アイテムの数が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="cdefb-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="cdefb-160">メールボックス内のすべての未開封の会話アイテムの数を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-161">Size</span><span class="sxs-lookup"><span data-stu-id="cdefb-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="cdefb-162">現在のフォルダー内のすべての会話アイテムのサイズから計算された会話のサイズを格納します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="cdefb-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="cdefb-164">メールボックス内のすべての会話アイテムのサイズによって計算された会話のサイズを含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-165">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="cdefb-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="cdefb-166">現在のフォルダー内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="cdefb-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="cdefb-168">メールボックス内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-169">Importance</span><span class="sxs-lookup"><span data-stu-id="cdefb-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="cdefb-170">現在のフォルダー内のすべての会話アイテムの集約された重要度を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="cdefb-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="cdefb-172">メールボックス内のすべての会話アイテムの集約された重要度を含みます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-173">ItemIds</span><span class="sxs-lookup"><span data-stu-id="cdefb-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="cdefb-174">現在のフォルダー内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cdefb-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="cdefb-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="cdefb-176">メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdefb-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cdefb-177">親要素</span><span class="sxs-lookup"><span data-stu-id="cdefb-177">Parent elements</span></span>

|<span data-ttu-id="cdefb-178">**要素**</span><span class="sxs-lookup"><span data-stu-id="cdefb-178">**Element**</span></span>|<span data-ttu-id="cdefb-179">**説明**</span><span class="sxs-lookup"><span data-stu-id="cdefb-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdefb-180">会話</span><span class="sxs-lookup"><span data-stu-id="cdefb-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cdefb-181">**Findconversation**応答で返されるスレッドの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="cdefb-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cdefb-182">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cdefb-182">Text value</span></span>

<span data-ttu-id="cdefb-183">なし。</span><span class="sxs-lookup"><span data-stu-id="cdefb-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cdefb-184">注釈</span><span class="sxs-lookup"><span data-stu-id="cdefb-184">Remarks</span></span>

<span data-ttu-id="cdefb-185">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cdefb-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdefb-186">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cdefb-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdefb-187">Namespace</span><span class="sxs-lookup"><span data-stu-id="cdefb-187">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cdefb-188">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cdefb-188">Schema name</span></span>  <br/> |<span data-ttu-id="cdefb-189">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cdefb-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="cdefb-190">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cdefb-190">Validation file</span></span>  <br/> |<span data-ttu-id="cdefb-191">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cdefb-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cdefb-192">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cdefb-192">Can be empty</span></span>  <br/> |<span data-ttu-id="cdefb-193">正しくない</span><span class="sxs-lookup"><span data-stu-id="cdefb-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cdefb-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="cdefb-194">See also</span></span>



[<span data-ttu-id="cdefb-195">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="cdefb-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="cdefb-196">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="cdefb-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="cdefb-197">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="cdefb-197">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

