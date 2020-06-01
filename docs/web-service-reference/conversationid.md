---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: ConversationId 要素には、アイテムまたは会話の識別子が含まれています。
ms.openlocfilehash: 4f12d70ae6b72773760a731f5778cf6743ce699f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461472"
---
# <a name="conversationid"></a><span data-ttu-id="09f4f-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="09f4f-103">ConversationId</span></span>

<span data-ttu-id="09f4f-104">**ConversationId**要素には、アイテムまたは会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09f4f-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="09f4f-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="09f4f-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09f4f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="09f4f-106">Attributes and elements</span></span>

<span data-ttu-id="09f4f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09f4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="09f4f-108">Attributes</span></span>

|<span data-ttu-id="09f4f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="09f4f-109">**Attribute**</span></span>|<span data-ttu-id="09f4f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="09f4f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="09f4f-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="09f4f-111">**Id**</span></span> <br/> |<span data-ttu-id="09f4f-112">Exchange ストア内の特定のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="09f4f-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="09f4f-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="09f4f-114">特定のバージョンのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="09f4f-115">次のシナリオでは、 **Changekey**が必要です。</span><span class="sxs-lookup"><span data-stu-id="09f4f-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="09f4f-116">- **ConflictResolution**属性が自動解決に設定されている場合、 [updateitem](updateitem.md)要素には**changekey**が必要です。</span><span class="sxs-lookup"><span data-stu-id="09f4f-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="09f4f-117">自動解決は既定値です。</span><span class="sxs-lookup"><span data-stu-id="09f4f-117">AutoResolve is a default value.</span></span> <span data-ttu-id="09f4f-118">**Changekey**属性が含まれていない場合、応答は、 **Errorchangekeyrequired**に[等しい値を](responsecode.md)返します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="09f4f-119">- [SendItem](senditem.md)、 [DeleteItem](deleteitem.md)、および[deletefolder](deletefolder.md)要素は、実行しようとした操作がアイテムの最新バージョンに対して動作するかどうかをテストするために、 **changekey**を必要とします。</span><span class="sxs-lookup"><span data-stu-id="09f4f-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="09f4f-120">**Changekey**属性が**ItemId**に含まれていない場合、または**changekey**が空の場合は、応答は**ErrorStaleObject**に等しい、応答し[た値を](responsecode.md)返します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="09f4f-121">子要素</span><span class="sxs-lookup"><span data-stu-id="09f4f-121">Child elements</span></span>

<span data-ttu-id="09f4f-122">なし。</span><span class="sxs-lookup"><span data-stu-id="09f4f-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09f4f-123">親要素</span><span class="sxs-lookup"><span data-stu-id="09f4f-123">Parent elements</span></span>

|<span data-ttu-id="09f4f-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="09f4f-124">**Element**</span></span>|<span data-ttu-id="09f4f-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="09f4f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09f4f-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="09f4f-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="09f4f-127">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-128">連絡先</span><span class="sxs-lookup"><span data-stu-id="09f4f-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="09f4f-129">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="09f4f-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="09f4f-131">単一の会話に適用される1つのアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="09f4f-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="09f4f-133">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-134">アイテム</span><span class="sxs-lookup"><span data-stu-id="09f4f-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="09f4f-135">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="09f4f-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="09f4f-137">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="09f4f-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="09f4f-139">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-140">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="09f4f-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="09f4f-141">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="09f4f-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="09f4f-143">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-144">Message</span><span class="sxs-lookup"><span data-stu-id="09f4f-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="09f4f-145">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="09f4f-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="09f4f-147">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="09f4f-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="09f4f-149">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-150">Task</span><span class="sxs-lookup"><span data-stu-id="09f4f-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="09f4f-151">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="09f4f-152">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="09f4f-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="09f4f-153">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="09f4f-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09f4f-154">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09f4f-154">Text value</span></span>

<span data-ttu-id="09f4f-155">なし。</span><span class="sxs-lookup"><span data-stu-id="09f4f-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09f4f-156">注釈</span><span class="sxs-lookup"><span data-stu-id="09f4f-156">Remarks</span></span>

<span data-ttu-id="09f4f-157">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="09f4f-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09f4f-158">要素の情報</span><span class="sxs-lookup"><span data-stu-id="09f4f-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09f4f-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="09f4f-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09f4f-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09f4f-160">Schema Name</span></span>  <br/> |<span data-ttu-id="09f4f-161">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="09f4f-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="09f4f-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09f4f-162">Validation File</span></span>  <br/> |<span data-ttu-id="09f4f-163">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="09f4f-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09f4f-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="09f4f-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="09f4f-165">正しくない</span><span class="sxs-lookup"><span data-stu-id="09f4f-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09f4f-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="09f4f-166">See also</span></span>

- [<span data-ttu-id="09f4f-167">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="09f4f-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="09f4f-168">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="09f4f-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

