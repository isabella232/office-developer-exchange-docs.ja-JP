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
description: RequestedView 要素は、クライアントが要求する予定表情報の種類を定義します。
ms.openlocfilehash: bc4f863841fc5a7d1d23f0bd4c7c2895d2593a2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459161"
---
# <a name="requestedview"></a><span data-ttu-id="baf0b-103">RequestedView</span><span class="sxs-lookup"><span data-stu-id="baf0b-103">RequestedView</span></span>

<span data-ttu-id="baf0b-104">**Requestedview**要素は、クライアントが要求する予定表情報の種類を定義します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-104">The **RequestedView** element defines the type of calendar information that a client requests.</span></span> 
  
[<span data-ttu-id="baf0b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="baf0b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="baf0b-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="baf0b-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="baf0b-107">RequestedView</span><span class="sxs-lookup"><span data-stu-id="baf0b-107">RequestedView</span></span>](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 <span data-ttu-id="baf0b-108">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="baf0b-108">**FreeBusyViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="baf0b-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="baf0b-109">Attributes and elements</span></span>

<span data-ttu-id="baf0b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="baf0b-111">属性</span><span class="sxs-lookup"><span data-stu-id="baf0b-111">Attributes</span></span>

<span data-ttu-id="baf0b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="baf0b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="baf0b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="baf0b-113">Child elements</span></span>

<span data-ttu-id="baf0b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="baf0b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="baf0b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="baf0b-115">Parent elements</span></span>

|<span data-ttu-id="baf0b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="baf0b-116">**Element**</span></span>|<span data-ttu-id="baf0b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="baf0b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="baf0b-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="baf0b-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="baf0b-119">応答で返される空き時間情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="baf0b-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="baf0b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="baf0b-121">Text value</span></span>

<span data-ttu-id="baf0b-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="baf0b-122">A text value is required.</span></span> <span data-ttu-id="baf0b-123">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="baf0b-124">**値**</span><span class="sxs-lookup"><span data-stu-id="baf0b-124">**Value**</span></span>|<span data-ttu-id="baf0b-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="baf0b-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="baf0b-126">なし</span><span class="sxs-lookup"><span data-stu-id="baf0b-126">None</span></span>  <br/> |<span data-ttu-id="baf0b-127">この値は、要求に対しては無効です。</span><span class="sxs-lookup"><span data-stu-id="baf0b-127">This value is not valid for requests.</span></span> <span data-ttu-id="baf0b-128">この値は、応答に対して有効です。</span><span class="sxs-lookup"><span data-stu-id="baf0b-128">This value is valid for responses.</span></span>  <br/> |
|<span data-ttu-id="baf0b-129">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="baf0b-129">MergedOnly</span></span>  <br/> |<span data-ttu-id="baf0b-130">集約された空き時間ストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-130">Represents an aggregated free/busy stream.</span></span> <span data-ttu-id="baf0b-131">1つのフォレストのターゲットユーザーが可用性サービスを構成していないフォレスト間のシナリオでは、リクエスターの可用性サービスが空き時間情報パブリックフォルダーからターゲットユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-131">In cross-forest scenarios in which the target user in one forest does not have an Availability service configured, the Availability service of the requestor retrieves the target user's free/busy information from the free/busy public folder.</span></span> <span data-ttu-id="baf0b-132">パブリックフォルダーは、空き時間情報のみをマージされた形式で格納するため、 **MergedOnly**のみが利用可能な情報です。</span><span class="sxs-lookup"><span data-stu-id="baf0b-132">Because public folders only store free/busy information in merged form, **MergedOnly** is the only available information.</span></span>  <br/> |
|<span data-ttu-id="baf0b-133">FreeBusy</span><span class="sxs-lookup"><span data-stu-id="baf0b-133">FreeBusy</span></span>  <br/> |<span data-ttu-id="baf0b-134">従来の状態の情報を表します。これは、空き時間、仮の予定、および OOF です。</span><span class="sxs-lookup"><span data-stu-id="baf0b-134">Represents the legacy status information: free, busy, tentative, and OOF.</span></span> <span data-ttu-id="baf0b-135">これには、予定の開始時刻と終了時刻も含まれます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-135">This also includes the start/end times of the appointments.</span></span> <span data-ttu-id="baf0b-136">このビューは、従来の空き時間表示よりも豊富です。個々の会議の開始時刻と終了時刻は、集計された空き時間ストリームの代わりに提供されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-136">This view is richer than the legacy free/busy view because individual meeting start and end times are provided instead of an aggregated free/busy stream.</span></span>  <br/> |
|<span data-ttu-id="baf0b-137">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="baf0b-137">FreeBusyMerged</span></span>  <br/> |<span data-ttu-id="baf0b-138">**FreeBusy**のすべてのプロパティを表し、結合された空き時間情報のストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-138">Represents all the properties in **FreeBusy** with a stream of merged free/busy information.</span></span>  <br/> |
|<span data-ttu-id="baf0b-139">詳細</span><span class="sxs-lookup"><span data-stu-id="baf0b-139">Detailed</span></span>  <br/> |<span data-ttu-id="baf0b-140">従来の状態の情報を表します。これは、空き時間、仮の予定、および OOF です。予定の開始/終了時刻。また、件名、場所、重要度など、予定のさまざまなプロパティを指定できます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-140">Represents the legacy status information: free, busy, tentative, and OOF; the start/end times of the appointments; and various properties of the appointment such as subject, location, and importance.</span></span> <span data-ttu-id="baf0b-141">この要求されたビューは、要求元ユーザーが特権を持っている情報の最大量を返します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-141">This requested view will return the maximum amount of information for which the requesting user is privileged.</span></span> <span data-ttu-id="baf0b-142">マージされた空き時間情報のみを使用できる場合は、Microsoft Exchange Server 2003 フォレスト内のユーザーに関する情報を要求すると、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-142">If merged free/busy information only is available, as with requesting information for users in a Microsoft Exchange Server 2003 forest, **MergedOnly** will be returned.</span></span> <span data-ttu-id="baf0b-143">それ以外の場合は、 **FreeBusy**または**Detailed**が返されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-143">Otherwise, **FreeBusy** or **Detailed** will be returned.</span></span>  <br/> |
|<span data-ttu-id="baf0b-144">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="baf0b-144">DetailedMerged</span></span>  <br/> |<span data-ttu-id="baf0b-145">結合された空き時間情報のストリームを使用して**詳細な**すべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="baf0b-145">Represents all the properties in **Detailed** with a stream of merged free/busy information.</span></span> <span data-ttu-id="baf0b-146">結合された空き時間情報のみを使用できる場合は、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-146">If merged free/busy information only is available, **MergedOnly** will be returned.</span></span> <span data-ttu-id="baf0b-147">それ以外の場合は、 **FreeBusyMerged**または**DetailedMerged**が返されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-147">Otherwise, **FreeBusyMerged** or **DetailedMerged** will be returned.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="baf0b-148">注釈</span><span class="sxs-lookup"><span data-stu-id="baf0b-148">Remarks</span></span>

<span data-ttu-id="baf0b-149">この要素によって設定された値は、応答の[FreeBusyViewType](freebusyviewtype.md)要素と共に返されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-149">The value set by this element is returned with the [FreeBusyViewType](freebusyviewtype.md) element in the response.</span></span> 
  
<span data-ttu-id="baf0b-150">次の表は、さまざまなビューの種類と、それに対応する MAPI プロパティに対して返されるものを示しています。</span><span class="sxs-lookup"><span data-stu-id="baf0b-150">The following table shows what is returned for the different view types and the corresponding MAPI property.</span></span> <span data-ttu-id="baf0b-151">各ビューの種類は、以前のビューの種類に基づいて作成されます。</span><span class="sxs-lookup"><span data-stu-id="baf0b-151">Each view type builds upon the former view type.</span></span>
  
|<span data-ttu-id="baf0b-152">**空き時間表示の種類**</span><span class="sxs-lookup"><span data-stu-id="baf0b-152">**Free/Busy View Type**</span></span>|<span data-ttu-id="baf0b-153">**Properties**</span><span class="sxs-lookup"><span data-stu-id="baf0b-153">**Properties**</span></span>|<span data-ttu-id="baf0b-154">**MAPI Calendar プロパティ**</span><span class="sxs-lookup"><span data-stu-id="baf0b-154">**MAPI Calendar Property**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="baf0b-155">**MergedOnly**</span><span class="sxs-lookup"><span data-stu-id="baf0b-155">**MergedOnly**</span></span> <br/> |<span data-ttu-id="baf0b-156">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="baf0b-156">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="baf0b-157">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="baf0b-157">**FreeBusy**</span></span> <br/> |<span data-ttu-id="baf0b-158">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="baf0b-158">Classical status</span></span>  <br/> |<span data-ttu-id="baf0b-159">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="baf0b-159">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="baf0b-160">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="baf0b-160">**FreeBusy**</span></span> <br/> |<span data-ttu-id="baf0b-161">就業時間</span><span class="sxs-lookup"><span data-stu-id="baf0b-161">Working hours</span></span>  <br/> ||
|<span data-ttu-id="baf0b-162">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="baf0b-162">**FreeBusy**</span></span> <br/> |<span data-ttu-id="baf0b-163">開始時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-163">Start time</span></span>  <br/> |<span data-ttu-id="baf0b-164">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-164">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-165">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="baf0b-165">**FreeBusy**</span></span> <br/> |<span data-ttu-id="baf0b-166">終了時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-166">End time</span></span>  <br/> |<span data-ttu-id="baf0b-167">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-167">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-168">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-168">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="baf0b-169">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="baf0b-169">Classical status</span></span>  <br/> |<span data-ttu-id="baf0b-170">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="baf0b-170">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="baf0b-171">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-171">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="baf0b-172">就業時間</span><span class="sxs-lookup"><span data-stu-id="baf0b-172">Working hours</span></span>  <br/> ||
|<span data-ttu-id="baf0b-173">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-173">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="baf0b-174">開始時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-174">Start time</span></span>  <br/> |<span data-ttu-id="baf0b-175">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-175">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-176">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-176">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="baf0b-177">終了時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-177">End time</span></span>  <br/> |<span data-ttu-id="baf0b-178">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-178">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-179">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-179">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="baf0b-180">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="baf0b-180">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="baf0b-181">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-181">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-182">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="baf0b-182">Classical status</span></span>  <br/> |<span data-ttu-id="baf0b-183">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="baf0b-183">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="baf0b-184">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-184">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-185">就業時間</span><span class="sxs-lookup"><span data-stu-id="baf0b-185">Working hours</span></span>  <br/> ||
|<span data-ttu-id="baf0b-186">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-186">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-187">開始時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-187">Start time</span></span>  <br/> |<span data-ttu-id="baf0b-188">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-188">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-189">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-189">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-190">終了時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-190">End time</span></span>  <br/> |<span data-ttu-id="baf0b-191">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-191">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-192">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-192">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-193">件名</span><span class="sxs-lookup"><span data-stu-id="baf0b-193">Subject</span></span>  <br/> |<span data-ttu-id="baf0b-194">PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="baf0b-194">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="baf0b-195">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-195">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-196">場所</span><span class="sxs-lookup"><span data-stu-id="baf0b-196">Location</span></span>  <br/> |<span data-ttu-id="baf0b-197">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="baf0b-197">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="baf0b-198">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-198">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-199">エントリ Id (プライベートでない場合)</span><span class="sxs-lookup"><span data-stu-id="baf0b-199">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="baf0b-200">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-200">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-201">プライベートフラグ</span><span class="sxs-lookup"><span data-stu-id="baf0b-201">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="baf0b-202">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-202">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-203">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="baf0b-203">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="baf0b-204">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-204">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-205">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="baf0b-205">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="baf0b-206">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-206">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-207">IsException</span><span class="sxs-lookup"><span data-stu-id="baf0b-207">IsException</span></span>  <br/> ||
|<span data-ttu-id="baf0b-208">**詳細**</span><span class="sxs-lookup"><span data-stu-id="baf0b-208">**Detailed**</span></span> <br/> |<span data-ttu-id="baf0b-209">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="baf0b-209">IsReminderSet</span></span>  <br/> ||
|<span data-ttu-id="baf0b-210">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-210">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-211">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="baf0b-211">Classical status</span></span>  <br/> |<span data-ttu-id="baf0b-212">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="baf0b-212">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="baf0b-213">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-213">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-214">就業時間</span><span class="sxs-lookup"><span data-stu-id="baf0b-214">Working hours</span></span>  <br/> ||
|<span data-ttu-id="baf0b-215">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-215">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-216">開始時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-216">Start time</span></span>  <br/> |<span data-ttu-id="baf0b-217">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-217">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-218">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-218">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-219">終了時刻</span><span class="sxs-lookup"><span data-stu-id="baf0b-219">End time</span></span>  <br/> |<span data-ttu-id="baf0b-220">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="baf0b-220">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="baf0b-221">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-221">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-222">件名</span><span class="sxs-lookup"><span data-stu-id="baf0b-222">Subject</span></span>  <br/> |<span data-ttu-id="baf0b-223">PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="baf0b-223">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="baf0b-224">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-224">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-225">場所</span><span class="sxs-lookup"><span data-stu-id="baf0b-225">Location</span></span>  <br/> |<span data-ttu-id="baf0b-226">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="baf0b-226">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="baf0b-227">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-227">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-228">エントリ Id (プライベートでない場合)</span><span class="sxs-lookup"><span data-stu-id="baf0b-228">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="baf0b-229">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-229">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-230">プライベートフラグ</span><span class="sxs-lookup"><span data-stu-id="baf0b-230">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="baf0b-231">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-231">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-232">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="baf0b-232">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="baf0b-233">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-233">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-234">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="baf0b-234">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="baf0b-235">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-235">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-236">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="baf0b-236">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="baf0b-237">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-237">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-238">IsException</span><span class="sxs-lookup"><span data-stu-id="baf0b-238">IsException</span></span>  <br/> ||
|<span data-ttu-id="baf0b-239">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="baf0b-239">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="baf0b-240">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="baf0b-240">IsReminderSet</span></span>  <br/> ||
   
## <a name="element-information"></a><span data-ttu-id="baf0b-241">要素の情報</span><span class="sxs-lookup"><span data-stu-id="baf0b-241">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="baf0b-242">Namespace</span><span class="sxs-lookup"><span data-stu-id="baf0b-242">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="baf0b-243">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="baf0b-243">Schema Name</span></span>  <br/> |<span data-ttu-id="baf0b-244">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="baf0b-244">Types schema</span></span>  <br/> |
|<span data-ttu-id="baf0b-245">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="baf0b-245">Validation File</span></span>  <br/> |<span data-ttu-id="baf0b-246">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="baf0b-246">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="baf0b-247">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="baf0b-247">Can be Empty</span></span>  <br/> |<span data-ttu-id="baf0b-248">正しくない</span><span class="sxs-lookup"><span data-stu-id="baf0b-248">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="baf0b-249">関連項目</span><span class="sxs-lookup"><span data-stu-id="baf0b-249">See also</span></span>



[<span data-ttu-id="baf0b-250">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="baf0b-250">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="baf0b-251">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="baf0b-251">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

