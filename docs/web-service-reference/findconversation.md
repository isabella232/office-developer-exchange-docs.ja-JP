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
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462648"
---
# <a name="findconversation"></a><span data-ttu-id="c7601-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="c7601-103">FindConversation</span></span>

<span data-ttu-id="c7601-104">**Findconversation**要素は、メールボックス内の会話を検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="c7601-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="c7601-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="c7601-105">FindConversation</span></span>](findconversation.md)
  
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

 <span data-ttu-id="c7601-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="c7601-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7601-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c7601-107">Attributes and elements</span></span>

<span data-ttu-id="c7601-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7601-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7601-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7601-109">Attributes</span></span>

****

|<span data-ttu-id="c7601-110">**属性**</span><span class="sxs-lookup"><span data-stu-id="c7601-110">**Attribute**</span></span>|<span data-ttu-id="c7601-111">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7601-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c7601-112">走査</span><span class="sxs-lookup"><span data-stu-id="c7601-112">Traversal</span></span>  <br/> |<span data-ttu-id="c7601-113">サブツリーの走査の種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="c7601-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="c7601-114">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="c7601-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="c7601-115">ViewFilter</span><span class="sxs-lookup"><span data-stu-id="c7601-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="c7601-116">種類ビューのフィルターを識別します。</span><span class="sxs-lookup"><span data-stu-id="c7601-116">Identifies the types view filters.</span></span> <span data-ttu-id="c7601-117">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="c7601-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="c7601-118">トラバース属性値</span><span class="sxs-lookup"><span data-stu-id="c7601-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="c7601-119">**値**</span><span class="sxs-lookup"><span data-stu-id="c7601-119">**Value**</span></span>|<span data-ttu-id="c7601-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7601-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c7601-121">浅い</span><span class="sxs-lookup"><span data-stu-id="c7601-121">Shallow</span></span>  <br/> |<span data-ttu-id="c7601-122">浅い走査を示します。</span><span class="sxs-lookup"><span data-stu-id="c7601-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="c7601-123">深い</span><span class="sxs-lookup"><span data-stu-id="c7601-123">Deep</span></span>  <br/> |<span data-ttu-id="c7601-124">Deep トラバースを示します。</span><span class="sxs-lookup"><span data-stu-id="c7601-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="c7601-125">ViewFilter 属性値</span><span class="sxs-lookup"><span data-stu-id="c7601-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="c7601-126">**値**</span><span class="sxs-lookup"><span data-stu-id="c7601-126">**Value**</span></span>|<span data-ttu-id="c7601-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7601-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c7601-128">すべて</span><span class="sxs-lookup"><span data-stu-id="c7601-128">All</span></span>  <br/> |<span data-ttu-id="c7601-129">すべての会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="c7601-130">Flagged</span><span class="sxs-lookup"><span data-stu-id="c7601-130">Flagged</span></span>  <br/> |<span data-ttu-id="c7601-131">フラグ付きの会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="c7601-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="c7601-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="c7601-133">添付ファイル付きの会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="c7601-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="c7601-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="c7601-135">[宛先] または [cc] の会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="c7601-136">Unread</span><span class="sxs-lookup"><span data-stu-id="c7601-136">Unread</span></span>  <br/> |<span data-ttu-id="c7601-137">未読の会話を検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="c7601-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="c7601-138">TaskActive</span></span>  <br/> |<span data-ttu-id="c7601-139">アクティブなタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="c7601-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="c7601-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="c7601-141">期限の過ぎたタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="c7601-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="c7601-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="c7601-143">完了したタスクを検索します。</span><span class="sxs-lookup"><span data-stu-id="c7601-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="c7601-144">低優先メール</span><span class="sxs-lookup"><span data-stu-id="c7601-144">NoClutter</span></span>  <br/> |<span data-ttu-id="c7601-145">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="c7601-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="c7601-146">クラッター機能</span><span class="sxs-lookup"><span data-stu-id="c7601-146">Clutter</span></span>  <br/> |<span data-ttu-id="c7601-147">内部使用のみ。</span><span class="sxs-lookup"><span data-stu-id="c7601-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c7601-148">子要素</span><span class="sxs-lookup"><span data-stu-id="c7601-148">Child elements</span></span>

|<span data-ttu-id="c7601-149">**Element**</span><span class="sxs-lookup"><span data-stu-id="c7601-149">**Element**</span></span>|<span data-ttu-id="c7601-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7601-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7601-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="c7601-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="c7601-152">ページングされた会話情報が返される方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7601-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="c7601-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="c7601-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="c7601-154">検索の終了を識別するために使用される条件、検索の開始インデックス、返される最大エントリ、および**FindItem**または**findconversation**検索の検索方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7601-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="c7601-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="c7601-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="c7601-156">[Findconversation 操作](findconversation-operation.md)要求でのアイテムの並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="c7601-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="c7601-157">**会話: LastDeliveryTime**プロパティは、 **findconversation**操作が使用されるときに並べ替えに対してサポートされている唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="c7601-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="c7601-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="c7601-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="c7601-159">会話を検索するフォルダーを指定します。</span><span class="sxs-lookup"><span data-stu-id="c7601-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="c7601-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="c7601-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="c7601-161">会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにスパンするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c7601-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c7601-162">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="c7601-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="c7601-163">高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7601-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="c7601-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="c7601-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="c7601-165">[Findconversation 操作](findconversation-operation.md)応答で返されるプロパティセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="c7601-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7601-166">親要素</span><span class="sxs-lookup"><span data-stu-id="c7601-166">Parent elements</span></span>

<span data-ttu-id="c7601-167">なし。</span><span class="sxs-lookup"><span data-stu-id="c7601-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7601-168">注釈</span><span class="sxs-lookup"><span data-stu-id="c7601-168">Remarks</span></span>

<span data-ttu-id="c7601-169">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c7601-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7601-170">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c7601-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7601-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7601-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7601-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c7601-172">Schema Name</span></span>  <br/> |<span data-ttu-id="c7601-173">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c7601-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c7601-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c7601-174">Validation File</span></span>  <br/> |<span data-ttu-id="c7601-175">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c7601-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7601-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c7601-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7601-177">正しくない</span><span class="sxs-lookup"><span data-stu-id="c7601-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7601-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7601-178">See also</span></span>



[<span data-ttu-id="c7601-179">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="c7601-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="c7601-180">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c7601-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c7601-181">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="c7601-181">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

