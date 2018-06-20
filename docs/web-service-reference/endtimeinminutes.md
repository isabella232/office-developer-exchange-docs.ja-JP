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
description: EndTimeInMinutes 要素は、メールボックスがユーザーの稼働日の終了を表します。
ms.openlocfilehash: 2885d810512eb0e575aa25b4f38d28332a10b8f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760314"
---
# <a name="endtimeinminutes"></a><span data-ttu-id="c2871-103">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c2871-103">EndTimeInMinutes</span></span>

<span data-ttu-id="c2871-104">**EndTimeInMinutes**要素は、メールボックスがユーザーの稼働日の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="c2871-104">The **EndTimeInMinutes** element represents the end of the working day for a mailbox user.</span></span> 
  
[<span data-ttu-id="c2871-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c2871-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c2871-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="c2871-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="c2871-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="c2871-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="c2871-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="c2871-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="c2871-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="c2871-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="c2871-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="c2871-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="c2871-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="c2871-111">WorkingPeriod</span></span>](workingperiod.md)
  
[<span data-ttu-id="c2871-112">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c2871-112">EndTimeInMinutes</span></span>](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 <span data-ttu-id="c2871-113">**int**</span><span class="sxs-lookup"><span data-stu-id="c2871-113">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2871-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c2871-114">Attributes and elements</span></span>

<span data-ttu-id="c2871-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2871-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2871-116">属性</span><span class="sxs-lookup"><span data-stu-id="c2871-116">Attributes</span></span>

<span data-ttu-id="c2871-117">なし。</span><span class="sxs-lookup"><span data-stu-id="c2871-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2871-118">子要素</span><span class="sxs-lookup"><span data-stu-id="c2871-118">Child elements</span></span>

<span data-ttu-id="c2871-119">なし。</span><span class="sxs-lookup"><span data-stu-id="c2871-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2871-120">親要素</span><span class="sxs-lookup"><span data-stu-id="c2871-120">Parent elements</span></span>

|<span data-ttu-id="c2871-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2871-121">**Element**</span></span>|<span data-ttu-id="c2871-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2871-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2871-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="c2871-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="c2871-124">日、およびメールボックス ユーザーの時間は、稼働日に含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2871-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="c2871-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c2871-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2871-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c2871-126">Text value</span></span>

<span data-ttu-id="c2871-127">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="c2871-127">A text value is required.</span></span> <span data-ttu-id="c2871-128">テキスト値は、1 日の開始後何分が経過した、稼働日の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="c2871-128">The text value represents the end of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="c2871-129">たとえば、午後 6 時の終了時刻</span><span class="sxs-lookup"><span data-stu-id="c2871-129">For example, an end time of 6 P.M.</span></span> <span data-ttu-id="c2871-130">1080 分で表されます。</span><span class="sxs-lookup"><span data-stu-id="c2871-130">is represented by 1080 minutes.</span></span>
  
<span data-ttu-id="c2871-131">この要素に指定できる値の範囲は、0 から 1440 です。</span><span class="sxs-lookup"><span data-stu-id="c2871-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2871-132">備考</span><span class="sxs-lookup"><span data-stu-id="c2871-132">Remarks</span></span>

<span data-ttu-id="c2871-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c2871-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2871-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="c2871-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2871-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="c2871-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2871-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2871-136">Schema Name</span></span>  <br/> |<span data-ttu-id="c2871-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c2871-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2871-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2871-138">Validation File</span></span>  <br/> |<span data-ttu-id="c2871-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2871-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2871-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2871-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2871-141">False</span><span class="sxs-lookup"><span data-stu-id="c2871-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2871-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2871-142">See also</span></span>



[<span data-ttu-id="c2871-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="c2871-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c2871-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c2871-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c2871-145">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="c2871-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

