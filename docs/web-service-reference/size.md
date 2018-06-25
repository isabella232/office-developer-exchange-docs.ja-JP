---
title: サイズ
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
description: サイズの要素は、現在のフォルダー内の会話ですべてのアイテムのバイト単位のサイズを表します。 このプロパティは値の取得のみ可能です。
ms.openlocfilehash: 15ee0bce6bc5fa2065cef4ecee40d7a6d65e3249
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833509"
---
# <a name="size"></a><span data-ttu-id="da6f5-104">サイズ</span><span class="sxs-lookup"><span data-stu-id="da6f5-104">Size</span></span>

<span data-ttu-id="da6f5-105">**サイズ**の要素は、現在のフォルダー内の会話ですべてのアイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-105">The **Size** element represents the size in bytes of an item or all the items in a conversation in the current folder.</span></span> <span data-ttu-id="da6f5-106">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="da6f5-106">This property is read-only.</span></span> 
  
```XML
<Size/>
```

 <span data-ttu-id="da6f5-107">**int**</span><span class="sxs-lookup"><span data-stu-id="da6f5-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da6f5-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="da6f5-108">Attributes and elements</span></span>

<span data-ttu-id="da6f5-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da6f5-110">属性</span><span class="sxs-lookup"><span data-stu-id="da6f5-110">Attributes</span></span>

<span data-ttu-id="da6f5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da6f5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da6f5-112">子要素</span><span class="sxs-lookup"><span data-stu-id="da6f5-112">Child elements</span></span>

<span data-ttu-id="da6f5-113">なし。</span><span class="sxs-lookup"><span data-stu-id="da6f5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da6f5-114">親要素</span><span class="sxs-lookup"><span data-stu-id="da6f5-114">Parent elements</span></span>

|<span data-ttu-id="da6f5-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="da6f5-115">**Element**</span></span>|<span data-ttu-id="da6f5-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="da6f5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da6f5-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="da6f5-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="da6f5-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-119">Contact</span><span class="sxs-lookup"><span data-stu-id="da6f5-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="da6f5-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-121">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="da6f5-121">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="da6f5-122">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-122">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="da6f5-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="da6f5-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-125">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="da6f5-125">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="da6f5-126">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-126">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-127">アイテム</span><span class="sxs-lookup"><span data-stu-id="da6f5-127">Item</span></span>](item.md) <br/> |<span data-ttu-id="da6f5-128">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-128">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-129">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="da6f5-129">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="da6f5-130">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-130">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="da6f5-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="da6f5-132">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="da6f5-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="da6f5-134">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-134">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="da6f5-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="da6f5-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="da6f5-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="da6f5-138">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-139">Message</span><span class="sxs-lookup"><span data-stu-id="da6f5-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="da6f5-140">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-140">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-141">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="da6f5-141">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="da6f5-142">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-142">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="da6f5-143">タスク</span><span class="sxs-lookup"><span data-stu-id="da6f5-143">Task</span></span>](task.md) <br/> |<span data-ttu-id="da6f5-144">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="da6f5-144">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da6f5-145">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da6f5-145">Text value</span></span>

<span data-ttu-id="da6f5-146">テキスト値は、バイト内の項目のサイズを識別する整数値です。</span><span class="sxs-lookup"><span data-stu-id="da6f5-146">The text value is an integer value that identifies the size of the item in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da6f5-147">備考</span><span class="sxs-lookup"><span data-stu-id="da6f5-147">Remarks</span></span>

<span data-ttu-id="da6f5-148">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="da6f5-148">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da6f5-149">要素情報</span><span class="sxs-lookup"><span data-stu-id="da6f5-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da6f5-150">名前空間</span><span class="sxs-lookup"><span data-stu-id="da6f5-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da6f5-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da6f5-151">Schema Name</span></span>  <br/> |<span data-ttu-id="da6f5-152">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="da6f5-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="da6f5-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da6f5-153">Validation File</span></span>  <br/> |<span data-ttu-id="da6f5-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da6f5-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da6f5-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="da6f5-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="da6f5-156">False</span><span class="sxs-lookup"><span data-stu-id="da6f5-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da6f5-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="da6f5-157">See also</span></span>



- [<span data-ttu-id="da6f5-158">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="da6f5-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

