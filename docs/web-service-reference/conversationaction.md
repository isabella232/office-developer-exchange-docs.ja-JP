---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: ConversationAction 要素には、単一の会話に適用される1つのアクションが含まれています。
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529253"
---
# <a name="conversationaction"></a><span data-ttu-id="82602-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="82602-103">ConversationAction</span></span>

<span data-ttu-id="82602-104">**ConversationAction**要素には、単一の会話に適用される1つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="82602-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="82602-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="82602-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="82602-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="82602-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="82602-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="82602-107">ConversationAction</span></span>](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 <span data-ttu-id="82602-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="82602-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82602-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="82602-109">Attributes and elements</span></span>

<span data-ttu-id="82602-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82602-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82602-111">属性</span><span class="sxs-lookup"><span data-stu-id="82602-111">Attributes</span></span>

<span data-ttu-id="82602-112">なし。</span><span class="sxs-lookup"><span data-stu-id="82602-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82602-113">子要素</span><span class="sxs-lookup"><span data-stu-id="82602-113">Child elements</span></span>

|<span data-ttu-id="82602-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="82602-114">**Element**</span></span>|<span data-ttu-id="82602-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="82602-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82602-116">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="82602-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="82602-117">[ConversationId](conversationid.md)要素によって指定された会話に対して実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="82602-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="82602-118">この要素が存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="82602-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="82602-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="82602-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="82602-120">スレッドのアイテムに適用される[action (ConversationActionTypeType)](action-conversationactiontypetype.md)要素によって指定されたアクションを実行する会話の識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="82602-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="82602-121">この要素が存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="82602-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="82602-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="82602-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="82602-123">フォルダーを使用する操作を対象とするフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="82602-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="82602-124">この要素は、ターゲットフォルダー内の会話アイテムのコピー、削除、移動、および読み取り状態の設定時に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="82602-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="82602-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="82602-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="82602-126">会話が最後に同期された日付と時刻が含まれます。</span><span class="sxs-lookup"><span data-stu-id="82602-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="82602-127">この要素は、指定された時刻までに受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="82602-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="82602-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="82602-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="82602-129">アクションがサーバー上での処理を開始するとすぐに応答が送信されるか、またはアクションの完了後に応答が送信されるかを示します。</span><span class="sxs-lookup"><span data-stu-id="82602-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="82602-130">この要素は、要求されたアクションに応答を非同期送信するために存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="82602-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="82602-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="82602-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="82602-132">コピー操作と移動操作の宛先フォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="82602-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="82602-133">Categories</span><span class="sxs-lookup"><span data-stu-id="82602-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="82602-134">会話内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="82602-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="82602-135">Enablealways Delete</span><span class="sxs-lookup"><span data-stu-id="82602-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="82602-136">スレッド内のすべての新規アイテムの削除を有効にするフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="82602-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="82602-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="82602-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="82602-138">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="82602-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="82602-139">DeleteType</span><span class="sxs-lookup"><span data-stu-id="82602-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="82602-140">スレッド内のアイテムが削除される方法を示します。</span><span class="sxs-lookup"><span data-stu-id="82602-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="82602-141">親要素</span><span class="sxs-lookup"><span data-stu-id="82602-141">Parent elements</span></span>

|<span data-ttu-id="82602-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="82602-142">**Element**</span></span>|<span data-ttu-id="82602-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="82602-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82602-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="82602-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="82602-145">会話のコレクションと、それらに適用するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="82602-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82602-146">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82602-146">Text value</span></span>

<span data-ttu-id="82602-147">**ConversationAction 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="82602-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="82602-148">**値**</span><span class="sxs-lookup"><span data-stu-id="82602-148">**Value**</span></span>|<span data-ttu-id="82602-149">**説明**</span><span class="sxs-lookup"><span data-stu-id="82602-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82602-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="82602-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="82602-151">常に会話を分類します。</span><span class="sxs-lookup"><span data-stu-id="82602-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-152">常に削除</span><span class="sxs-lookup"><span data-stu-id="82602-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="82602-153">常に会話を削除します。</span><span class="sxs-lookup"><span data-stu-id="82602-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-154">常に移動</span><span class="sxs-lookup"><span data-stu-id="82602-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="82602-155">常に会話を移動します。</span><span class="sxs-lookup"><span data-stu-id="82602-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-156">削除</span><span class="sxs-lookup"><span data-stu-id="82602-156">Delete</span></span>  <br/> |<span data-ttu-id="82602-157">会話を削除します。</span><span class="sxs-lookup"><span data-stu-id="82602-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-158">Move</span><span class="sxs-lookup"><span data-stu-id="82602-158">Move</span></span>  <br/> |<span data-ttu-id="82602-159">会話を移動します。</span><span class="sxs-lookup"><span data-stu-id="82602-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-160">Copy</span><span class="sxs-lookup"><span data-stu-id="82602-160">Copy</span></span>  <br/> |<span data-ttu-id="82602-161">会話をコピーします。</span><span class="sxs-lookup"><span data-stu-id="82602-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="82602-162">SetReadState</span></span>  <br/> |<span data-ttu-id="82602-163">会話の読み取り状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="82602-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="82602-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="82602-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="82602-165">会話のアイテム保持ポリシーを設定します。</span><span class="sxs-lookup"><span data-stu-id="82602-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="82602-166">注釈</span><span class="sxs-lookup"><span data-stu-id="82602-166">Remarks</span></span>

<span data-ttu-id="82602-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="82602-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82602-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="82602-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82602-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="82602-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82602-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82602-170">Schema Name</span></span>  <br/> |<span data-ttu-id="82602-171">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="82602-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="82602-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82602-172">Validation File</span></span>  <br/> |<span data-ttu-id="82602-173">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="82602-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82602-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82602-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="82602-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="82602-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82602-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="82602-176">See also</span></span>



[<span data-ttu-id="82602-177">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="82602-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="82602-178">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="82602-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

