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
description: MergedFreeBusy 要素には、マージされた空き時間情報データ ストリームが含まれています。
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832449"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="f39ac-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="f39ac-103">MergedFreeBusy</span></span>

<span data-ttu-id="f39ac-104">**MergedFreeBusy**要素には、マージされた空き時間情報データ ストリームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f39ac-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="f39ac-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f39ac-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f39ac-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f39ac-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f39ac-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f39ac-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f39ac-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f39ac-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f39ac-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="f39ac-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="f39ac-110">**string**</span><span class="sxs-lookup"><span data-stu-id="f39ac-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f39ac-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f39ac-111">Attributes and elements</span></span>

<span data-ttu-id="f39ac-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f39ac-113">属性</span><span class="sxs-lookup"><span data-stu-id="f39ac-113">Attributes</span></span>

<span data-ttu-id="f39ac-114">なし。</span><span class="sxs-lookup"><span data-stu-id="f39ac-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f39ac-115">子要素</span><span class="sxs-lookup"><span data-stu-id="f39ac-115">Child elements</span></span>

<span data-ttu-id="f39ac-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f39ac-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f39ac-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f39ac-117">Parent elements</span></span>

|<span data-ttu-id="f39ac-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f39ac-118">**Element**</span></span>|<span data-ttu-id="f39ac-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f39ac-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f39ac-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f39ac-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="f39ac-121">特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f39ac-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="f39ac-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f39ac-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f39ac-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f39ac-123">Text value</span></span>

<span data-ttu-id="f39ac-124">テキスト値は、 [FreeBusyViewType](freebusyviewtype.md)要素の値は、次のいずれかの場合、サーバーにより提供されます。</span><span class="sxs-lookup"><span data-stu-id="f39ac-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="f39ac-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="f39ac-125">DetailedMerged</span></span>
    
- <span data-ttu-id="f39ac-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="f39ac-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="f39ac-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="f39ac-127">MergedOnly</span></span>
    
<span data-ttu-id="f39ac-128">テキスト値は、空き時間情報のストリームです。</span><span class="sxs-lookup"><span data-stu-id="f39ac-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f39ac-129">備考</span><span class="sxs-lookup"><span data-stu-id="f39ac-129">Remarks</span></span>

<span data-ttu-id="f39ac-130">この要素によって提供されるデータのストリームは、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)と[時間](timewindow.md)の要素によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="f39ac-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="f39ac-131">[時間](timewindow.md)要素では、可用性のクエリを実行する時間間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="f39ac-132">[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素は、 **MergedFreeBusy**要素で返される間隔に[時間](timewindow.md)の要素からの時間を分割する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="f39ac-133">**MergedFreeBusy**ストリームのそれぞれの数値は、 [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素で定義されている 1 つの間隔を表します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="f39ac-134">次の表は、個々 の間隔の可能な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="f39ac-135">**桁**</span><span class="sxs-lookup"><span data-stu-id="f39ac-135">**Digit**</span></span>|<span data-ttu-id="f39ac-136">**可用性**</span><span class="sxs-lookup"><span data-stu-id="f39ac-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f39ac-137">0</span><span class="sxs-lookup"><span data-stu-id="f39ac-137">0</span></span>  <br/> |<span data-ttu-id="f39ac-138">Free</span><span class="sxs-lookup"><span data-stu-id="f39ac-138">Free</span></span>  <br/> |
|<span data-ttu-id="f39ac-139">1</span><span class="sxs-lookup"><span data-stu-id="f39ac-139">1</span></span>  <br/> |<span data-ttu-id="f39ac-140">Tentative</span><span class="sxs-lookup"><span data-stu-id="f39ac-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="f39ac-141">2</span><span class="sxs-lookup"><span data-stu-id="f39ac-141">2</span></span>  <br/> |<span data-ttu-id="f39ac-142">Busy</span><span class="sxs-lookup"><span data-stu-id="f39ac-142">Busy</span></span>  <br/> |
|<span data-ttu-id="f39ac-143">3</span><span class="sxs-lookup"><span data-stu-id="f39ac-143">3</span></span>  <br/> |<span data-ttu-id="f39ac-144">不在時 (OOF)</span><span class="sxs-lookup"><span data-stu-id="f39ac-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="f39ac-145">4</span><span class="sxs-lookup"><span data-stu-id="f39ac-145">4</span></span>  <br/> |<span data-ttu-id="f39ac-146">データがありません。</span><span class="sxs-lookup"><span data-stu-id="f39ac-146">No data</span></span>  <br/> |
   
<span data-ttu-id="f39ac-147">たとえば、空き時間情報データに対する要求には、4 つの時間を表す[時間](timewindow.md)の要素と 60 分を表す[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f39ac-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="f39ac-148">要求されたユーザーの予定表では、不在時の最初の 60 分間、次の 90 分の時間と時間ウィンドウで、最後の 90 分間予定されていない**MergedFreeBusy**ストリームなります 3220。</span><span class="sxs-lookup"><span data-stu-id="f39ac-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="f39ac-149">間隔には、2 つ以上の可用性のクラス分けが含まれています、その間隔を分類する最上位の番号が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f39ac-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="f39ac-150">この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="f39ac-151">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f39ac-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f39ac-152">要素情報</span><span class="sxs-lookup"><span data-stu-id="f39ac-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f39ac-153">名前空間</span><span class="sxs-lookup"><span data-stu-id="f39ac-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f39ac-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f39ac-154">Schema Name</span></span>  <br/> |<span data-ttu-id="f39ac-155">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f39ac-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="f39ac-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f39ac-156">Validation File</span></span>  <br/> |<span data-ttu-id="f39ac-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f39ac-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f39ac-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f39ac-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="f39ac-159">False</span><span class="sxs-lookup"><span data-stu-id="f39ac-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f39ac-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="f39ac-160">See also</span></span>



[<span data-ttu-id="f39ac-161">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f39ac-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f39ac-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f39ac-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f39ac-163">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="f39ac-163">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

