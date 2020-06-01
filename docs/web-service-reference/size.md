---
title: Size
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Size
api_type:
- schema
ms.assetid: 966f4daf-c20e-49f8-aeb6-965f3e2da7c3
description: Size 要素は、現在のフォルダー内の1つのアイテムまたはスレッド内のすべてのアイテムのサイズ (バイト単位) を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: 406271c80db6bbb797592dae22e50ebe7c42ee85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467292"
---
# <a name="size"></a><span data-ttu-id="e35cd-104">Size</span><span class="sxs-lookup"><span data-stu-id="e35cd-104">Size</span></span>

<span data-ttu-id="e35cd-105">**Size**要素は、現在のフォルダー内の1つのアイテムまたはスレッド内のすべてのアイテムのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-105">The **Size** element represents the size in bytes of an item or all the items in a conversation in the current folder.</span></span> <span data-ttu-id="e35cd-106">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-106">This property is read-only.</span></span> 
  
```XML
<Size/>
```

 <span data-ttu-id="e35cd-107">**int**</span><span class="sxs-lookup"><span data-stu-id="e35cd-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e35cd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e35cd-108">Attributes and elements</span></span>

<span data-ttu-id="e35cd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e35cd-110">属性</span><span class="sxs-lookup"><span data-stu-id="e35cd-110">Attributes</span></span>

<span data-ttu-id="e35cd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e35cd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e35cd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="e35cd-112">Child elements</span></span>

<span data-ttu-id="e35cd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e35cd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e35cd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="e35cd-114">Parent elements</span></span>

|<span data-ttu-id="e35cd-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="e35cd-115">**Element**</span></span>|<span data-ttu-id="e35cd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="e35cd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e35cd-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="e35cd-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e35cd-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-119">連絡先</span><span class="sxs-lookup"><span data-stu-id="e35cd-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e35cd-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-121">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e35cd-121">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e35cd-122">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-122">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e35cd-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e35cd-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-125">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="e35cd-125">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="e35cd-126">Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-126">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-127">アイテム</span><span class="sxs-lookup"><span data-stu-id="e35cd-127">Item</span></span>](item.md) <br/> |<span data-ttu-id="e35cd-128">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-128">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-129">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="e35cd-129">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="e35cd-130">別の Exchange アイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-130">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e35cd-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e35cd-132">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e35cd-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e35cd-134">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-134">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e35cd-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e35cd-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e35cd-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e35cd-138">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-139">Message</span><span class="sxs-lookup"><span data-stu-id="e35cd-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e35cd-140">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-140">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-141">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e35cd-141">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e35cd-142">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-142">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e35cd-143">Task</span><span class="sxs-lookup"><span data-stu-id="e35cd-143">Task</span></span>](task.md) <br/> |<span data-ttu-id="e35cd-144">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="e35cd-144">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e35cd-145">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e35cd-145">Text value</span></span>

<span data-ttu-id="e35cd-146">Text 値は、アイテムのサイズをバイト単位で示す整数値です。</span><span class="sxs-lookup"><span data-stu-id="e35cd-146">The text value is an integer value that identifies the size of the item in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e35cd-147">注釈</span><span class="sxs-lookup"><span data-stu-id="e35cd-147">Remarks</span></span>

<span data-ttu-id="e35cd-148">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e35cd-148">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e35cd-149">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e35cd-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e35cd-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="e35cd-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e35cd-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e35cd-151">Schema Name</span></span>  <br/> |<span data-ttu-id="e35cd-152">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e35cd-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="e35cd-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e35cd-153">Validation File</span></span>  <br/> |<span data-ttu-id="e35cd-154">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e35cd-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e35cd-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e35cd-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="e35cd-156">正しくない</span><span class="sxs-lookup"><span data-stu-id="e35cd-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e35cd-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="e35cd-157">See also</span></span>



- [<span data-ttu-id="e35cd-158">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e35cd-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

