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
description: DeliveryStatus 要素は、メッセージの状態を指定します。
ms.openlocfilehash: ae32202284d3dd272f693fbb7b76070cb6019d28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461402"
---
# <a name="deliverystatus"></a><span data-ttu-id="26d81-103">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="26d81-103">DeliveryStatus</span></span>

<span data-ttu-id="26d81-104">**Deliverystatus**要素は、メッセージの状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="26d81-104">The **DeliveryStatus** element specifies the status for a message.</span></span> 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 <span data-ttu-id="26d81-105">**MessageTrackingDeliveryStatusType**</span><span class="sxs-lookup"><span data-stu-id="26d81-105">**MessageTrackingDeliveryStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26d81-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="26d81-106">Attributes and elements</span></span>

<span data-ttu-id="26d81-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="26d81-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26d81-108">属性</span><span class="sxs-lookup"><span data-stu-id="26d81-108">Attributes</span></span>

<span data-ttu-id="26d81-109">なし。</span><span class="sxs-lookup"><span data-stu-id="26d81-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26d81-110">子要素</span><span class="sxs-lookup"><span data-stu-id="26d81-110">Child elements</span></span>

<span data-ttu-id="26d81-111">なし。</span><span class="sxs-lookup"><span data-stu-id="26d81-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26d81-112">親要素</span><span class="sxs-lookup"><span data-stu-id="26d81-112">Parent elements</span></span>

|<span data-ttu-id="26d81-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="26d81-113">**Element**</span></span>|<span data-ttu-id="26d81-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="26d81-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26d81-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="26d81-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="26d81-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="26d81-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26d81-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="26d81-117">Text value</span></span>

<span data-ttu-id="26d81-118">**Deliverystatus**要素の使用可能なテキスト値を次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="26d81-118">The following table lists the possible text values for the **DeliveryStatus** element.</span></span> 
  
<span data-ttu-id="26d81-119">**DeliveryStatus 要素の値**</span><span class="sxs-lookup"><span data-stu-id="26d81-119">**DeliveryStatus element values**</span></span>

|<span data-ttu-id="26d81-120">**値**</span><span class="sxs-lookup"><span data-stu-id="26d81-120">**Value**</span></span>|<span data-ttu-id="26d81-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="26d81-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="26d81-122">いか</span><span class="sxs-lookup"><span data-stu-id="26d81-122">Unsuccessful</span></span>  <br/> |<span data-ttu-id="26d81-123">メッセージが配信されなかったことを指定します。</span><span class="sxs-lookup"><span data-stu-id="26d81-123">Specifies that a message was not delivered.</span></span>  <br/> |
|<span data-ttu-id="26d81-124">Pending</span><span class="sxs-lookup"><span data-stu-id="26d81-124">Pending</span></span>  <br/> |<span data-ttu-id="26d81-125">メッセージがモデレーターからの承認を待機していることを指定します。</span><span class="sxs-lookup"><span data-stu-id="26d81-125">Specifies that the message is waiting for approval from a moderator.</span></span>  <br/> |
|<span data-ttu-id="26d81-126">届け</span><span class="sxs-lookup"><span data-stu-id="26d81-126">Delivered</span></span>  <br/> |<span data-ttu-id="26d81-127">メッセージが指定されたすべての受信者に配信されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="26d81-127">Specifies that the message was delivered to all of the specified recipients.</span></span>  <br/> |
|<span data-ttu-id="26d81-128">付与</span><span class="sxs-lookup"><span data-stu-id="26d81-128">Transferred</span></span>  <br/> |<span data-ttu-id="26d81-129">メッセージが検索範囲外のサーバーに転送されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="26d81-129">Specifies that the message was transferred to a server outside the search scope.</span></span>  <br/> |
|<span data-ttu-id="26d81-130">Read</span><span class="sxs-lookup"><span data-stu-id="26d81-130">Read</span></span>  <br/> |<span data-ttu-id="26d81-131">受信者によってメッセージが配信および開封されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="26d81-131">Specifies that the message was delivered and read by the recipients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26d81-132">注釈</span><span class="sxs-lookup"><span data-stu-id="26d81-132">Remarks</span></span>

<span data-ttu-id="26d81-133">**Deliverystatus**要素の種類は、Exchange Server 2010 の**Messagetrackingdeliverystatustype**た。</span><span class="sxs-lookup"><span data-stu-id="26d81-133">The **DeliveryStatus** element was of type **MessageTrackingDeliveryStatusType** in Exchange Server 2010.</span></span> 
  
<span data-ttu-id="26d81-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="26d81-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26d81-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="26d81-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26d81-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="26d81-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26d81-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="26d81-137">Schema Name</span></span>  <br/> |<span data-ttu-id="26d81-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="26d81-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="26d81-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="26d81-139">Validation File</span></span>  <br/> |<span data-ttu-id="26d81-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="26d81-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26d81-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="26d81-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="26d81-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="26d81-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26d81-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="26d81-143">See also</span></span>

- [<span data-ttu-id="26d81-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="26d81-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

