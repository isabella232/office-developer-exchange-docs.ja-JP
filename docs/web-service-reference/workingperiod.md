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
description: WorkingPeriod 要素には、日、およびメールボックス ユーザーの時間の作業週が含まれています。
ms.openlocfilehash: 0f2707bede5e49174ed62a35ba704e39c0c48e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840044"
---
# <a name="workingperiod"></a><span data-ttu-id="a3b73-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a3b73-103">WorkingPeriod</span></span>

<span data-ttu-id="a3b73-104">**WorkingPeriod**要素には、日、およびメールボックス ユーザーの時間の作業週が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3b73-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="a3b73-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3b73-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a3b73-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a3b73-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="a3b73-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a3b73-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="a3b73-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a3b73-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="a3b73-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="a3b73-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="a3b73-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="a3b73-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="a3b73-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a3b73-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="a3b73-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="a3b73-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3b73-113">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a3b73-113">Attributes and elements</span></span>

<span data-ttu-id="a3b73-114">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3b73-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3b73-115">属性</span><span class="sxs-lookup"><span data-stu-id="a3b73-115">Attributes</span></span>

<span data-ttu-id="a3b73-116">なし。</span><span class="sxs-lookup"><span data-stu-id="a3b73-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3b73-117">子要素</span><span class="sxs-lookup"><span data-stu-id="a3b73-117">Child elements</span></span>

|<span data-ttu-id="a3b73-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="a3b73-118">**Element**</span></span>|<span data-ttu-id="a3b73-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3b73-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3b73-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="a3b73-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="a3b73-121">メールボックス ユーザーのスケジュールの稼働日のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3b73-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="a3b73-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a3b73-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="a3b73-123">メールボックスがユーザーの稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="a3b73-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="a3b73-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="a3b73-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="a3b73-125">メールボックスがユーザーの稼働日の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="a3b73-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3b73-126">親要素</span><span class="sxs-lookup"><span data-stu-id="a3b73-126">Parent elements</span></span>

|<span data-ttu-id="a3b73-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="a3b73-127">**Element**</span></span>|<span data-ttu-id="a3b73-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="a3b73-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3b73-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="a3b73-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="a3b73-130">メールボックス ユーザーについて、期間の作業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3b73-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="a3b73-131">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a3b73-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3b73-132">備考</span><span class="sxs-lookup"><span data-stu-id="a3b73-132">Remarks</span></span>

<span data-ttu-id="a3b73-133">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a3b73-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="a3b73-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a3b73-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3b73-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="a3b73-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3b73-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="a3b73-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3b73-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3b73-137">Schema Name</span></span>  <br/> |<span data-ttu-id="a3b73-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a3b73-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3b73-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3b73-139">Validation File</span></span>  <br/> |<span data-ttu-id="a3b73-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3b73-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3b73-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a3b73-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3b73-142">False</span><span class="sxs-lookup"><span data-stu-id="a3b73-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3b73-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="a3b73-143">See also</span></span>



[<span data-ttu-id="a3b73-144">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="a3b73-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a3b73-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3b73-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a3b73-146">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3b73-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

