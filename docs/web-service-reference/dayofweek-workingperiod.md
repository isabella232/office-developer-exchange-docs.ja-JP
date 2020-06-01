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
description: DayOfWeek 要素には、メールボックスユーザーに対してスケジュールされた稼働日の一覧が含まれています。
ms.openlocfilehash: 06d4a7d5541b3b71fcbf9be9beb7512d06853283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457446"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="b8131-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="b8131-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="b8131-104">**DayOfWeek**要素には、メールボックスユーザーに対してスケジュールされた稼働日の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b8131-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="b8131-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b8131-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="b8131-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b8131-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="b8131-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b8131-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="b8131-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b8131-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="b8131-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="b8131-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="b8131-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="b8131-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="b8131-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="b8131-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="b8131-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="b8131-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="b8131-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b8131-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b8131-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b8131-114">Attributes and elements</span></span>

<span data-ttu-id="b8131-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8131-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8131-116">属性</span><span class="sxs-lookup"><span data-stu-id="b8131-116">Attributes</span></span>

<span data-ttu-id="b8131-117">なし。</span><span class="sxs-lookup"><span data-stu-id="b8131-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8131-118">子要素</span><span class="sxs-lookup"><span data-stu-id="b8131-118">Child elements</span></span>

<span data-ttu-id="b8131-119">なし。</span><span class="sxs-lookup"><span data-stu-id="b8131-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8131-120">親要素</span><span class="sxs-lookup"><span data-stu-id="b8131-120">Parent elements</span></span>

|<span data-ttu-id="b8131-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8131-121">**Element**</span></span>|<span data-ttu-id="b8131-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8131-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8131-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="b8131-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="b8131-124">メールボックスユーザーの勤務週の曜日と時間を含みます。</span><span class="sxs-lookup"><span data-stu-id="b8131-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="b8131-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8131-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8131-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b8131-126">Text value</span></span>

<span data-ttu-id="b8131-127">メールボックスユーザーが稼働日を表すように日付を設定している場合は、テキスト値が返されます。</span><span class="sxs-lookup"><span data-stu-id="b8131-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="b8131-128">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b8131-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="b8131-129">日曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-129">Sunday</span></span>    
- <span data-ttu-id="b8131-130">月曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-130">Monday</span></span>    
- <span data-ttu-id="b8131-131">火曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-131">Tuesday</span></span>    
- <span data-ttu-id="b8131-132">水曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-132">Wednesday</span></span>    
- <span data-ttu-id="b8131-133">木曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-133">Thursday</span></span>    
- <span data-ttu-id="b8131-134">金曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-134">Friday</span></span>    
- <span data-ttu-id="b8131-135">土曜日</span><span class="sxs-lookup"><span data-stu-id="b8131-135">Saturday</span></span> 
    
<span data-ttu-id="b8131-136">この順序でテキスト値が返されます。</span><span class="sxs-lookup"><span data-stu-id="b8131-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8131-137">注釈</span><span class="sxs-lookup"><span data-stu-id="b8131-137">Remarks</span></span>

<span data-ttu-id="b8131-138">この要素と Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md)要素の違いは、型である点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="b8131-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="b8131-139">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b8131-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8131-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b8131-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8131-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8131-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8131-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8131-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b8131-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b8131-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8131-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8131-144">Validation File</span></span>  <br/> |<span data-ttu-id="b8131-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b8131-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8131-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b8131-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8131-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="b8131-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8131-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8131-148">See also</span></span>

- [<span data-ttu-id="b8131-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="b8131-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="b8131-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b8131-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="b8131-151">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="b8131-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

