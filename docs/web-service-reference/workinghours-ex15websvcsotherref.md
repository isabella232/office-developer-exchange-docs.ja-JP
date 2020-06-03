---
title: WorkingHours
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: WorkingHours 要素は、要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。
ms.openlocfilehash: 9cb21e72f7024b96b4b5f252a8a3b85bb704e67c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468342"
---
# <a name="workinghours"></a><span data-ttu-id="e09de-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="e09de-103">WorkingHours</span></span>

<span data-ttu-id="e09de-104">**WorkingHours**要素は、要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。</span><span class="sxs-lookup"><span data-stu-id="e09de-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="e09de-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e09de-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e09de-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="e09de-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="e09de-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="e09de-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="e09de-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e09de-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="e09de-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="e09de-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="e09de-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="e09de-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e09de-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e09de-111">Attributes and elements</span></span>

<span data-ttu-id="e09de-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e09de-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e09de-113">属性</span><span class="sxs-lookup"><span data-stu-id="e09de-113">Attributes</span></span>

<span data-ttu-id="e09de-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e09de-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e09de-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e09de-115">Child elements</span></span>

|<span data-ttu-id="e09de-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="e09de-116">**Element**</span></span>|<span data-ttu-id="e09de-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e09de-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e09de-118">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="e09de-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="e09de-119">タイムゾーン情報を識別する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="e09de-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="e09de-120">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="e09de-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="e09de-121">この要素は、 **WorkingHours**要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="e09de-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="e09de-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="e09de-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="e09de-123">メールボックスユーザーの作業期間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="e09de-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="e09de-124">この要素は、 **WorkingHours**要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="e09de-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e09de-125">親要素</span><span class="sxs-lookup"><span data-stu-id="e09de-125">Parent elements</span></span>

|<span data-ttu-id="e09de-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="e09de-126">**Element**</span></span>|<span data-ttu-id="e09de-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="e09de-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e09de-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e09de-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="e09de-129">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="e09de-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="e09de-130">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e09de-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e09de-131">注釈</span><span class="sxs-lookup"><span data-stu-id="e09de-131">Remarks</span></span>

<span data-ttu-id="e09de-132">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="e09de-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="e09de-133">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="e09de-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="e09de-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e09de-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e09de-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e09de-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e09de-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e09de-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e09de-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e09de-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e09de-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e09de-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="e09de-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e09de-139">Validation File</span></span>  <br/> |<span data-ttu-id="e09de-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e09de-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e09de-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e09de-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="e09de-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="e09de-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e09de-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="e09de-143">See also</span></span>



[<span data-ttu-id="e09de-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e09de-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e09de-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e09de-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e09de-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="e09de-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

