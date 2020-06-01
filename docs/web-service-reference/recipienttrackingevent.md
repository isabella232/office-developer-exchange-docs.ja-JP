---
title: 受信者 Trackingイベント
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
description: 受信者 Trackingevent 要素には、受信者に対する1つのイベントに関する情報が含まれています。
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465486"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="1f47b-103">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="1f47b-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="1f47b-104">受信者**trackingevent**要素には、受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f47b-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
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

 <span data-ttu-id="1f47b-105">**受信者 Trackingeventtype**</span><span class="sxs-lookup"><span data-stu-id="1f47b-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f47b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f47b-106">Attributes and elements</span></span>

<span data-ttu-id="1f47b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f47b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f47b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f47b-108">Attributes</span></span>

<span data-ttu-id="1f47b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1f47b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f47b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1f47b-110">Child elements</span></span>

|<span data-ttu-id="1f47b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1f47b-111">**Element**</span></span>|<span data-ttu-id="1f47b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f47b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f47b-113">日付 (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="1f47b-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="1f47b-114">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-114">This element is required.</span></span>  <br/> |
|<span data-ttu-id="1f47b-115">[[受信者]](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1f47b-115">[Recipient](recipient.md)</span></span> <br/> |<span data-ttu-id="1f47b-116">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="1f47b-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="1f47b-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-119">イベントの説明</span><span class="sxs-lookup"><span data-stu-id="1f47b-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="1f47b-120">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-121">EventData</span><span class="sxs-lookup"><span data-stu-id="1f47b-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="1f47b-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-123">サーバー (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="1f47b-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="1f47b-124">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="1f47b-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="1f47b-126">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1f47b-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="1f47b-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="1f47b-128">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="1f47b-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="1f47b-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="1f47b-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="1f47b-132">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="1f47b-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="1f47b-134">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="1f47b-135">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="1f47b-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="1f47b-136">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="1f47b-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f47b-137">親要素</span><span class="sxs-lookup"><span data-stu-id="1f47b-137">Parent elements</span></span>

|<span data-ttu-id="1f47b-138">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f47b-138">**Element**</span></span>|<span data-ttu-id="1f47b-139">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f47b-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f47b-140">受信者 Trackingevents</span><span class="sxs-lookup"><span data-stu-id="1f47b-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="1f47b-141">受信者の1つまたは複数の追跡イベントのリストを格納します。</span><span class="sxs-lookup"><span data-stu-id="1f47b-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f47b-142">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1f47b-142">Text value</span></span>

<span data-ttu-id="1f47b-143">なし。</span><span class="sxs-lookup"><span data-stu-id="1f47b-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f47b-144">注釈</span><span class="sxs-lookup"><span data-stu-id="1f47b-144">Remarks</span></span>

<span data-ttu-id="1f47b-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1f47b-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f47b-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f47b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f47b-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f47b-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f47b-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f47b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="1f47b-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f47b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f47b-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f47b-150">Validation File</span></span>  <br/> |<span data-ttu-id="1f47b-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1f47b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f47b-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f47b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f47b-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f47b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f47b-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f47b-154">See also</span></span>



[<span data-ttu-id="1f47b-155">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="1f47b-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="1f47b-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f47b-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

