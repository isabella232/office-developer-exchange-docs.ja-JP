---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: イベントの種類の要素は、サブスクリプションを作成するために使用し、通知で報告されるイベントの種類を識別します。
ms.openlocfilehash: fb54c9e042f105d10e68cb0e9b48feae7ed8bf7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760336"
---
# <a name="eventtype"></a><span data-ttu-id="bd7e9-103">EventType</span><span class="sxs-lookup"><span data-stu-id="bd7e9-103">EventType</span></span>

<span data-ttu-id="bd7e9-104">**イベントの種類**の要素は、サブスクリプションを作成するために使用し、通知で報告されるイベントの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="bd7e9-105">**NotificationEventTypeType**</span><span class="sxs-lookup"><span data-stu-id="bd7e9-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd7e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bd7e9-106">Attributes and elements</span></span>

<span data-ttu-id="bd7e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd7e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd7e9-108">Attributes</span></span>

<span data-ttu-id="bd7e9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd7e9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd7e9-110">Child elements</span></span>

<span data-ttu-id="bd7e9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd7e9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bd7e9-112">Parent elements</span></span>

|<span data-ttu-id="bd7e9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bd7e9-113">**Element**</span></span>|<span data-ttu-id="bd7e9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd7e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd7e9-115">EventTypes</span><span class="sxs-lookup"><span data-stu-id="bd7e9-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="bd7e9-116">サブスクリプションの作成に使用されるイベント通知イベントの種類のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd7e9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bd7e9-117">Text value</span></span>

<span data-ttu-id="bd7e9-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-118">A text value is required.</span></span> <span data-ttu-id="bd7e9-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="bd7e9-120">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-120">CopiedEvent</span></span>
    
- <span data-ttu-id="bd7e9-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-121">CreatedEvent</span></span>
    
- <span data-ttu-id="bd7e9-122">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-122">DeletedEvent</span></span>
    
- <span data-ttu-id="bd7e9-123">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="bd7e9-124">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-124">MovedEvent</span></span>
    
- <span data-ttu-id="bd7e9-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-125">NewMailEvent</span></span>
    
- <span data-ttu-id="bd7e9-126">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="bd7e9-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="bd7e9-127">備考</span><span class="sxs-lookup"><span data-stu-id="bd7e9-127">Remarks</span></span>

<span data-ttu-id="bd7e9-128">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="bd7e9-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd7e9-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="bd7e9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd7e9-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="bd7e9-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd7e9-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd7e9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="bd7e9-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bd7e9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd7e9-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd7e9-133">Validation File</span></span>  <br/> |<span data-ttu-id="bd7e9-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd7e9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd7e9-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd7e9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd7e9-136">False</span><span class="sxs-lookup"><span data-stu-id="bd7e9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd7e9-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd7e9-137">See also</span></span>



[<span data-ttu-id="bd7e9-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="bd7e9-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="bd7e9-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="bd7e9-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="bd7e9-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="bd7e9-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

