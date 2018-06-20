---
title: FreeBusyChangedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyChangedEvent
api_type:
- schema
ms.assetid: 63abbfc5-c29f-4110-a922-6b1247187f28
description: FreeBusyChangedEvent 要素は、アイテムの空き時間情報の変更に使用されたイベントを表します。
ms.openlocfilehash: 7271d375526e7614d0150594c2b988666a59eb8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760601"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="112ee-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="112ee-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="112ee-104">**FreeBusyChangedEvent**要素は、アイテムの空き時間情報の変更に使用されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="112ee-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="112ee-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="112ee-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="112ee-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="112ee-106">Attributes and elements</span></span>

<span data-ttu-id="112ee-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="112ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="112ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="112ee-108">Attributes</span></span>

<span data-ttu-id="112ee-109">なし。</span><span class="sxs-lookup"><span data-stu-id="112ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="112ee-110">子要素</span><span class="sxs-lookup"><span data-stu-id="112ee-110">Child elements</span></span>

|<span data-ttu-id="112ee-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="112ee-111">**Element**</span></span>|<span data-ttu-id="112ee-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="112ee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="112ee-113">透かし</span><span class="sxs-lookup"><span data-stu-id="112ee-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="112ee-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="112ee-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="112ee-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="112ee-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="112ee-116">アイテムの空き/予約済みメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="112ee-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="112ee-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="112ee-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="112ee-118">空き/予約済みの項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="112ee-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="112ee-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="112ee-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="112ee-120">空き時間アイテムの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="112ee-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="112ee-121">親要素</span><span class="sxs-lookup"><span data-stu-id="112ee-121">Parent elements</span></span>

|<span data-ttu-id="112ee-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="112ee-122">**Element**</span></span>|<span data-ttu-id="112ee-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="112ee-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="112ee-124">通知</span><span class="sxs-lookup"><span data-stu-id="112ee-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="112ee-125">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="112ee-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="112ee-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="112ee-126">Text value</span></span>

<span data-ttu-id="112ee-127">なし。</span><span class="sxs-lookup"><span data-stu-id="112ee-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="112ee-128">備考</span><span class="sxs-lookup"><span data-stu-id="112ee-128">Remarks</span></span>

<span data-ttu-id="112ee-129">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="112ee-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="112ee-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="112ee-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="112ee-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="112ee-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="112ee-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="112ee-132">Schema name</span></span>  <br/> |<span data-ttu-id="112ee-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="112ee-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="112ee-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="112ee-134">Validation file</span></span>  <br/> |<span data-ttu-id="112ee-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="112ee-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="112ee-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="112ee-136">Can be empty</span></span>  <br/> |<span data-ttu-id="112ee-137">False</span><span class="sxs-lookup"><span data-stu-id="112ee-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="112ee-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="112ee-138">See also</span></span>



[<span data-ttu-id="112ee-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="112ee-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="112ee-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="112ee-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="112ee-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="112ee-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="112ee-142">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="112ee-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="112ee-143">EWS でのイベントの通知</span><span class="sxs-lookup"><span data-stu-id="112ee-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

