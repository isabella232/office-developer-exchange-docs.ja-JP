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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468342"
---
# <a name="workinghours"></a><span data-ttu-id="d8c54-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d8c54-103">WorkingHours</span></span>

<span data-ttu-id="d8c54-104">**WorkingHours**要素は、要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。</span><span class="sxs-lookup"><span data-stu-id="d8c54-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="d8c54-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d8c54-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d8c54-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d8c54-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d8c54-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d8c54-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d8c54-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d8c54-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d8c54-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d8c54-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="d8c54-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="d8c54-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8c54-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d8c54-111">Attributes and elements</span></span>

<span data-ttu-id="d8c54-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d8c54-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8c54-113">属性</span><span class="sxs-lookup"><span data-stu-id="d8c54-113">Attributes</span></span>

<span data-ttu-id="d8c54-114">なし。</span><span class="sxs-lookup"><span data-stu-id="d8c54-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8c54-115">子要素</span><span class="sxs-lookup"><span data-stu-id="d8c54-115">Child elements</span></span>

|<span data-ttu-id="d8c54-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="d8c54-116">**Element**</span></span>|<span data-ttu-id="d8c54-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8c54-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c54-118">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="d8c54-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="d8c54-119">タイムゾーン情報を識別する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="d8c54-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="d8c54-120">この要素には、標準時から夏時間への切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="d8c54-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="d8c54-121">この要素は、 **WorkingHours**要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="d8c54-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="d8c54-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d8c54-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="d8c54-123">メールボックスユーザーの作業期間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="d8c54-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="d8c54-124">この要素は、 **WorkingHours**要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="d8c54-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8c54-125">親要素</span><span class="sxs-lookup"><span data-stu-id="d8c54-125">Parent elements</span></span>

|<span data-ttu-id="d8c54-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="d8c54-126">**Element**</span></span>|<span data-ttu-id="d8c54-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="d8c54-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8c54-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d8c54-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="d8c54-129">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="d8c54-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="d8c54-130">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d8c54-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8c54-131">注釈</span><span class="sxs-lookup"><span data-stu-id="d8c54-131">Remarks</span></span>

<span data-ttu-id="d8c54-132">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="d8c54-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="d8c54-133">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="d8c54-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="d8c54-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d8c54-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8c54-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d8c54-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8c54-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8c54-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8c54-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d8c54-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d8c54-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d8c54-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8c54-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d8c54-139">Validation File</span></span>  <br/> |<span data-ttu-id="d8c54-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d8c54-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8c54-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d8c54-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8c54-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="d8c54-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8c54-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="d8c54-143">See also</span></span>



[<span data-ttu-id="d8c54-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d8c54-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d8c54-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d8c54-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d8c54-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="d8c54-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

