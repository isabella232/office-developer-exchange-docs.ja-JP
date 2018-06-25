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
description: ConversationAction 要素には、1 つのテーマを適用する 1 つのアクションが含まれています。
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759753"
---
# <a name="conversationaction"></a><span data-ttu-id="54884-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="54884-103">ConversationAction</span></span>

<span data-ttu-id="54884-104">**ConversationAction**要素には、1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="54884-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="54884-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="54884-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="54884-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="54884-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="54884-107">ConversationAction</span></span>](conversationaction.md)
  
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

 <span data-ttu-id="54884-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="54884-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54884-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="54884-109">Attributes and elements</span></span>

<span data-ttu-id="54884-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54884-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54884-111">属性</span><span class="sxs-lookup"><span data-stu-id="54884-111">Attributes</span></span>

<span data-ttu-id="54884-112">なし。</span><span class="sxs-lookup"><span data-stu-id="54884-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54884-113">子要素</span><span class="sxs-lookup"><span data-stu-id="54884-113">Child elements</span></span>

|<span data-ttu-id="54884-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="54884-114">**Element**</span></span>|<span data-ttu-id="54884-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="54884-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54884-116">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="54884-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="54884-117">[ConversationId](conversationid.md)要素で指定されたスレッド上で実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="54884-118">この要素が存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54884-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="54884-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="54884-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="54884-120">会話内のアイテムに適用される[アクション (ConversationActionTypeType)](action-conversationactiontypetype.md)の要素によって指定されたアクションがある会話スレッドの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="54884-121">この要素が存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54884-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="54884-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="54884-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="54884-123">フォルダーを使用する操作を対象としているフォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="54884-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="54884-124">この要素は、コピー、削除、移動、およびターゲット フォルダー内のアイテムの会話の読み取り状態を設定するときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54884-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="54884-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="54884-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="54884-126">会話が最後に同期された日時が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="54884-127">この要素は、会話で指定した時刻までに受信したすべてのアイテムを削除しようとするときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54884-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="54884-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="54884-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="54884-129">アクションがサーバーまたはアクションが完了した後に応答を送信するかどうかで処理を開始すると、すぐに応答を送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="54884-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="54884-130">この要素は、要求された操作を非同期に送信する応答のために存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="54884-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="54884-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="54884-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="54884-132">コピー先のフォルダーを指定し、アクションを移動します。</span><span class="sxs-lookup"><span data-stu-id="54884-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="54884-133">Categories</span><span class="sxs-lookup"><span data-stu-id="54884-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="54884-134">会話内の項目が所属するカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="54884-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="54884-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="54884-136">会話内のすべての新しいアイテムの削除を有効にするフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="54884-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="54884-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="54884-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="54884-138">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="54884-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="54884-139">削除の種類</span><span class="sxs-lookup"><span data-stu-id="54884-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="54884-140">会話内の項目を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="54884-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54884-141">親要素</span><span class="sxs-lookup"><span data-stu-id="54884-141">Parent elements</span></span>

|<span data-ttu-id="54884-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="54884-142">**Element**</span></span>|<span data-ttu-id="54884-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="54884-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54884-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="54884-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="54884-145">会話およびそれらに適用するアクションのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="54884-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54884-146">テキスト値</span><span class="sxs-lookup"><span data-stu-id="54884-146">Text value</span></span>

<span data-ttu-id="54884-147">**ConversationAction 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="54884-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="54884-148">**値**</span><span class="sxs-lookup"><span data-stu-id="54884-148">**Value**</span></span>|<span data-ttu-id="54884-149">**説明**</span><span class="sxs-lookup"><span data-stu-id="54884-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54884-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="54884-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="54884-151">会話を常に分類します。</span><span class="sxs-lookup"><span data-stu-id="54884-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="54884-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="54884-153">会話を常に削除します。</span><span class="sxs-lookup"><span data-stu-id="54884-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="54884-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="54884-155">会話を常に移動します。</span><span class="sxs-lookup"><span data-stu-id="54884-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-156">削除</span><span class="sxs-lookup"><span data-stu-id="54884-156">Delete</span></span>  <br/> |<span data-ttu-id="54884-157">会話を削除します。</span><span class="sxs-lookup"><span data-stu-id="54884-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-158">移動</span><span class="sxs-lookup"><span data-stu-id="54884-158">Move</span></span>  <br/> |<span data-ttu-id="54884-159">会話に移動します。</span><span class="sxs-lookup"><span data-stu-id="54884-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-160">Copy</span><span class="sxs-lookup"><span data-stu-id="54884-160">Copy</span></span>  <br/> |<span data-ttu-id="54884-161">会話をコピーします。</span><span class="sxs-lookup"><span data-stu-id="54884-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="54884-162">SetReadState</span></span>  <br/> |<span data-ttu-id="54884-163">会話の読み取り状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="54884-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="54884-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="54884-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="54884-165">会話のリテンション ・ ポリシーを設定します。</span><span class="sxs-lookup"><span data-stu-id="54884-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54884-166">備考</span><span class="sxs-lookup"><span data-stu-id="54884-166">Remarks</span></span>

<span data-ttu-id="54884-167">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="54884-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54884-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="54884-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54884-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="54884-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54884-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54884-170">Schema Name</span></span>  <br/> |<span data-ttu-id="54884-171">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="54884-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="54884-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54884-172">Validation File</span></span>  <br/> |<span data-ttu-id="54884-173">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="54884-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54884-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="54884-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="54884-175">False</span><span class="sxs-lookup"><span data-stu-id="54884-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54884-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="54884-176">See also</span></span>



[<span data-ttu-id="54884-177">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="54884-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="54884-178">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="54884-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

