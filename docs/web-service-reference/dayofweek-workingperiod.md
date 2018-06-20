---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: DayOfWeek の要素には、メールボックス ユーザーのスケジュールの稼働日のリストが含まれています。
ms.openlocfilehash: a6a68017291ba13f45b3970307669222d583fcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759942"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="970b8-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="970b8-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="970b8-104">**DayOfWeek**の要素には、メールボックス ユーザーのスケジュールの稼働日のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="970b8-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="970b8-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="970b8-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="970b8-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="970b8-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="970b8-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="970b8-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="970b8-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="970b8-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="970b8-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="970b8-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="970b8-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="970b8-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="970b8-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="970b8-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="970b8-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="970b8-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="970b8-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="970b8-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="970b8-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="970b8-114">Attributes and elements</span></span>

<span data-ttu-id="970b8-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="970b8-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="970b8-116">属性</span><span class="sxs-lookup"><span data-stu-id="970b8-116">Attributes</span></span>

<span data-ttu-id="970b8-117">なし。</span><span class="sxs-lookup"><span data-stu-id="970b8-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="970b8-118">子要素</span><span class="sxs-lookup"><span data-stu-id="970b8-118">Child elements</span></span>

<span data-ttu-id="970b8-119">なし。</span><span class="sxs-lookup"><span data-stu-id="970b8-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="970b8-120">親要素</span><span class="sxs-lookup"><span data-stu-id="970b8-120">Parent elements</span></span>

|<span data-ttu-id="970b8-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="970b8-121">**Element**</span></span>|<span data-ttu-id="970b8-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="970b8-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="970b8-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="970b8-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="970b8-124">日、およびメールボックス ユーザーの時間は、稼働日に含まれています。</span><span class="sxs-lookup"><span data-stu-id="970b8-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="970b8-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="970b8-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="970b8-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="970b8-126">Text value</span></span>

<span data-ttu-id="970b8-127">メールボックスのユーザーに稼働日を表す設定日が設定されている場合は、テキスト値が返されます。</span><span class="sxs-lookup"><span data-stu-id="970b8-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="970b8-128">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="970b8-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="970b8-129">日曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-129">Sunday</span></span>    
- <span data-ttu-id="970b8-130">月曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-130">Monday</span></span>    
- <span data-ttu-id="970b8-131">火曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-131">Tuesday</span></span>    
- <span data-ttu-id="970b8-132">水曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-132">Wednesday</span></span>    
- <span data-ttu-id="970b8-133">木曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-133">Thursday</span></span>    
- <span data-ttu-id="970b8-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-134">Friday</span></span>    
- <span data-ttu-id="970b8-135">土曜日</span><span class="sxs-lookup"><span data-stu-id="970b8-135">Saturday</span></span> 
    
<span data-ttu-id="970b8-136">テキスト値は、その順序で返されます。</span><span class="sxs-lookup"><span data-stu-id="970b8-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="970b8-137">備考</span><span class="sxs-lookup"><span data-stu-id="970b8-137">Remarks</span></span>

<span data-ttu-id="970b8-138">この要素と、可用性の[曜日 (タイムゾーン)](dayofweek-timezone.md)の違いが型であることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="970b8-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="970b8-139">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="970b8-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="970b8-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="970b8-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="970b8-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="970b8-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="970b8-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="970b8-142">Schema Name</span></span>  <br/> |<span data-ttu-id="970b8-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="970b8-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="970b8-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="970b8-144">Validation File</span></span>  <br/> |<span data-ttu-id="970b8-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="970b8-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="970b8-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="970b8-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="970b8-147">False</span><span class="sxs-lookup"><span data-stu-id="970b8-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="970b8-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="970b8-148">See also</span></span>

- [<span data-ttu-id="970b8-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="970b8-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="970b8-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="970b8-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="970b8-151">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="970b8-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

