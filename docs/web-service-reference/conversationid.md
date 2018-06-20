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
description: ConversationId 要素には、アイテムや会話の識別子が含まれています。
ms.openlocfilehash: 1f82e6ade60fb70db4a9f026fd72d9f11cc63821
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759756"
---
# <a name="conversationid"></a><span data-ttu-id="4ab42-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="4ab42-103">ConversationId</span></span>

<span data-ttu-id="4ab42-104">**ConversationId**要素には、アイテムや会話の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4ab42-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="4ab42-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="4ab42-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ab42-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4ab42-106">Attributes and elements</span></span>

<span data-ttu-id="4ab42-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ab42-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ab42-108">Attributes</span></span>

|<span data-ttu-id="4ab42-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4ab42-109">**Attribute**</span></span>|<span data-ttu-id="4ab42-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ab42-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ab42-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="4ab42-111">**Id**</span></span> <br/> |<span data-ttu-id="4ab42-112">Exchange ストア内の特定の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="4ab42-113">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="4ab42-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="4ab42-114">アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="4ab42-115">の**変更キー**は、次のシナリオで必要です。</span><span class="sxs-lookup"><span data-stu-id="4ab42-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="4ab42-116">- [UpdateItem](updateitem.md)要素では、自動解決する**ConflictResolution**属性が設定されている場合に、**変更キー**が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ab42-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="4ab42-117">自動解決は、既定値です。</span><span class="sxs-lookup"><span data-stu-id="4ab42-117">AutoResolve is a default value.</span></span> <span data-ttu-id="4ab42-118">**変更キー**属性が含まれていない場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorChangeKeyRequired**に等しい。</span><span class="sxs-lookup"><span data-stu-id="4ab42-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="4ab42-119">- [SendItem](senditem.md)、 [DeleteItem](deleteitem.md)、および[DeleteFolder](deletefolder.md)の要素は、試行した操作は、項目の最新バージョンに対して機能するかどうかをテストするための**変更キー**を必要とします。</span><span class="sxs-lookup"><span data-stu-id="4ab42-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="4ab42-120">**アイテム Id**の**変更キー**の属性が含まれていない場合、または**変更キー**が空の場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorStaleObject**に等しい。</span><span class="sxs-lookup"><span data-stu-id="4ab42-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4ab42-121">子要素</span><span class="sxs-lookup"><span data-stu-id="4ab42-121">Child elements</span></span>

<span data-ttu-id="4ab42-122">なし。</span><span class="sxs-lookup"><span data-stu-id="4ab42-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ab42-123">親要素</span><span class="sxs-lookup"><span data-stu-id="4ab42-123">Parent elements</span></span>

|<span data-ttu-id="4ab42-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ab42-124">**Element**</span></span>|<span data-ttu-id="4ab42-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ab42-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ab42-126">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="4ab42-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4ab42-127">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-128">Contact</span><span class="sxs-lookup"><span data-stu-id="4ab42-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4ab42-129">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="4ab42-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="4ab42-131">1 つのテーマを適用する 1 つのアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="4ab42-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="4ab42-133">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-134">アイテム</span><span class="sxs-lookup"><span data-stu-id="4ab42-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="4ab42-135">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="4ab42-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4ab42-137">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="4ab42-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="4ab42-139">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-140">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4ab42-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4ab42-141">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4ab42-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4ab42-143">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-144">Message</span><span class="sxs-lookup"><span data-stu-id="4ab42-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4ab42-145">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="4ab42-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="4ab42-147">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="4ab42-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="4ab42-149">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-150">タスク</span><span class="sxs-lookup"><span data-stu-id="4ab42-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="4ab42-151">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4ab42-152">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4ab42-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="4ab42-153">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="4ab42-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ab42-154">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ab42-154">Text value</span></span>

<span data-ttu-id="4ab42-155">なし。</span><span class="sxs-lookup"><span data-stu-id="4ab42-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ab42-156">備考</span><span class="sxs-lookup"><span data-stu-id="4ab42-156">Remarks</span></span>

<span data-ttu-id="4ab42-157">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4ab42-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ab42-158">要素情報</span><span class="sxs-lookup"><span data-stu-id="4ab42-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ab42-159">名前空間</span><span class="sxs-lookup"><span data-stu-id="4ab42-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ab42-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ab42-160">Schema Name</span></span>  <br/> |<span data-ttu-id="4ab42-161">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ab42-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ab42-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ab42-162">Validation File</span></span>  <br/> |<span data-ttu-id="4ab42-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ab42-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ab42-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ab42-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ab42-165">False</span><span class="sxs-lookup"><span data-stu-id="4ab42-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ab42-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ab42-166">See also</span></span>

- <span data-ttu-id="4ab42-167">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4ab42-167">[FindConversation operation](findconversation-operation.md)</span></span>
- [<span data-ttu-id="4ab42-168">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ab42-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

