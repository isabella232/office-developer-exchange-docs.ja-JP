---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: MergedFreeBusy 要素には、データのマージされた空き時間ストリームが含まれています。
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468727"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="3272a-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="3272a-103">MergedFreeBusy</span></span>

<span data-ttu-id="3272a-104">**MergedFreeBusy**要素には、データのマージされた空き時間ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3272a-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="3272a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3272a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3272a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3272a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="3272a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3272a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="3272a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3272a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="3272a-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="3272a-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="3272a-110">**string**</span><span class="sxs-lookup"><span data-stu-id="3272a-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3272a-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3272a-111">Attributes and elements</span></span>

<span data-ttu-id="3272a-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3272a-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3272a-113">属性</span><span class="sxs-lookup"><span data-stu-id="3272a-113">Attributes</span></span>

<span data-ttu-id="3272a-114">なし。</span><span class="sxs-lookup"><span data-stu-id="3272a-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3272a-115">子要素</span><span class="sxs-lookup"><span data-stu-id="3272a-115">Child elements</span></span>

<span data-ttu-id="3272a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="3272a-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3272a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="3272a-117">Parent elements</span></span>

|<span data-ttu-id="3272a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="3272a-118">**Element**</span></span>|<span data-ttu-id="3272a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="3272a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3272a-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3272a-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="3272a-121">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="3272a-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="3272a-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3272a-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3272a-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3272a-123">Text value</span></span>

<span data-ttu-id="3272a-124">[FreeBusyViewType](freebusyviewtype.md)要素の値が次のいずれかの場合、サーバーによってテキスト値が提供されます。</span><span class="sxs-lookup"><span data-stu-id="3272a-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="3272a-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="3272a-125">DetailedMerged</span></span>
    
- <span data-ttu-id="3272a-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="3272a-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="3272a-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="3272a-127">MergedOnly</span></span>
    
<span data-ttu-id="3272a-128">テキスト値は、空き時間情報のストリームです。</span><span class="sxs-lookup"><span data-stu-id="3272a-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3272a-129">注釈</span><span class="sxs-lookup"><span data-stu-id="3272a-129">Remarks</span></span>

<span data-ttu-id="3272a-130">この要素によって提供されるデータのストリームは、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素および[TimeWindow](timewindow.md)要素によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="3272a-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="3272a-131">[TimeWindow](timewindow.md)要素は、可用性を照会した期間を定義します。</span><span class="sxs-lookup"><span data-stu-id="3272a-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="3272a-132">[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素は、 [TimeWindow](timewindow.md)要素からの時間を**MergedFreeBusy**要素で返される間隔にどのように分割するかを定義します。</span><span class="sxs-lookup"><span data-stu-id="3272a-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="3272a-133">**MergedFreeBusy** stream の各数値は、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素によって定義された1つの間隔を表します。</span><span class="sxs-lookup"><span data-stu-id="3272a-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="3272a-134">次の表に、個別の間隔に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="3272a-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="3272a-135">**進数**</span><span class="sxs-lookup"><span data-stu-id="3272a-135">**Digit**</span></span>|<span data-ttu-id="3272a-136">**可用性**</span><span class="sxs-lookup"><span data-stu-id="3272a-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3272a-137">.0</span><span class="sxs-lookup"><span data-stu-id="3272a-137">0</span></span>  <br/> |<span data-ttu-id="3272a-138">空き</span><span class="sxs-lookup"><span data-stu-id="3272a-138">Free</span></span>  <br/> |
|<span data-ttu-id="3272a-139">1 </span><span class="sxs-lookup"><span data-stu-id="3272a-139">1</span></span>  <br/> |<span data-ttu-id="3272a-140">仮の予定</span><span class="sxs-lookup"><span data-stu-id="3272a-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="3272a-141">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3272a-141">2</span></span>  <br/> |<span data-ttu-id="3272a-142">多忙</span><span class="sxs-lookup"><span data-stu-id="3272a-142">Busy</span></span>  <br/> |
|<span data-ttu-id="3272a-143">1/3</span><span class="sxs-lookup"><span data-stu-id="3272a-143">3</span></span>  <br/> |<span data-ttu-id="3272a-144">不在時 (OOF)</span><span class="sxs-lookup"><span data-stu-id="3272a-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="3272a-145">4 </span><span class="sxs-lookup"><span data-stu-id="3272a-145">4</span></span>  <br/> |<span data-ttu-id="3272a-146">データなし</span><span class="sxs-lookup"><span data-stu-id="3272a-146">No data</span></span>  <br/> |
   
<span data-ttu-id="3272a-147">たとえば、空き時間情報データの要求には、4時間を表す[TimeWindow](timewindow.md)要素と、60分を表す[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3272a-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="3272a-148">要求されたユーザーの予定表が、最初の60分間、次の90分間、およびタイムウィンドウの最終の90分に対して予定外となっている場合、 **MergedFreeBusy**ストリームは3220になります。</span><span class="sxs-lookup"><span data-stu-id="3272a-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="3272a-149">間隔に複数の可用性分類が含まれている場合は、その間隔を分類するために最大数が使用されます。</span><span class="sxs-lookup"><span data-stu-id="3272a-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="3272a-150">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="3272a-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="3272a-151">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3272a-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3272a-152">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3272a-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3272a-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="3272a-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3272a-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3272a-154">Schema Name</span></span>  <br/> |<span data-ttu-id="3272a-155">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3272a-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="3272a-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3272a-156">Validation File</span></span>  <br/> |<span data-ttu-id="3272a-157">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3272a-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3272a-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3272a-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="3272a-159">正しくない</span><span class="sxs-lookup"><span data-stu-id="3272a-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3272a-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="3272a-160">See also</span></span>



[<span data-ttu-id="3272a-161">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="3272a-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3272a-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3272a-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3272a-163">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="3272a-163">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

