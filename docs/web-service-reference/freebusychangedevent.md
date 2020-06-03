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
description: FreeBusyChangedEvent 要素は、アイテムの空き時間情報が変更されたイベントを表します。
ms.openlocfilehash: d9ea8bc210ab503c4e9f606bcb66317cefe15de1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456480"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="07848-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="07848-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="07848-104">**FreeBusyChangedEvent**要素は、アイテムの空き時間情報が変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="07848-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="07848-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="07848-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07848-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="07848-106">Attributes and elements</span></span>

<span data-ttu-id="07848-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07848-108">属性</span><span class="sxs-lookup"><span data-stu-id="07848-108">Attributes</span></span>

<span data-ttu-id="07848-109">なし。</span><span class="sxs-lookup"><span data-stu-id="07848-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07848-110">子要素</span><span class="sxs-lookup"><span data-stu-id="07848-110">Child elements</span></span>

|<span data-ttu-id="07848-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="07848-111">**Element**</span></span>|<span data-ttu-id="07848-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="07848-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07848-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="07848-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="07848-114">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="07848-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="07848-115">示</span><span class="sxs-lookup"><span data-stu-id="07848-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="07848-116">空き時間アイテムメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="07848-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="07848-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="07848-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="07848-118">空き時間情報アイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="07848-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="07848-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="07848-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="07848-120">空き時間情報アイテムの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="07848-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07848-121">親要素</span><span class="sxs-lookup"><span data-stu-id="07848-121">Parent elements</span></span>

|<span data-ttu-id="07848-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="07848-122">**Element**</span></span>|<span data-ttu-id="07848-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="07848-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07848-124">通知</span><span class="sxs-lookup"><span data-stu-id="07848-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="07848-125">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="07848-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07848-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="07848-126">Text value</span></span>

<span data-ttu-id="07848-127">なし。</span><span class="sxs-lookup"><span data-stu-id="07848-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="07848-128">注釈</span><span class="sxs-lookup"><span data-stu-id="07848-128">Remarks</span></span>

<span data-ttu-id="07848-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="07848-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07848-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="07848-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07848-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="07848-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07848-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="07848-132">Schema name</span></span>  <br/> |<span data-ttu-id="07848-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="07848-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="07848-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="07848-134">Validation file</span></span>  <br/> |<span data-ttu-id="07848-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="07848-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07848-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="07848-136">Can be empty</span></span>  <br/> |<span data-ttu-id="07848-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="07848-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07848-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="07848-138">See also</span></span>



[<span data-ttu-id="07848-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="07848-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="07848-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="07848-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="07848-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="07848-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="07848-142">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="07848-142">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="07848-143">EWS でのイベント通知</span><span class="sxs-lookup"><span data-stu-id="07848-143">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

