---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: FreeBusyViewType 要素は、応答で返される空き時間情報の種類を表します。
ms.openlocfilehash: 3556ad236693ac9aa018b8aa3af7843765da6aa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459568"
---
# <a name="freebusyviewtype"></a><span data-ttu-id="1d91d-103">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="1d91d-103">FreeBusyViewType</span></span>

<span data-ttu-id="1d91d-104">**FreeBusyViewType**要素は、応答で返される空き時間情報の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-104">The **FreeBusyViewType** element represents the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="1d91d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d91d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1d91d-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1d91d-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1d91d-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1d91d-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1d91d-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1d91d-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1d91d-109">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="1d91d-109">FreeBusyViewType</span></span>](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
```

 <span data-ttu-id="1d91d-110">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="1d91d-110">**FreeBusyViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d91d-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1d91d-111">Attributes and elements</span></span>

<span data-ttu-id="1d91d-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d91d-113">属性</span><span class="sxs-lookup"><span data-stu-id="1d91d-113">Attributes</span></span>

<span data-ttu-id="1d91d-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1d91d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d91d-115">子要素</span><span class="sxs-lookup"><span data-stu-id="1d91d-115">Child elements</span></span>

<span data-ttu-id="1d91d-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1d91d-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d91d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1d91d-117">Parent elements</span></span>

|<span data-ttu-id="1d91d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d91d-118">**Element**</span></span>|<span data-ttu-id="1d91d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d91d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d91d-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1d91d-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="1d91d-121">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="1d91d-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="1d91d-122">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d91d-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1d91d-123">Text value</span></span>

<span data-ttu-id="1d91d-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-124">A text value is required.</span></span> <span data-ttu-id="1d91d-125">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-125">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="1d91d-126">**値**</span><span class="sxs-lookup"><span data-stu-id="1d91d-126">**Value**</span></span>|<span data-ttu-id="1d91d-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d91d-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1d91d-128">なし</span><span class="sxs-lookup"><span data-stu-id="1d91d-128">None</span></span>  <br/> |<span data-ttu-id="1d91d-129">この値は、要求に対しては無効です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-129">This value is not valid for requests.</span></span> <span data-ttu-id="1d91d-130">この値は、応答に対して有効です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-130">This value is valid for responses.</span></span>  <br/> |
|<span data-ttu-id="1d91d-131">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="1d91d-131">MergedOnly</span></span>  <br/> |<span data-ttu-id="1d91d-132">集約された空き時間ストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-132">Represents an aggregated free/busy stream.</span></span> <span data-ttu-id="1d91d-133">1つのフォレストのターゲットユーザーが可用性サービスを構成していないフォレスト間のシナリオでは、リクエスターの可用性サービスが空き時間情報パブリックフォルダーからターゲットユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-133">In cross-forest scenarios in which the target user in one forest does not have an Availability service configured, the Availability service of the requestor retrieves the target user's free/busy information from the free/busy public folder.</span></span> <span data-ttu-id="1d91d-134">パブリックフォルダーは、空き時間情報のみをマージされた形式で格納するため、 **MergedOnly**のみが利用可能な情報です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-134">Because public folders only store free/busy information in merged form, **MergedOnly** is the only available information.</span></span>  <br/> |
|<span data-ttu-id="1d91d-135">FreeBusy</span><span class="sxs-lookup"><span data-stu-id="1d91d-135">FreeBusy</span></span>  <br/> |<span data-ttu-id="1d91d-136">従来の状態の情報を表します。これは、空き時間、仮の予定、および OOF です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-136">Represents the legacy status information: free, busy, tentative, and OOF.</span></span> <span data-ttu-id="1d91d-137">これには、予定の開始時刻と終了時刻も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-137">This also includes the start/end times of the appointments.</span></span> <span data-ttu-id="1d91d-138">このビューは、従来の空き時間表示よりも豊富です。個々の会議の開始時刻と終了時刻は、集計された空き時間ストリームの代わりに提供されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-138">This view is richer than the legacy free/busy view because individual meeting start and end times are provided instead of an aggregated free/busy stream.</span></span>  <br/> |
|<span data-ttu-id="1d91d-139">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="1d91d-139">FreeBusyMerged</span></span>  <br/> |<span data-ttu-id="1d91d-140">**FreeBusy**のすべてのプロパティを表し、マージされた空き時間情報を含むストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-140">Represents all the properties in **FreeBusy** with a stream of merged free/busy availability information.</span></span>  <br/> |
|<span data-ttu-id="1d91d-141">詳細</span><span class="sxs-lookup"><span data-stu-id="1d91d-141">Detailed</span></span>  <br/> |<span data-ttu-id="1d91d-142">従来の状態の情報を表します。これは、空き時間、仮の予定、および OOF です。予定の開始/終了時刻。また、件名、場所、重要度など、予定のさまざまなプロパティを指定できます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-142">Represents the legacy status information: free, busy, tentative, and OOF; the start/end times of the appointments; and various properties of the appointment such as subject, location, and importance.</span></span> <span data-ttu-id="1d91d-143">この要求されたビューは、要求元ユーザーが特権を持っている情報の最大量を返します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-143">This requested view will return the maximum amount of information for which the requesting user is privileged.</span></span> <span data-ttu-id="1d91d-144">マージされた空き時間情報のみを使用できる場合は、Microsoft Exchange Server 2003 フォレスト内のユーザーに関する情報を要求すると、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-144">If merged free/busy information only is available, as with requesting information for users in a Microsoft Exchange Server 2003 forest, **MergedOnly** will be returned.</span></span> <span data-ttu-id="1d91d-145">それ以外の場合は、 **FreeBusy**または**Detailed**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-145">Otherwise, **FreeBusy** or **Detailed** will be returned.</span></span>  <br/> <span data-ttu-id="1d91d-146">配布リストに**詳細**が指定されている場合は、リストのメンバーの空き時間情報が結合され、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-146">If **Detailed** is specified for a distribution list, the free/busy information for the members of the list is merged, and **MergedOnly** is returned.</span></span>  <br/> |
|<span data-ttu-id="1d91d-147">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="1d91d-147">DetailedMerged</span></span>  <br/> |<span data-ttu-id="1d91d-148">マージされた空き時間情報のストリームに**詳細**が含まれるすべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1d91d-148">Represents all the properties in **Detailed** with a stream of merged free/busy availability information.</span></span> <span data-ttu-id="1d91d-149">マージされた空き時間情報のみが利用可能な場合 (たとえば、Exchange 2003 を実行しているコンピューター上にメールボックスが存在する場合)、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-149">If only merged free/busy information is available, for example if the mailbox exists on a computer running Exchange 2003, **MergedOnly** will be returned.</span></span> <span data-ttu-id="1d91d-150">それ以外の場合は、 **FreeBusyMerged**または**DetailedMerged**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-150">Otherwise, **FreeBusyMerged** or **DetailedMerged** will be returned.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d91d-151">注釈</span><span class="sxs-lookup"><span data-stu-id="1d91d-151">Remarks</span></span>

<span data-ttu-id="1d91d-152">この要素は、 [FreeBusyView](freebusyview.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="1d91d-152">This element is required if the [FreeBusyView](freebusyview.md) element is used.</span></span> <span data-ttu-id="1d91d-153">返される空き時間情報の種類は、 [Requestedview](requestedview.md)要素で指定されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-153">The type of free/busy information returned is designated in the [RequestedView](requestedview.md) element.</span></span> <span data-ttu-id="1d91d-154">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1d91d-154">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="1d91d-155">次の表は、さまざまなビューの種類と、それに対応する MAPI プロパティに対して返されるものを示しています。</span><span class="sxs-lookup"><span data-stu-id="1d91d-155">The following table shows what is returned for the different view types and the corresponding MAPI property.</span></span> <span data-ttu-id="1d91d-156">各ビューの種類は、以前のビューの種類に基づいて作成されます。</span><span class="sxs-lookup"><span data-stu-id="1d91d-156">Each view type builds upon the former view type.</span></span>
  
|<span data-ttu-id="1d91d-157">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="1d91d-157">**FreeBusyViewType**</span></span>|<span data-ttu-id="1d91d-158">**Properties**</span><span class="sxs-lookup"><span data-stu-id="1d91d-158">**Properties**</span></span>|<span data-ttu-id="1d91d-159">**MAPI Calendar プロパティ**</span><span class="sxs-lookup"><span data-stu-id="1d91d-159">**MAPI Calendar Property**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1d91d-160">**MergedOnly**</span><span class="sxs-lookup"><span data-stu-id="1d91d-160">**MergedOnly**</span></span> <br/> |<span data-ttu-id="1d91d-161">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1d91d-161">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1d91d-162">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="1d91d-162">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1d91d-163">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="1d91d-163">Classical status</span></span>  <br/> |<span data-ttu-id="1d91d-164">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1d91d-164">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1d91d-165">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="1d91d-165">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1d91d-166">就業時間</span><span class="sxs-lookup"><span data-stu-id="1d91d-166">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1d91d-167">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="1d91d-167">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1d91d-168">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-168">Start time</span></span>  <br/> |<span data-ttu-id="1d91d-169">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-169">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-170">**FreeBusy**</span><span class="sxs-lookup"><span data-stu-id="1d91d-170">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1d91d-171">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-171">End time</span></span>  <br/> |<span data-ttu-id="1d91d-172">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-172">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-173">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-173">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1d91d-174">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="1d91d-174">Classical status</span></span>  <br/> |<span data-ttu-id="1d91d-175">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1d91d-175">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1d91d-176">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-176">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1d91d-177">就業時間</span><span class="sxs-lookup"><span data-stu-id="1d91d-177">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1d91d-178">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-178">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1d91d-179">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-179">Start time</span></span>  <br/> |<span data-ttu-id="1d91d-180">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-180">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-181">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-181">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1d91d-182">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-182">End time</span></span>  <br/> |<span data-ttu-id="1d91d-183">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-183">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-184">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-184">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1d91d-185">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1d91d-185">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1d91d-186">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-186">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-187">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="1d91d-187">Classical status</span></span>  <br/> |<span data-ttu-id="1d91d-188">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1d91d-188">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1d91d-189">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-189">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-190">就業時間</span><span class="sxs-lookup"><span data-stu-id="1d91d-190">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1d91d-191">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-191">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-192">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-192">Start time</span></span>  <br/> |<span data-ttu-id="1d91d-193">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-193">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-194">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-194">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-195">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-195">End time</span></span>  <br/> |<span data-ttu-id="1d91d-196">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-196">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-197">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-197">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-198">件名</span><span class="sxs-lookup"><span data-stu-id="1d91d-198">Subject</span></span>  <br/> |<span data-ttu-id="1d91d-199">PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="1d91d-199">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="1d91d-200">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-200">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-201">場所</span><span class="sxs-lookup"><span data-stu-id="1d91d-201">Location</span></span>  <br/> |<span data-ttu-id="1d91d-202">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="1d91d-202">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="1d91d-203">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-203">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-204">エントリ Id (プライベートでない場合)</span><span class="sxs-lookup"><span data-stu-id="1d91d-204">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="1d91d-205">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-205">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-206">プライベートフラグ</span><span class="sxs-lookup"><span data-stu-id="1d91d-206">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="1d91d-207">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-207">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-208">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="1d91d-208">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="1d91d-209">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-209">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-210">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="1d91d-210">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="1d91d-211">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-211">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-212">IsException</span><span class="sxs-lookup"><span data-stu-id="1d91d-212">IsException</span></span>  <br/> ||
|<span data-ttu-id="1d91d-213">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-213">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-214">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="1d91d-214">IsReminderSet</span></span>  <br/> ||
|<span data-ttu-id="1d91d-215">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1d91d-215">**Detailed**</span></span> <br/> |<span data-ttu-id="1d91d-216">不在時のメッセージ (要求された場合)</span><span class="sxs-lookup"><span data-stu-id="1d91d-216">Out of Office Message (if requested)</span></span>  <br/> ||
|<span data-ttu-id="1d91d-217">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-217">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-218">クラシック状態</span><span class="sxs-lookup"><span data-stu-id="1d91d-218">Classical status</span></span>  <br/> |<span data-ttu-id="1d91d-219">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1d91d-219">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1d91d-220">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-220">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-221">就業時間</span><span class="sxs-lookup"><span data-stu-id="1d91d-221">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1d91d-222">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-222">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-223">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-223">Start time</span></span>  <br/> |<span data-ttu-id="1d91d-224">PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-224">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-225">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-225">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-226">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1d91d-226">End time</span></span>  <br/> |<span data-ttu-id="1d91d-227">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1d91d-227">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1d91d-228">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-228">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-229">件名</span><span class="sxs-lookup"><span data-stu-id="1d91d-229">Subject</span></span>  <br/> |<span data-ttu-id="1d91d-230">PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="1d91d-230">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="1d91d-231">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-231">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-232">場所</span><span class="sxs-lookup"><span data-stu-id="1d91d-232">Location</span></span>  <br/> |<span data-ttu-id="1d91d-233">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="1d91d-233">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="1d91d-234">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-234">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-235">エントリ Id (プライベートでない場合)</span><span class="sxs-lookup"><span data-stu-id="1d91d-235">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="1d91d-236">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-236">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-237">プライベートフラグ</span><span class="sxs-lookup"><span data-stu-id="1d91d-237">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="1d91d-238">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-238">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-239">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1d91d-239">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1d91d-240">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-240">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-241">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="1d91d-241">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="1d91d-242">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-242">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-243">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="1d91d-243">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="1d91d-244">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-244">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-245">IsException</span><span class="sxs-lookup"><span data-stu-id="1d91d-245">IsException</span></span>  <br/> ||
|<span data-ttu-id="1d91d-246">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1d91d-246">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1d91d-247">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="1d91d-247">IsReminderSet</span></span>  <br/> ||
   
## <a name="element-information"></a><span data-ttu-id="1d91d-248">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1d91d-248">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d91d-249">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d91d-249">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d91d-250">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d91d-250">Schema Name</span></span>  <br/> |<span data-ttu-id="1d91d-251">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1d91d-251">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d91d-252">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d91d-252">Validation File</span></span>  <br/> |<span data-ttu-id="1d91d-253">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1d91d-253">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d91d-254">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d91d-254">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d91d-255">正しくない</span><span class="sxs-lookup"><span data-stu-id="1d91d-255">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d91d-256">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d91d-256">See also</span></span>



[<span data-ttu-id="1d91d-257">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1d91d-257">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1d91d-258">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d91d-258">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1d91d-259">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="1d91d-259">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

