---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: RequestedView 要素は、クライアントが要求する予定表の情報の種類を定義します。
ms.openlocfilehash: 7710227720264432c325f95da894cbbbd4748dc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833145"
---
# <a name="requestedview"></a><span data-ttu-id="a0910-103">RequestedView</span><span class="sxs-lookup"><span data-stu-id="a0910-103">RequestedView</span></span>

<span data-ttu-id="a0910-104">**RequestedView**要素は、クライアントが要求する予定表の情報の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="a0910-104">The **RequestedView** element defines the type of calendar information that a client requests.</span></span> 
  
[<span data-ttu-id="a0910-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a0910-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="a0910-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="a0910-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="a0910-107">RequestedView</span><span class="sxs-lookup"><span data-stu-id="a0910-107">RequestedView</span></span>](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 <span data-ttu-id="a0910-108">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="a0910-108">**FreeBusyViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0910-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a0910-109">Attributes and elements</span></span>

<span data-ttu-id="a0910-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0910-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0910-111">属性</span><span class="sxs-lookup"><span data-stu-id="a0910-111">Attributes</span></span>

<span data-ttu-id="a0910-112">なし。</span><span class="sxs-lookup"><span data-stu-id="a0910-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0910-113">子要素</span><span class="sxs-lookup"><span data-stu-id="a0910-113">Child elements</span></span>

<span data-ttu-id="a0910-114">なし。</span><span class="sxs-lookup"><span data-stu-id="a0910-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0910-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a0910-115">Parent elements</span></span>

|<span data-ttu-id="a0910-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a0910-116">**Element**</span></span>|<span data-ttu-id="a0910-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0910-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0910-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="a0910-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="a0910-119">応答で返される空き時間情報の情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0910-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="a0910-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="a0910-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0910-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a0910-121">Text value</span></span>

<span data-ttu-id="a0910-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="a0910-122">A text value is required.</span></span> <span data-ttu-id="a0910-123">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="a0910-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="a0910-124">**値**</span><span class="sxs-lookup"><span data-stu-id="a0910-124">**Value**</span></span>|<span data-ttu-id="a0910-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0910-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0910-126">なし</span><span class="sxs-lookup"><span data-stu-id="a0910-126">None</span></span>  <br/> |<span data-ttu-id="a0910-127">この値は、要求に対して有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="a0910-127">This value is not valid for requests.</span></span> <span data-ttu-id="a0910-128">この値は応答をします。</span><span class="sxs-lookup"><span data-stu-id="a0910-128">This value is valid for responses.</span></span>  <br/> |
|<span data-ttu-id="a0910-129">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="a0910-129">MergedOnly</span></span>  <br/> |<span data-ttu-id="a0910-130">集計の空き/予約済みのストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="a0910-130">Represents an aggregated free/busy stream.</span></span> <span data-ttu-id="a0910-131">1 つのフォレスト内の移動先のユーザーが、可用性サービスが構成されているフォレスト間のシナリオでは、要求側の可用性サービスは、空き時間情報パブリック フォルダーからターゲット ユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="a0910-131">In cross-forest scenarios in which the target user in one forest does not have an Availability service configured, the Availability service of the requestor retrieves the target user's free/busy information from the free/busy public folder.</span></span> <span data-ttu-id="a0910-132">パブリック フォルダーは、差し込み印刷の形式でのみ空き時間情報を格納するため**MergedOnly**はのみ利用可能な情報です。</span><span class="sxs-lookup"><span data-stu-id="a0910-132">Because public folders only store free/busy information in merged form, **MergedOnly** is the only available information.</span></span>  <br/> |
|<span data-ttu-id="a0910-133">空き時間情報</span><span class="sxs-lookup"><span data-stu-id="a0910-133">FreeBusy</span></span>  <br/> |<span data-ttu-id="a0910-134">従来のステータス情報を表します。 フリー、予定あり、仮の予定、および不在時。</span><span class="sxs-lookup"><span data-stu-id="a0910-134">Represents the legacy status information: free, busy, tentative, and OOF.</span></span> <span data-ttu-id="a0910-135">これには、予定の開始/終了時刻も含まれています。</span><span class="sxs-lookup"><span data-stu-id="a0910-135">This also includes the start/end times of the appointments.</span></span> <span data-ttu-id="a0910-136">このビューは、豊富な集計の空き時間情報のストリームではなく、時間が用意されている個々 の会議の開始し、終了のために表示、レガシ空き時間情報よりも。</span><span class="sxs-lookup"><span data-stu-id="a0910-136">This view is richer than the legacy free/busy view because individual meeting start and end times are provided instead of an aggregated free/busy stream.</span></span>  <br/> |
|<span data-ttu-id="a0910-137">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="a0910-137">FreeBusyMerged</span></span>  <br/> |<span data-ttu-id="a0910-138">結合された空き時間情報のストリームを**空き時間情報**のすべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a0910-138">Represents all the properties in **FreeBusy** with a stream of merged free/busy information.</span></span>  <br/> |
|<span data-ttu-id="a0910-139">Detailed</span><span class="sxs-lookup"><span data-stu-id="a0910-139">Detailed</span></span>  <br/> |<span data-ttu-id="a0910-140">従来のステータス情報を表します: 無料、ビジー状態で、仮の予定と OOF。予定の開始/終了時刻予定の件名、場所、および重要度などのさまざまなプロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="a0910-140">Represents the legacy status information: free, busy, tentative, and OOF; the start/end times of the appointments; and various properties of the appointment such as subject, location, and importance.</span></span> <span data-ttu-id="a0910-141">この要求されたビューでは、要求元のユーザーの特権の情報量の最大を返します。</span><span class="sxs-lookup"><span data-stu-id="a0910-141">This requested view will return the maximum amount of information for which the requesting user is privileged.</span></span> <span data-ttu-id="a0910-142">結合された空き時間情報のみがある場合と、Microsoft Exchange Server 2003 フォレスト内のユーザーの情報を要求すると**MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="a0910-142">If merged free/busy information only is available, as with requesting information for users in a Microsoft Exchange Server 2003 forest, **MergedOnly** will be returned.</span></span> <span data-ttu-id="a0910-143">それ以外の場合、**空き時間情報**や**詳細**が返されます。</span><span class="sxs-lookup"><span data-stu-id="a0910-143">Otherwise, **FreeBusy** or **Detailed** will be returned.</span></span>  <br/> |
|<span data-ttu-id="a0910-144">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="a0910-144">DetailedMerged</span></span>  <br/> |<span data-ttu-id="a0910-145">ストリーム マージされた空き時間情報の**詳細**のすべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a0910-145">Represents all the properties in **Detailed** with a stream of merged free/busy information.</span></span> <span data-ttu-id="a0910-146">結合された空き時間情報のみがある場合、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="a0910-146">If merged free/busy information only is available, **MergedOnly** will be returned.</span></span> <span data-ttu-id="a0910-147">それ以外の場合、 **FreeBusyMerged**または**DetailedMerged**が返されます。</span><span class="sxs-lookup"><span data-stu-id="a0910-147">Otherwise, **FreeBusyMerged** or **DetailedMerged** will be returned.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0910-148">備考</span><span class="sxs-lookup"><span data-stu-id="a0910-148">Remarks</span></span>

<span data-ttu-id="a0910-149">応答内の[FreeBusyViewType](freebusyviewtype.md)要素には、この要素によって設定された値が返されます。</span><span class="sxs-lookup"><span data-stu-id="a0910-149">The value set by this element is returned with the [FreeBusyViewType](freebusyviewtype.md) element in the response.</span></span> 
  
<span data-ttu-id="a0910-150">次の表は、別のビューの種類と対応する MAPI プロパティに対して返されるを示します。</span><span class="sxs-lookup"><span data-stu-id="a0910-150">The following table shows what is returned for the different view types and the corresponding MAPI property.</span></span> <span data-ttu-id="a0910-151">各ビューの種類は、以前のビューの種類に基づいて構築します。</span><span class="sxs-lookup"><span data-stu-id="a0910-151">Each view type builds upon the former view type.</span></span>
  
|<span data-ttu-id="a0910-152">**空き時間情報の表示の種類**</span><span class="sxs-lookup"><span data-stu-id="a0910-152">**Free/Busy View Type**</span></span>|<span data-ttu-id="a0910-153">**新しいプロパティ**</span><span class="sxs-lookup"><span data-stu-id="a0910-153">**Properties**</span></span>|<span data-ttu-id="a0910-154">**MAPI 予定表のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="a0910-154">**MAPI Calendar Property**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0910-155">**MergedOnly**</span><span class="sxs-lookup"><span data-stu-id="a0910-155">**MergedOnly**</span></span> <br/> |<span data-ttu-id="a0910-156">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="a0910-156">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="a0910-157">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="a0910-157">**FreeBusy**</span></span> <br/> |<span data-ttu-id="a0910-158">古典の状態</span><span class="sxs-lookup"><span data-stu-id="a0910-158">Classical status</span></span>  <br/> |<span data-ttu-id="a0910-159">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="a0910-159">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="a0910-160">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="a0910-160">**FreeBusy**</span></span> <br/> |<span data-ttu-id="a0910-161">作業時間</span><span class="sxs-lookup"><span data-stu-id="a0910-161">Working hours</span></span>  <br/> ||
|<span data-ttu-id="a0910-162">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="a0910-162">**FreeBusy**</span></span> <br/> |<span data-ttu-id="a0910-163">開始時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-163">Start time</span></span>  <br/> |<span data-ttu-id="a0910-164">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-164">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-165">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="a0910-165">**FreeBusy**</span></span> <br/> |<span data-ttu-id="a0910-166">終了時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-166">End time</span></span>  <br/> |<span data-ttu-id="a0910-167">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-167">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-168">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-168">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="a0910-169">古典の状態</span><span class="sxs-lookup"><span data-stu-id="a0910-169">Classical status</span></span>  <br/> |<span data-ttu-id="a0910-170">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="a0910-170">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="a0910-171">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-171">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="a0910-172">作業時間</span><span class="sxs-lookup"><span data-stu-id="a0910-172">Working hours</span></span>  <br/> ||
|<span data-ttu-id="a0910-173">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-173">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="a0910-174">開始時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-174">Start time</span></span>  <br/> |<span data-ttu-id="a0910-175">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-175">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-176">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-176">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="a0910-177">終了時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-177">End time</span></span>  <br/> |<span data-ttu-id="a0910-178">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-178">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-179">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-179">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="a0910-180">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="a0910-180">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="a0910-181">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-181">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-182">古典の状態</span><span class="sxs-lookup"><span data-stu-id="a0910-182">Classical status</span></span>  <br/> |<span data-ttu-id="a0910-183">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="a0910-183">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="a0910-184">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-184">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-185">作業時間</span><span class="sxs-lookup"><span data-stu-id="a0910-185">Working hours</span></span>  <br/> ||
|<span data-ttu-id="a0910-186">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-186">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-187">開始時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-187">Start time</span></span>  <br/> |<span data-ttu-id="a0910-188">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-188">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-189">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-189">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-190">終了時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-190">End time</span></span>  <br/> |<span data-ttu-id="a0910-191">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-191">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-192">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-192">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-193">件名</span><span class="sxs-lookup"><span data-stu-id="a0910-193">Subject</span></span>  <br/> |<span data-ttu-id="a0910-194">あるの PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="a0910-194">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="a0910-195">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-195">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-196">場所</span><span class="sxs-lookup"><span data-stu-id="a0910-196">Location</span></span>  <br/> |<span data-ttu-id="a0910-197">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="a0910-197">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="a0910-198">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-198">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-199">エントリ Id(unless private)</span><span class="sxs-lookup"><span data-stu-id="a0910-199">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="a0910-200">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-200">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-201">プライベート フラグ</span><span class="sxs-lookup"><span data-stu-id="a0910-201">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="a0910-202">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-202">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-203">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="a0910-203">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="a0910-204">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-204">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-205">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="a0910-205">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="a0910-206">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-206">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-207">IsException</span><span class="sxs-lookup"><span data-stu-id="a0910-207">IsException</span></span>  <br/> ||
|<span data-ttu-id="a0910-208">**詳細**</span><span class="sxs-lookup"><span data-stu-id="a0910-208">**Detailed**</span></span> <br/> |<span data-ttu-id="a0910-209">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="a0910-209">IsReminderSet</span></span>  <br/> ||
|<span data-ttu-id="a0910-210">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-210">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-211">古典の状態</span><span class="sxs-lookup"><span data-stu-id="a0910-211">Classical status</span></span>  <br/> |<span data-ttu-id="a0910-212">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="a0910-212">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="a0910-213">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-213">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-214">作業時間</span><span class="sxs-lookup"><span data-stu-id="a0910-214">Working hours</span></span>  <br/> ||
|<span data-ttu-id="a0910-215">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-215">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-216">開始時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-216">Start time</span></span>  <br/> |<span data-ttu-id="a0910-217">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-217">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-218">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-218">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-219">終了時刻</span><span class="sxs-lookup"><span data-stu-id="a0910-219">End time</span></span>  <br/> |<span data-ttu-id="a0910-220">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="a0910-220">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="a0910-221">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-221">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-222">件名</span><span class="sxs-lookup"><span data-stu-id="a0910-222">Subject</span></span>  <br/> |<span data-ttu-id="a0910-223">あるの PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="a0910-223">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="a0910-224">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-224">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-225">場所</span><span class="sxs-lookup"><span data-stu-id="a0910-225">Location</span></span>  <br/> |<span data-ttu-id="a0910-226">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="a0910-226">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="a0910-227">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-227">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-228">エントリ Id(unless private)</span><span class="sxs-lookup"><span data-stu-id="a0910-228">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="a0910-229">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-229">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-230">プライベート フラグ</span><span class="sxs-lookup"><span data-stu-id="a0910-230">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="a0910-231">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-231">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-232">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="a0910-232">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="a0910-233">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-233">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-234">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="a0910-234">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="a0910-235">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-235">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-236">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="a0910-236">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="a0910-237">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-237">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-238">IsException</span><span class="sxs-lookup"><span data-stu-id="a0910-238">IsException</span></span>  <br/> ||
|<span data-ttu-id="a0910-239">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="a0910-239">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="a0910-240">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="a0910-240">IsReminderSet</span></span>  <br/> ||
   
## <a name="element-information"></a><span data-ttu-id="a0910-241">要素情報</span><span class="sxs-lookup"><span data-stu-id="a0910-241">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0910-242">名前空間</span><span class="sxs-lookup"><span data-stu-id="a0910-242">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0910-243">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a0910-243">Schema Name</span></span>  <br/> |<span data-ttu-id="a0910-244">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a0910-244">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0910-245">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a0910-245">Validation File</span></span>  <br/> |<span data-ttu-id="a0910-246">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0910-246">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0910-247">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a0910-247">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0910-248">False</span><span class="sxs-lookup"><span data-stu-id="a0910-248">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0910-249">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0910-249">See also</span></span>



[<span data-ttu-id="a0910-250">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="a0910-250">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="a0910-251">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="a0910-251">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

