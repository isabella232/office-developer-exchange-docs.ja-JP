---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: DeliveryStatus 要素は、メッセージのステータスを指定します。
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760006"
---
# <a name="deliverystatus"></a><span data-ttu-id="b77ea-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="b77ea-103">DeliveryStatus</span></span>

<span data-ttu-id="b77ea-104">**DeliveryStatus**要素は、メッセージのステータスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="b77ea-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="b77ea-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b77ea-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b77ea-106">Attributes and elements</span></span>

<span data-ttu-id="b77ea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b77ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="b77ea-108">Attributes</span></span>

<span data-ttu-id="b77ea-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b77ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b77ea-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b77ea-110">Child elements</span></span>

<span data-ttu-id="b77ea-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b77ea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b77ea-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b77ea-112">Parent elements</span></span>

|<span data-ttu-id="b77ea-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b77ea-113">**Element**</span></span>|<span data-ttu-id="b77ea-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b77ea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b77ea-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="b77ea-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="b77ea-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b77ea-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b77ea-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b77ea-117">Text value</span></span>

<span data-ttu-id="b77ea-118">**DeliveryStatus**要素の可能なテキスト値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="b77ea-119">**DeliveryStatus 要素の値**</span><span class="sxs-lookup"><span data-stu-id="b77ea-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="b77ea-120">**値**</span><span class="sxs-lookup"><span data-stu-id="b77ea-120">**Value**</span></span>|<span data-ttu-id="b77ea-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="b77ea-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b77ea-122">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="b77ea-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="b77ea-123">メッセージが配信されなかったことを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="b77ea-124">Pending</span><span class="sxs-lookup"><span data-stu-id="b77ea-124">Pending</span></span>  <br/> |<span data-ttu-id="b77ea-125">メッセージがモデレーターの承認を待機しているかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="b77ea-126">配信</span><span class="sxs-lookup"><span data-stu-id="b77ea-126">Delivered</span></span>  <br/> |<span data-ttu-id="b77ea-127">すべての指定された受信者にメッセージが配信されたことを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="b77ea-128">転送</span><span class="sxs-lookup"><span data-stu-id="b77ea-128">Transferred</span></span>  <br/> |<span data-ttu-id="b77ea-129">検索範囲外のサーバにメッセージが転送されたことを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="b77ea-130">読み取り</span><span class="sxs-lookup"><span data-stu-id="b77ea-130">Read</span></span>  <br/> |<span data-ttu-id="b77ea-131">メッセージが配信され、受信者が読み取ることを指定します。</span><span class="sxs-lookup"><span data-stu-id="b77ea-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b77ea-132">備考</span><span class="sxs-lookup"><span data-stu-id="b77ea-132">Remarks</span></span>

<span data-ttu-id="b77ea-133">**DeliveryStatus**要素は、[Exchange Server 2010 の型**MessageTrackingDeliveryStatusType**のでした。</span><span class="sxs-lookup"><span data-stu-id="b77ea-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="b77ea-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b77ea-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b77ea-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="b77ea-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b77ea-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="b77ea-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b77ea-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b77ea-137">Schema Name</span></span>  <br/> |<span data-ttu-id="b77ea-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b77ea-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="b77ea-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b77ea-139">Validation File</span></span>  <br/> |<span data-ttu-id="b77ea-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b77ea-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b77ea-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b77ea-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="b77ea-142">False</span><span class="sxs-lookup"><span data-stu-id="b77ea-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b77ea-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="b77ea-143">See also</span></span>

- [<span data-ttu-id="b77ea-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b77ea-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

