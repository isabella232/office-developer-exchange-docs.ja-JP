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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833509"
---
# <a name="size"></a><span data-ttu-id="0bb53-104">サイズ</span><span class="sxs-lookup"><span data-stu-id="0bb53-104">Size</span></span>

<span data-ttu-id="0bb53-105">**サイズ**の要素は、現在のフォルダー内の会話ですべてのアイテムのバイト単位のサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-105">The **Size** element represents the size in bytes of an item or all the items in a conversation in the current folder.</span></span> <span data-ttu-id="0bb53-106">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0bb53-106">This property is read-only.</span></span> 
  
```XML
<Size/>
```

 <span data-ttu-id="0bb53-107">**int**</span><span class="sxs-lookup"><span data-stu-id="0bb53-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bb53-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0bb53-108">Attributes and elements</span></span>

<span data-ttu-id="0bb53-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bb53-110">属性</span><span class="sxs-lookup"><span data-stu-id="0bb53-110">Attributes</span></span>

<span data-ttu-id="0bb53-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0bb53-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bb53-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0bb53-112">Child elements</span></span>

<span data-ttu-id="0bb53-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0bb53-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bb53-114">親要素</span><span class="sxs-lookup"><span data-stu-id="0bb53-114">Parent elements</span></span>

|<span data-ttu-id="0bb53-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bb53-115">**Element**</span></span>|<span data-ttu-id="0bb53-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bb53-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bb53-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="0bb53-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0bb53-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-119">Contact</span><span class="sxs-lookup"><span data-stu-id="0bb53-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0bb53-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-121">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0bb53-121">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="0bb53-122">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-122">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-123">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0bb53-123">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="0bb53-124">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-124">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-125">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="0bb53-125">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="0bb53-126">Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-126">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-127">アイテム</span><span class="sxs-lookup"><span data-stu-id="0bb53-127">Item</span></span>](item.md) <br/> |<span data-ttu-id="0bb53-128">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-128">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-129">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0bb53-129">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="0bb53-130">Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-130">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-131">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0bb53-131">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0bb53-132">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-132">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-133">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0bb53-133">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0bb53-134">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-134">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0bb53-135">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0bb53-136">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-136">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-137">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0bb53-137">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0bb53-138">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-138">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-139">Message</span><span class="sxs-lookup"><span data-stu-id="0bb53-139">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0bb53-140">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-140">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-141">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0bb53-141">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0bb53-142">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-142">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb53-143">タスク</span><span class="sxs-lookup"><span data-stu-id="0bb53-143">Task</span></span>](task.md) <br/> |<span data-ttu-id="0bb53-144">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb53-144">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bb53-145">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0bb53-145">Text value</span></span>

<span data-ttu-id="0bb53-146">テキスト値は、バイト内の項目のサイズを識別する整数値です。</span><span class="sxs-lookup"><span data-stu-id="0bb53-146">The text value is an integer value that identifies the size of the item in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bb53-147">備考</span><span class="sxs-lookup"><span data-stu-id="0bb53-147">Remarks</span></span>

<span data-ttu-id="0bb53-148">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0bb53-148">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bb53-149">要素情報</span><span class="sxs-lookup"><span data-stu-id="0bb53-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bb53-150">名前空間</span><span class="sxs-lookup"><span data-stu-id="0bb53-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bb53-151">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bb53-151">Schema Name</span></span>  <br/> |<span data-ttu-id="0bb53-152">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0bb53-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bb53-153">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bb53-153">Validation File</span></span>  <br/> |<span data-ttu-id="0bb53-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bb53-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bb53-155">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0bb53-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bb53-156">False</span><span class="sxs-lookup"><span data-stu-id="0bb53-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bb53-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bb53-157">See also</span></span>



- [<span data-ttu-id="0bb53-158">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0bb53-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

