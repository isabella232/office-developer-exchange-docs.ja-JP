---
title: EndTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeInMinutes
api_type:
- schema
ms.assetid: ef05bdda-7a66-44db-bb73-a2ce8316c257
description: EndTimeInMinutes 要素は、メールボックスユーザーの稼働日の終了を表します。
ms.openlocfilehash: cb564f9de944848734749a30c813a94d6b5c4187
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459652"
---
# <a name="endtimeinminutes"></a><span data-ttu-id="1d130-103">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d130-103">EndTimeInMinutes</span></span>

<span data-ttu-id="1d130-104">**EndTimeInMinutes**要素は、メールボックスユーザーの稼働日の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="1d130-104">The **EndTimeInMinutes** element represents the end of the working day for a mailbox user.</span></span> 
  
[<span data-ttu-id="1d130-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d130-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1d130-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1d130-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1d130-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1d130-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1d130-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1d130-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1d130-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="1d130-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="1d130-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="1d130-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="1d130-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="1d130-111">WorkingPeriod</span></span>](workingperiod.md)
  
[<span data-ttu-id="1d130-112">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d130-112">EndTimeInMinutes</span></span>](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 <span data-ttu-id="1d130-113">**int**</span><span class="sxs-lookup"><span data-stu-id="1d130-113">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d130-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1d130-114">Attributes and elements</span></span>

<span data-ttu-id="1d130-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d130-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d130-116">属性</span><span class="sxs-lookup"><span data-stu-id="1d130-116">Attributes</span></span>

<span data-ttu-id="1d130-117">なし。</span><span class="sxs-lookup"><span data-stu-id="1d130-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d130-118">子要素</span><span class="sxs-lookup"><span data-stu-id="1d130-118">Child elements</span></span>

<span data-ttu-id="1d130-119">なし。</span><span class="sxs-lookup"><span data-stu-id="1d130-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d130-120">親要素</span><span class="sxs-lookup"><span data-stu-id="1d130-120">Parent elements</span></span>

|<span data-ttu-id="1d130-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d130-121">**Element**</span></span>|<span data-ttu-id="1d130-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d130-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d130-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="1d130-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="1d130-124">メールボックスユーザーの勤務週の曜日と時間を含みます。</span><span class="sxs-lookup"><span data-stu-id="1d130-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="1d130-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d130-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d130-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1d130-126">Text value</span></span>

<span data-ttu-id="1d130-127">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1d130-127">A text value is required.</span></span> <span data-ttu-id="1d130-128">テキスト値は、1日から開始されてから経過した時間数で、稼働日の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="1d130-128">The text value represents the end of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="1d130-129">たとえば、午後6時の終了時刻</span><span class="sxs-lookup"><span data-stu-id="1d130-129">For example, an end time of 6 P.M.</span></span> <span data-ttu-id="1d130-130">は1080分で表されます。</span><span class="sxs-lookup"><span data-stu-id="1d130-130">is represented by 1080 minutes.</span></span>
  
<span data-ttu-id="1d130-131">この要素で使用できる値の範囲は 0 ~ 1440 です。</span><span class="sxs-lookup"><span data-stu-id="1d130-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d130-132">注釈</span><span class="sxs-lookup"><span data-stu-id="1d130-132">Remarks</span></span>

<span data-ttu-id="1d130-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1d130-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d130-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1d130-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d130-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d130-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d130-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d130-136">Schema Name</span></span>  <br/> |<span data-ttu-id="1d130-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1d130-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d130-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d130-138">Validation File</span></span>  <br/> |<span data-ttu-id="1d130-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1d130-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d130-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d130-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d130-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="1d130-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d130-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d130-142">See also</span></span>



[<span data-ttu-id="1d130-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1d130-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1d130-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1d130-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1d130-145">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="1d130-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

