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
description: EventType 要素は、サブスクリプションを作成し、通知で報告されるイベントの種類を識別するために使用されます。
ms.openlocfilehash: 58c7ce571434b6fb8ac0b1dc2a3f8cd4fd56ff17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526173"
---
# <a name="eventtype"></a><span data-ttu-id="6591b-103">EventType</span><span class="sxs-lookup"><span data-stu-id="6591b-103">EventType</span></span>

<span data-ttu-id="6591b-104">**EventType**要素は、サブスクリプションを作成し、通知で報告されるイベントの種類を識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="6591b-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="6591b-105">**NotificationEventTypeType**</span><span class="sxs-lookup"><span data-stu-id="6591b-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6591b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6591b-106">Attributes and elements</span></span>

<span data-ttu-id="6591b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6591b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6591b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6591b-108">Attributes</span></span>

<span data-ttu-id="6591b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6591b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6591b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6591b-110">Child elements</span></span>

<span data-ttu-id="6591b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6591b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6591b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6591b-112">Parent elements</span></span>

|<span data-ttu-id="6591b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6591b-113">**Element**</span></span>|<span data-ttu-id="6591b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6591b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6591b-115">EventTypes</span><span class="sxs-lookup"><span data-stu-id="6591b-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="6591b-116">サブスクリプションの作成に使用されるイベント通知イベントの種類のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6591b-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6591b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6591b-117">Text value</span></span>

<span data-ttu-id="6591b-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="6591b-118">A text value is required.</span></span> <span data-ttu-id="6591b-119">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="6591b-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="6591b-120">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="6591b-120">CopiedEvent</span></span>
    
- <span data-ttu-id="6591b-121">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="6591b-121">CreatedEvent</span></span>
    
- <span data-ttu-id="6591b-122">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="6591b-122">DeletedEvent</span></span>
    
- <span data-ttu-id="6591b-123">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="6591b-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="6591b-124">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="6591b-124">MovedEvent</span></span>
    
- <span data-ttu-id="6591b-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="6591b-125">NewMailEvent</span></span>
    
- <span data-ttu-id="6591b-126">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="6591b-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6591b-127">注釈</span><span class="sxs-lookup"><span data-stu-id="6591b-127">Remarks</span></span>

<span data-ttu-id="6591b-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6591b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6591b-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6591b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6591b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6591b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6591b-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6591b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6591b-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6591b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6591b-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6591b-133">Validation File</span></span>  <br/> |<span data-ttu-id="6591b-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6591b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6591b-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6591b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6591b-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="6591b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6591b-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="6591b-137">See also</span></span>



[<span data-ttu-id="6591b-138">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6591b-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="6591b-139">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="6591b-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="6591b-140">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="6591b-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

