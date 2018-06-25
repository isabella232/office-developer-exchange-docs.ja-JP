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
description: FreeBusyViewType 要素は、応答で返される空き時間情報の情報の種類を表します。
ms.openlocfilehash: fe965d062f72d99dff7148f4d00b12fd8c4e1366
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760617"
---
# <a name="freebusyviewtype"></a><span data-ttu-id="1cefd-103">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="1cefd-103">FreeBusyViewType</span></span>

<span data-ttu-id="1cefd-104">**FreeBusyViewType**要素は、応答で返される空き時間情報の情報の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-104">The **FreeBusyViewType** element represents the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="1cefd-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1cefd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1cefd-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1cefd-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1cefd-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1cefd-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1cefd-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1cefd-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1cefd-109">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="1cefd-109">FreeBusyViewType</span></span>](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
```

 <span data-ttu-id="1cefd-110">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="1cefd-110">**FreeBusyViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cefd-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1cefd-111">Attributes and elements</span></span>

<span data-ttu-id="1cefd-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cefd-113">属性</span><span class="sxs-lookup"><span data-stu-id="1cefd-113">Attributes</span></span>

<span data-ttu-id="1cefd-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1cefd-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cefd-115">子要素</span><span class="sxs-lookup"><span data-stu-id="1cefd-115">Child elements</span></span>

<span data-ttu-id="1cefd-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1cefd-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1cefd-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1cefd-117">Parent elements</span></span>

|<span data-ttu-id="1cefd-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cefd-118">**Element**</span></span>|<span data-ttu-id="1cefd-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cefd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cefd-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1cefd-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="1cefd-121">特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cefd-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="1cefd-122">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1cefd-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1cefd-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1cefd-123">Text value</span></span>

<span data-ttu-id="1cefd-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1cefd-124">A text value is required.</span></span> <span data-ttu-id="1cefd-125">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-125">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="1cefd-126">**値**</span><span class="sxs-lookup"><span data-stu-id="1cefd-126">**Value**</span></span>|<span data-ttu-id="1cefd-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cefd-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1cefd-128">なし</span><span class="sxs-lookup"><span data-stu-id="1cefd-128">None</span></span>  <br/> |<span data-ttu-id="1cefd-129">この値は、要求に対して有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="1cefd-129">This value is not valid for requests.</span></span> <span data-ttu-id="1cefd-130">この値は応答をします。</span><span class="sxs-lookup"><span data-stu-id="1cefd-130">This value is valid for responses.</span></span>  <br/> |
|<span data-ttu-id="1cefd-131">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="1cefd-131">MergedOnly</span></span>  <br/> |<span data-ttu-id="1cefd-132">集計の空き/予約済みのストリームを表します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-132">Represents an aggregated free/busy stream.</span></span> <span data-ttu-id="1cefd-133">1 つのフォレスト内の移動先のユーザーが、可用性サービスが構成されているフォレスト間のシナリオでは、要求側の可用性サービスは、空き時間情報パブリック フォルダーからターゲット ユーザーの空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-133">In cross-forest scenarios in which the target user in one forest does not have an Availability service configured, the Availability service of the requestor retrieves the target user's free/busy information from the free/busy public folder.</span></span> <span data-ttu-id="1cefd-134">パブリック フォルダーは、差し込み印刷の形式でのみ空き時間情報を格納するため**MergedOnly**はのみ利用可能な情報です。</span><span class="sxs-lookup"><span data-stu-id="1cefd-134">Because public folders only store free/busy information in merged form, **MergedOnly** is the only available information.</span></span>  <br/> |
|<span data-ttu-id="1cefd-135">空き時間情報</span><span class="sxs-lookup"><span data-stu-id="1cefd-135">FreeBusy</span></span>  <br/> |<span data-ttu-id="1cefd-136">従来のステータス情報を表します。 フリー、予定あり、仮の予定、および不在時。</span><span class="sxs-lookup"><span data-stu-id="1cefd-136">Represents the legacy status information: free, busy, tentative, and OOF.</span></span> <span data-ttu-id="1cefd-137">これには、予定の開始/終了時刻も含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cefd-137">This also includes the start/end times of the appointments.</span></span> <span data-ttu-id="1cefd-138">このビューは、豊富な集計の空き時間情報のストリームではなく、時間が用意されている個々 の会議の開始し、終了のために表示、レガシ空き時間情報よりも。</span><span class="sxs-lookup"><span data-stu-id="1cefd-138">This view is richer than the legacy free/busy view because individual meeting start and end times are provided instead of an aggregated free/busy stream.</span></span>  <br/> |
|<span data-ttu-id="1cefd-139">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="1cefd-139">FreeBusyMerged</span></span>  <br/> |<span data-ttu-id="1cefd-140">結合された空き時間情報の可用性情報のストリームを**空き時間情報**のすべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-140">Represents all the properties in **FreeBusy** with a stream of merged free/busy availability information.</span></span>  <br/> |
|<span data-ttu-id="1cefd-141">Detailed</span><span class="sxs-lookup"><span data-stu-id="1cefd-141">Detailed</span></span>  <br/> |<span data-ttu-id="1cefd-142">従来のステータス情報を表します: 無料、ビジー状態で、仮の予定と OOF。予定の開始/終了時刻予定の件名、場所、および重要度などのさまざまなプロパティを選択します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-142">Represents the legacy status information: free, busy, tentative, and OOF; the start/end times of the appointments; and various properties of the appointment such as subject, location, and importance.</span></span> <span data-ttu-id="1cefd-143">この要求されたビューでは、要求元のユーザーの特権の情報量の最大を返します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-143">This requested view will return the maximum amount of information for which the requesting user is privileged.</span></span> <span data-ttu-id="1cefd-144">結合された空き時間情報のみがある場合と、Microsoft Exchange Server 2003 フォレスト内のユーザーの情報を要求すると**MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-144">If merged free/busy information only is available, as with requesting information for users in a Microsoft Exchange Server 2003 forest, **MergedOnly** will be returned.</span></span> <span data-ttu-id="1cefd-145">それ以外の場合、**空き時間情報**や**詳細**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-145">Otherwise, **FreeBusy** or **Detailed** will be returned.</span></span>  <br/> <span data-ttu-id="1cefd-146">配布リストの**詳細**を指定すると、そのリストのメンバーの空き時間情報が差し込まれると、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-146">If **Detailed** is specified for a distribution list, the free/busy information for the members of the list is merged, and **MergedOnly** is returned.</span></span>  <br/> |
|<span data-ttu-id="1cefd-147">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="1cefd-147">DetailedMerged</span></span>  <br/> |<span data-ttu-id="1cefd-148">ストリームの結合された空き時間情報の可用性情報の**詳細**のすべてのプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-148">Represents all the properties in **Detailed** with a stream of merged free/busy availability information.</span></span> <span data-ttu-id="1cefd-149">結合された空き時間情報がある、たとえば、メールボックスが Exchange 2003 を実行するコンピューター上に存在する場合、だけの場合は、 **MergedOnly**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-149">If only merged free/busy information is available, for example if the mailbox exists on a computer running Exchange 2003, **MergedOnly** will be returned.</span></span> <span data-ttu-id="1cefd-150">それ以外の場合、 **FreeBusyMerged**または**DetailedMerged**が返されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-150">Otherwise, **FreeBusyMerged** or **DetailedMerged** will be returned.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1cefd-151">備考</span><span class="sxs-lookup"><span data-stu-id="1cefd-151">Remarks</span></span>

<span data-ttu-id="1cefd-152">[FreeBusyView](freebusyview.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cefd-152">This element is required if the [FreeBusyView](freebusyview.md) element is used.</span></span> <span data-ttu-id="1cefd-153">返される空き時間情報の種類は、 [RequestedView](requestedview.md)要素で指定されます。</span><span class="sxs-lookup"><span data-stu-id="1cefd-153">The type of free/busy information returned is designated in the [RequestedView](requestedview.md) element.</span></span> <span data-ttu-id="1cefd-154">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1cefd-154">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="1cefd-155">次の表は、別のビューの種類と対応する MAPI プロパティに対して返されるを示します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-155">The following table shows what is returned for the different view types and the corresponding MAPI property.</span></span> <span data-ttu-id="1cefd-156">各ビューの種類は、以前のビューの種類に基づいて構築します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-156">Each view type builds upon the former view type.</span></span>
  
|<span data-ttu-id="1cefd-157">**FreeBusyViewType**</span><span class="sxs-lookup"><span data-stu-id="1cefd-157">**FreeBusyViewType**</span></span>|<span data-ttu-id="1cefd-158">**新しいプロパティ**</span><span class="sxs-lookup"><span data-stu-id="1cefd-158">**Properties**</span></span>|<span data-ttu-id="1cefd-159">**MAPI 予定表のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="1cefd-159">**MAPI Calendar Property**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1cefd-160">**MergedOnly**</span><span class="sxs-lookup"><span data-stu-id="1cefd-160">**MergedOnly**</span></span> <br/> |<span data-ttu-id="1cefd-161">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1cefd-161">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1cefd-162">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="1cefd-162">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1cefd-163">古典の状態</span><span class="sxs-lookup"><span data-stu-id="1cefd-163">Classical status</span></span>  <br/> |<span data-ttu-id="1cefd-164">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1cefd-164">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1cefd-165">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="1cefd-165">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1cefd-166">作業時間</span><span class="sxs-lookup"><span data-stu-id="1cefd-166">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1cefd-167">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="1cefd-167">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1cefd-168">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-168">Start time</span></span>  <br/> |<span data-ttu-id="1cefd-169">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-169">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-170">**空き時間情報**</span><span class="sxs-lookup"><span data-stu-id="1cefd-170">**FreeBusy**</span></span> <br/> |<span data-ttu-id="1cefd-171">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-171">End time</span></span>  <br/> |<span data-ttu-id="1cefd-172">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-172">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-173">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-173">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1cefd-174">古典の状態</span><span class="sxs-lookup"><span data-stu-id="1cefd-174">Classical status</span></span>  <br/> |<span data-ttu-id="1cefd-175">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1cefd-175">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1cefd-176">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-176">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1cefd-177">作業時間</span><span class="sxs-lookup"><span data-stu-id="1cefd-177">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1cefd-178">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-178">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1cefd-179">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-179">Start time</span></span>  <br/> |<span data-ttu-id="1cefd-180">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-180">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-181">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-181">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1cefd-182">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-182">End time</span></span>  <br/> |<span data-ttu-id="1cefd-183">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-183">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-184">**FreeBusyMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-184">**FreeBusyMerged**</span></span> <br/> |<span data-ttu-id="1cefd-185">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1cefd-185">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1cefd-186">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-186">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-187">古典の状態</span><span class="sxs-lookup"><span data-stu-id="1cefd-187">Classical status</span></span>  <br/> |<span data-ttu-id="1cefd-188">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1cefd-188">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1cefd-189">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-189">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-190">作業時間</span><span class="sxs-lookup"><span data-stu-id="1cefd-190">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1cefd-191">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-191">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-192">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-192">Start time</span></span>  <br/> |<span data-ttu-id="1cefd-193">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-193">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-194">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-194">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-195">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-195">End time</span></span>  <br/> |<span data-ttu-id="1cefd-196">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-196">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-197">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-197">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-198">件名</span><span class="sxs-lookup"><span data-stu-id="1cefd-198">Subject</span></span>  <br/> |<span data-ttu-id="1cefd-199">あるの PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="1cefd-199">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="1cefd-200">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-200">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-201">場所</span><span class="sxs-lookup"><span data-stu-id="1cefd-201">Location</span></span>  <br/> |<span data-ttu-id="1cefd-202">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="1cefd-202">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="1cefd-203">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-203">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-204">エントリ Id(unless private)</span><span class="sxs-lookup"><span data-stu-id="1cefd-204">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="1cefd-205">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-205">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-206">プライベート フラグ</span><span class="sxs-lookup"><span data-stu-id="1cefd-206">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="1cefd-207">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-207">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-208">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="1cefd-208">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="1cefd-209">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-209">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-210">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="1cefd-210">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="1cefd-211">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-211">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-212">IsException</span><span class="sxs-lookup"><span data-stu-id="1cefd-212">IsException</span></span>  <br/> ||
|<span data-ttu-id="1cefd-213">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-213">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-214">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="1cefd-214">IsReminderSet</span></span>  <br/> ||
|<span data-ttu-id="1cefd-215">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1cefd-215">**Detailed**</span></span> <br/> |<span data-ttu-id="1cefd-216">Office のメッセージ (要求された場合)</span><span class="sxs-lookup"><span data-stu-id="1cefd-216">Out of Office Message (if requested)</span></span>  <br/> ||
|<span data-ttu-id="1cefd-217">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-217">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-218">古典の状態</span><span class="sxs-lookup"><span data-stu-id="1cefd-218">Classical status</span></span>  <br/> |<span data-ttu-id="1cefd-219">PropTag (0x80860003)</span><span class="sxs-lookup"><span data-stu-id="1cefd-219">PropTag (0x80860003)</span></span>  <br/> |
|<span data-ttu-id="1cefd-220">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-220">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-221">作業時間</span><span class="sxs-lookup"><span data-stu-id="1cefd-221">Working hours</span></span>  <br/> ||
|<span data-ttu-id="1cefd-222">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-222">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-223">開始時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-223">Start time</span></span>  <br/> |<span data-ttu-id="1cefd-224">単に PR_START_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-224">PR_START_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-225">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-225">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-226">終了時刻</span><span class="sxs-lookup"><span data-stu-id="1cefd-226">End time</span></span>  <br/> |<span data-ttu-id="1cefd-227">PR_END_DATE</span><span class="sxs-lookup"><span data-stu-id="1cefd-227">PR_END_DATE</span></span>  <br/> |
|<span data-ttu-id="1cefd-228">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-228">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-229">件名</span><span class="sxs-lookup"><span data-stu-id="1cefd-229">Subject</span></span>  <br/> |<span data-ttu-id="1cefd-230">あるの PR_SUBJECT</span><span class="sxs-lookup"><span data-stu-id="1cefd-230">PR_SUBJECT</span></span>  <br/> |
|<span data-ttu-id="1cefd-231">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-231">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-232">場所</span><span class="sxs-lookup"><span data-stu-id="1cefd-232">Location</span></span>  <br/> |<span data-ttu-id="1cefd-233">PR_LOCATION</span><span class="sxs-lookup"><span data-stu-id="1cefd-233">PR_LOCATION</span></span>  <br/> |
|<span data-ttu-id="1cefd-234">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-234">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-235">エントリ Id(unless private)</span><span class="sxs-lookup"><span data-stu-id="1cefd-235">Entry-Id(unless private)</span></span>  <br/> ||
|<span data-ttu-id="1cefd-236">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-236">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-237">プライベート フラグ</span><span class="sxs-lookup"><span data-stu-id="1cefd-237">Private Flag</span></span>  <br/> ||
|<span data-ttu-id="1cefd-238">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-238">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-239">MergedFreeBusyStream</span><span class="sxs-lookup"><span data-stu-id="1cefd-239">MergedFreeBusyStream</span></span>  <br/> ||
|<span data-ttu-id="1cefd-240">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-240">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-241">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="1cefd-241">IsMeeting</span></span>  <br/> ||
|<span data-ttu-id="1cefd-242">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-242">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-243">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="1cefd-243">IsRecurring</span></span>  <br/> ||
|<span data-ttu-id="1cefd-244">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-244">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-245">IsException</span><span class="sxs-lookup"><span data-stu-id="1cefd-245">IsException</span></span>  <br/> ||
|<span data-ttu-id="1cefd-246">**DetailedMerged**</span><span class="sxs-lookup"><span data-stu-id="1cefd-246">**DetailedMerged**</span></span> <br/> |<span data-ttu-id="1cefd-247">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="1cefd-247">IsReminderSet</span></span>  <br/> ||
   
## <a name="element-information"></a><span data-ttu-id="1cefd-248">要素情報</span><span class="sxs-lookup"><span data-stu-id="1cefd-248">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cefd-249">名前空間</span><span class="sxs-lookup"><span data-stu-id="1cefd-249">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cefd-250">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cefd-250">Schema Name</span></span>  <br/> |<span data-ttu-id="1cefd-251">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1cefd-251">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cefd-252">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cefd-252">Validation File</span></span>  <br/> |<span data-ttu-id="1cefd-253">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1cefd-253">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cefd-254">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1cefd-254">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cefd-255">False</span><span class="sxs-lookup"><span data-stu-id="1cefd-255">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cefd-256">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cefd-256">See also</span></span>



[<span data-ttu-id="1cefd-257">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1cefd-257">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1cefd-258">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1cefd-258">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1cefd-259">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1cefd-259">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

