---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: FindConversation 要素は、メールボックス内の会話を検索するための要求を定義します。
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760497"
---
# <a name="findconversation"></a><span data-ttu-id="70151-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="70151-103">FindConversation</span></span>

<span data-ttu-id="70151-104">**FindConversation**要素は、メールボックス内の会話を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="70151-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="70151-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="70151-105">FindConversation</span></span>](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 <span data-ttu-id="70151-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="70151-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70151-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="70151-107">Attributes and elements</span></span>

<span data-ttu-id="70151-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70151-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70151-109">属性</span><span class="sxs-lookup"><span data-stu-id="70151-109">Attributes</span></span>

****

|<span data-ttu-id="70151-110">**属性**</span><span class="sxs-lookup"><span data-stu-id="70151-110">**Attribute**</span></span>|<span data-ttu-id="70151-111">**説明**</span><span class="sxs-lookup"><span data-stu-id="70151-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70151-112">トラバーサル</span><span class="sxs-lookup"><span data-stu-id="70151-112">Traversal</span></span>  <br/> |<span data-ttu-id="70151-113">サブツリーの走査の種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="70151-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="70151-114">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="70151-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="70151-115">ビューワ</span><span class="sxs-lookup"><span data-stu-id="70151-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="70151-116">型ビューのフィルターを識別します。</span><span class="sxs-lookup"><span data-stu-id="70151-116">Identifies the types view filters.</span></span> <span data-ttu-id="70151-117">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="70151-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="70151-118">検査の属性値</span><span class="sxs-lookup"><span data-stu-id="70151-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="70151-119">**値**</span><span class="sxs-lookup"><span data-stu-id="70151-119">**Value**</span></span>|<span data-ttu-id="70151-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="70151-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70151-121">浅い</span><span class="sxs-lookup"><span data-stu-id="70151-121">Shallow</span></span>  <br/> |<span data-ttu-id="70151-122">Shallow トラバースを示します。</span><span class="sxs-lookup"><span data-stu-id="70151-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="70151-123">深い</span><span class="sxs-lookup"><span data-stu-id="70151-123">Deep</span></span>  <br/> |<span data-ttu-id="70151-124">Deep traversal 検索を示します。</span><span class="sxs-lookup"><span data-stu-id="70151-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="70151-125">ビューワの属性値</span><span class="sxs-lookup"><span data-stu-id="70151-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="70151-126">**値**</span><span class="sxs-lookup"><span data-stu-id="70151-126">**Value**</span></span>|<span data-ttu-id="70151-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="70151-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70151-128">All</span><span class="sxs-lookup"><span data-stu-id="70151-128">All</span></span>  <br/> |<span data-ttu-id="70151-129">すべての会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="70151-130">Flagged</span><span class="sxs-lookup"><span data-stu-id="70151-130">Flagged</span></span>  <br/> |<span data-ttu-id="70151-131">フラグが設定された会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="70151-132">添付ファイルあり</span><span class="sxs-lookup"><span data-stu-id="70151-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="70151-133">添付ファイルとの会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="70151-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="70151-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="70151-135">会話の宛先または cc のように自分の名前を検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="70151-136">Unread</span><span class="sxs-lookup"><span data-stu-id="70151-136">Unread</span></span>  <br/> |<span data-ttu-id="70151-137">未読の会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="70151-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="70151-138">TaskActive</span></span>  <br/> |<span data-ttu-id="70151-139">アクティブなタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="70151-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="70151-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="70151-141">期限過ぎのタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="70151-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="70151-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="70151-143">完了したタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="70151-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="70151-144">NoClutter</span><span class="sxs-lookup"><span data-stu-id="70151-144">NoClutter</span></span>  <br/> |<span data-ttu-id="70151-145">内部使用のために用意されています。</span><span class="sxs-lookup"><span data-stu-id="70151-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="70151-146">散乱</span><span class="sxs-lookup"><span data-stu-id="70151-146">Clutter</span></span>  <br/> |<span data-ttu-id="70151-147">内部使用のために用意されています。</span><span class="sxs-lookup"><span data-stu-id="70151-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70151-148">子要素</span><span class="sxs-lookup"><span data-stu-id="70151-148">Child elements</span></span>

|<span data-ttu-id="70151-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="70151-149">**Element**</span></span>|<span data-ttu-id="70151-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="70151-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70151-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="70151-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="70151-152">ページがどのように会話を説明する情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="70151-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="70151-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="70151-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="70151-154">検索の終了、検索、戻るには、最大のエントリと**FindItem**または**FindConversation**の検索に検索方向の開始インデックスを識別するために使用される条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="70151-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="70151-155">並べ替え順序</span><span class="sxs-lookup"><span data-stu-id="70151-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="70151-156">[FindConversation 操作](findconversation-operation.md)の要求の項目の並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="70151-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="70151-157">**会話: LastDeliveryTime**プロパティは、 **FindConversation**操作を使用する場合の並べ替えはサポートされている唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="70151-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="70151-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="70151-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="70151-159">会話を検索するフォルダーを識別します。</span><span class="sxs-lookup"><span data-stu-id="70151-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="70151-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="70151-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="70151-161">かどうか、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスのアーカイブを指定します。</span><span class="sxs-lookup"><span data-stu-id="70151-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="70151-162">クエリ文字列 (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="70151-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="70151-163">ベースの高度なクエリ構文 (AQS) のメールボックスのクエリ文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="70151-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="70151-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="70151-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="70151-165">[FindConversation 操作](findconversation-operation.md)の応答を返すにプロパティ セットを識別します。</span><span class="sxs-lookup"><span data-stu-id="70151-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70151-166">親要素</span><span class="sxs-lookup"><span data-stu-id="70151-166">Parent elements</span></span>

<span data-ttu-id="70151-167">なし。</span><span class="sxs-lookup"><span data-stu-id="70151-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70151-168">備考</span><span class="sxs-lookup"><span data-stu-id="70151-168">Remarks</span></span>

<span data-ttu-id="70151-169">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="70151-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70151-170">要素情報</span><span class="sxs-lookup"><span data-stu-id="70151-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70151-171">名前空間</span><span class="sxs-lookup"><span data-stu-id="70151-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70151-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70151-172">Schema Name</span></span>  <br/> |<span data-ttu-id="70151-173">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="70151-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70151-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70151-174">Validation File</span></span>  <br/> |<span data-ttu-id="70151-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70151-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70151-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70151-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="70151-177">False</span><span class="sxs-lookup"><span data-stu-id="70151-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70151-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="70151-178">See also</span></span>



<span data-ttu-id="70151-179">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="70151-179">[FindConversation operation](findconversation-operation.md)</span></span>


- [<span data-ttu-id="70151-180">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="70151-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="70151-181">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="70151-181">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

