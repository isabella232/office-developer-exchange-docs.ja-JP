---
title: NewMailEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewMailEvent
api_type:
- schema
ms.assetid: 45057945-a3ec-4dac-92db-f0dc5fcfc34d
description: NewMailEvent 要素は、メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。
ms.openlocfilehash: aa562b60a7299543af8653bbc767edf329075644
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466816"
---
# <a name="newmailevent"></a><span data-ttu-id="d3844-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d3844-103">NewMailEvent</span></span>

<span data-ttu-id="d3844-104">**Newmailevent**要素は、メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="d3844-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="d3844-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="d3844-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3844-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d3844-106">Attributes and elements</span></span>

<span data-ttu-id="d3844-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3844-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3844-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3844-108">Attributes</span></span>

<span data-ttu-id="d3844-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d3844-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3844-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d3844-110">Child elements</span></span>

|<span data-ttu-id="d3844-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d3844-111">**Element**</span></span>|<span data-ttu-id="d3844-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3844-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3844-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="d3844-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d3844-114">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="d3844-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="d3844-115">示</span><span class="sxs-lookup"><span data-stu-id="d3844-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="d3844-116">メールボックスに新しいメールアイテムが到着したときのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="d3844-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3844-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="d3844-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d3844-118">新しいメールアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d3844-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="d3844-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d3844-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d3844-120">新しいメールアイテムの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d3844-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3844-121">親要素</span><span class="sxs-lookup"><span data-stu-id="d3844-121">Parent elements</span></span>

|<span data-ttu-id="d3844-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3844-122">**Element**</span></span>|<span data-ttu-id="d3844-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3844-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3844-124">通知</span><span class="sxs-lookup"><span data-stu-id="d3844-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d3844-125">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d3844-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3844-126">注釈</span><span class="sxs-lookup"><span data-stu-id="d3844-126">Remarks</span></span>

<span data-ttu-id="d3844-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d3844-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3844-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d3844-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3844-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3844-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3844-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3844-130">Schema name</span></span>  <br/> |<span data-ttu-id="d3844-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d3844-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3844-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3844-132">Validation file</span></span>  <br/> |<span data-ttu-id="d3844-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d3844-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3844-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d3844-134">Can be empty</span></span>  <br/> |<span data-ttu-id="d3844-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="d3844-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3844-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3844-136">See also</span></span>



[<span data-ttu-id="d3844-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d3844-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d3844-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d3844-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d3844-139">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d3844-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

