---
title: WorkingPeriod
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriod
api_type:
- schema
ms.assetid: 3b4e48af-9880-42b9-a0dc-dae7ac43c264
description: WorkingPeriod 要素には、メールボックスユーザーの勤務週の曜日と時間が含まれます。
ms.openlocfilehash: 5c217169fb193d4bb6dae4e18570873d55de6127
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459680"
---
# <a name="workingperiod"></a><span data-ttu-id="24f9a-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="24f9a-103">WorkingPeriod</span></span>

<span data-ttu-id="24f9a-104">**WorkingPeriod**要素には、メールボックスユーザーの勤務週の曜日と時間が含まれます。</span><span class="sxs-lookup"><span data-stu-id="24f9a-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="24f9a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="24f9a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="24f9a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="24f9a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="24f9a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="24f9a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="24f9a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="24f9a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="24f9a-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="24f9a-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="24f9a-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="24f9a-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="24f9a-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="24f9a-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="24f9a-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="24f9a-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24f9a-113">属性と要素</span><span class="sxs-lookup"><span data-stu-id="24f9a-113">Attributes and elements</span></span>

<span data-ttu-id="24f9a-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="24f9a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24f9a-115">属性</span><span class="sxs-lookup"><span data-stu-id="24f9a-115">Attributes</span></span>

<span data-ttu-id="24f9a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="24f9a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24f9a-117">子要素</span><span class="sxs-lookup"><span data-stu-id="24f9a-117">Child elements</span></span>

|<span data-ttu-id="24f9a-118">**Element**</span><span class="sxs-lookup"><span data-stu-id="24f9a-118">**Element**</span></span>|<span data-ttu-id="24f9a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="24f9a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f9a-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="24f9a-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="24f9a-121">メールボックスユーザーに対してスケジュールされた稼働日の一覧が含まれます。</span><span class="sxs-lookup"><span data-stu-id="24f9a-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="24f9a-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="24f9a-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="24f9a-123">メールボックスユーザーの稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="24f9a-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="24f9a-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="24f9a-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="24f9a-125">メールボックスユーザーの稼働日の終了日を表します。</span><span class="sxs-lookup"><span data-stu-id="24f9a-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24f9a-126">親要素</span><span class="sxs-lookup"><span data-stu-id="24f9a-126">Parent elements</span></span>

|<span data-ttu-id="24f9a-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="24f9a-127">**Element**</span></span>|<span data-ttu-id="24f9a-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="24f9a-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f9a-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="24f9a-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="24f9a-130">メールボックスユーザーの作業期間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="24f9a-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="24f9a-131">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="24f9a-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24f9a-132">注釈</span><span class="sxs-lookup"><span data-stu-id="24f9a-132">Remarks</span></span>

<span data-ttu-id="24f9a-133">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="24f9a-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="24f9a-134">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="24f9a-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24f9a-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="24f9a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24f9a-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="24f9a-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24f9a-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="24f9a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="24f9a-138">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="24f9a-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="24f9a-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="24f9a-139">Validation File</span></span>  <br/> |<span data-ttu-id="24f9a-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="24f9a-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24f9a-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="24f9a-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="24f9a-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="24f9a-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24f9a-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="24f9a-143">See also</span></span>



[<span data-ttu-id="24f9a-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="24f9a-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="24f9a-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="24f9a-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="24f9a-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="24f9a-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

