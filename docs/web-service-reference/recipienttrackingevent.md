---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: RecipientTrackingEvent 要素には、受信者の 1 つのイベントの情報が含まれています。
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832989"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="85520-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="85520-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="85520-104">**RecipientTrackingEvent**要素には、受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="85520-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 <span data-ttu-id="85520-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="85520-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85520-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="85520-106">Attributes and elements</span></span>

<span data-ttu-id="85520-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="85520-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85520-108">属性</span><span class="sxs-lookup"><span data-stu-id="85520-108">Attributes</span></span>

<span data-ttu-id="85520-109">なし。</span><span class="sxs-lookup"><span data-stu-id="85520-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85520-110">子要素</span><span class="sxs-lookup"><span data-stu-id="85520-110">Child elements</span></span>

|<span data-ttu-id="85520-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="85520-111">**Element**</span></span>|<span data-ttu-id="85520-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="85520-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85520-113">日付 (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="85520-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="85520-114">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-115">Recipient</span><span class="sxs-lookup"><span data-stu-id="85520-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="85520-116">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="85520-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="85520-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-119">EventDescription</span><span class="sxs-lookup"><span data-stu-id="85520-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="85520-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-121">EventData</span><span class="sxs-lookup"><span data-stu-id="85520-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="85520-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85520-123">サーバー (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="85520-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="85520-124">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-125">Internalid など</span><span class="sxs-lookup"><span data-stu-id="85520-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="85520-126">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="85520-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="85520-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="85520-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="85520-128">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85520-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="85520-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="85520-130">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85520-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="85520-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="85520-132">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85520-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="85520-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="85520-134">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="85520-135">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="85520-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="85520-136">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="85520-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85520-137">親要素</span><span class="sxs-lookup"><span data-stu-id="85520-137">Parent elements</span></span>

|<span data-ttu-id="85520-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="85520-138">**Element**</span></span>|<span data-ttu-id="85520-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="85520-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85520-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="85520-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="85520-141">受信者の 1 つまたは複数の追跡イベントのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="85520-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85520-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="85520-142">Text value</span></span>

<span data-ttu-id="85520-143">なし。</span><span class="sxs-lookup"><span data-stu-id="85520-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85520-144">備考</span><span class="sxs-lookup"><span data-stu-id="85520-144">Remarks</span></span>

<span data-ttu-id="85520-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="85520-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85520-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="85520-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85520-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="85520-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85520-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="85520-148">Schema Name</span></span>  <br/> |<span data-ttu-id="85520-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="85520-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="85520-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="85520-150">Validation File</span></span>  <br/> |<span data-ttu-id="85520-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85520-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85520-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="85520-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="85520-153">False</span><span class="sxs-lookup"><span data-stu-id="85520-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85520-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="85520-154">See also</span></span>



[<span data-ttu-id="85520-155">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="85520-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="85520-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="85520-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

