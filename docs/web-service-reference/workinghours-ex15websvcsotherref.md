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
description: WorkingHours 要素は、要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。
ms.openlocfilehash: c53779422b87adebed370a1ed88e4e91c7a2dcaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840032"
---
# <a name="workinghours"></a><span data-ttu-id="3fce2-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3fce2-103">WorkingHours</span></span>

<span data-ttu-id="3fce2-104">**WorkingHours**要素は、要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="3fce2-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="3fce2-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3fce2-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3fce2-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3fce2-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="3fce2-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3fce2-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="3fce2-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3fce2-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="3fce2-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3fce2-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="3fce2-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="3fce2-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fce2-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3fce2-111">Attributes and elements</span></span>

<span data-ttu-id="3fce2-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3fce2-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fce2-113">属性</span><span class="sxs-lookup"><span data-stu-id="3fce2-113">Attributes</span></span>

<span data-ttu-id="3fce2-114">なし。</span><span class="sxs-lookup"><span data-stu-id="3fce2-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fce2-115">子要素</span><span class="sxs-lookup"><span data-stu-id="3fce2-115">Child elements</span></span>

|<span data-ttu-id="3fce2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fce2-116">**Element**</span></span>|<span data-ttu-id="3fce2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fce2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fce2-118">タイムゾーン (可用性)</span><span class="sxs-lookup"><span data-stu-id="3fce2-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="3fce2-119">タイム ゾーン情報を識別する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fce2-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="3fce2-120">この要素には、標準時と夏時間の切り替えに関する情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fce2-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="3fce2-121">**WorkingHours**要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fce2-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="3fce2-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="3fce2-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="3fce2-123">メールボックス ユーザーについて、期間の作業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fce2-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="3fce2-124">**WorkingHours**要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fce2-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fce2-125">親要素</span><span class="sxs-lookup"><span data-stu-id="3fce2-125">Parent elements</span></span>

|<span data-ttu-id="3fce2-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fce2-126">**Element**</span></span>|<span data-ttu-id="3fce2-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fce2-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fce2-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3fce2-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="3fce2-129">特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fce2-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="3fce2-130">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3fce2-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3fce2-131">備考</span><span class="sxs-lookup"><span data-stu-id="3fce2-131">Remarks</span></span>

<span data-ttu-id="3fce2-132">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="3fce2-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="3fce2-133">この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。</span><span class="sxs-lookup"><span data-stu-id="3fce2-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="3fce2-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3fce2-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fce2-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="3fce2-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fce2-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="3fce2-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fce2-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3fce2-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3fce2-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3fce2-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fce2-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3fce2-139">Validation File</span></span>  <br/> |<span data-ttu-id="3fce2-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3fce2-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fce2-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3fce2-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fce2-142">False</span><span class="sxs-lookup"><span data-stu-id="3fce2-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fce2-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fce2-143">See also</span></span>



[<span data-ttu-id="3fce2-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="3fce2-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3fce2-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3fce2-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3fce2-146">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="3fce2-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

