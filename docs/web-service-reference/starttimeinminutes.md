---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: StartTimeInMinutes 要素は、メールボックスがユーザーの稼働日の開始を表します。
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833558"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="79bb1-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="79bb1-103">StartTimeInMinutes</span></span>

<span data-ttu-id="79bb1-104">**StartTimeInMinutes**要素は、メールボックスがユーザーの稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="79bb1-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="79bb1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="79bb1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="79bb1-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="79bb1-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="79bb1-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="79bb1-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="79bb1-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="79bb1-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="79bb1-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="79bb1-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="79bb1-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="79bb1-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="79bb1-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="79bb1-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="79bb1-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="79bb1-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="79bb1-113">**int**</span><span class="sxs-lookup"><span data-stu-id="79bb1-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="79bb1-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="79bb1-114">Attributes and elements</span></span>

<span data-ttu-id="79bb1-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79bb1-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79bb1-116">属性</span><span class="sxs-lookup"><span data-stu-id="79bb1-116">Attributes</span></span>

<span data-ttu-id="79bb1-117">なし。</span><span class="sxs-lookup"><span data-stu-id="79bb1-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79bb1-118">子要素</span><span class="sxs-lookup"><span data-stu-id="79bb1-118">Child elements</span></span>

<span data-ttu-id="79bb1-119">なし。</span><span class="sxs-lookup"><span data-stu-id="79bb1-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79bb1-120">親要素</span><span class="sxs-lookup"><span data-stu-id="79bb1-120">Parent elements</span></span>

|<span data-ttu-id="79bb1-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="79bb1-121">**Element**</span></span>|<span data-ttu-id="79bb1-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="79bb1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79bb1-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="79bb1-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="79bb1-124">日、およびメールボックス ユーザーの時間は、稼働日に含まれています。</span><span class="sxs-lookup"><span data-stu-id="79bb1-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="79bb1-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="79bb1-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79bb1-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="79bb1-126">Text value</span></span>

<span data-ttu-id="79bb1-127">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="79bb1-127">A text value is required.</span></span> <span data-ttu-id="79bb1-128">テキスト値は、1 日の開始後何分が経過した、稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="79bb1-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="79bb1-129">たとえば、午前 8 時の開始時刻</span><span class="sxs-lookup"><span data-stu-id="79bb1-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="79bb1-130">480 分で表されます。</span><span class="sxs-lookup"><span data-stu-id="79bb1-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="79bb1-131">この要素に指定できる値の範囲は、0 から 1440 です。</span><span class="sxs-lookup"><span data-stu-id="79bb1-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79bb1-132">備考</span><span class="sxs-lookup"><span data-stu-id="79bb1-132">Remarks</span></span>

<span data-ttu-id="79bb1-133">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="79bb1-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79bb1-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="79bb1-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79bb1-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="79bb1-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79bb1-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79bb1-136">Schema Name</span></span>  <br/> |<span data-ttu-id="79bb1-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="79bb1-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="79bb1-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79bb1-138">Validation File</span></span>  <br/> |<span data-ttu-id="79bb1-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79bb1-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79bb1-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="79bb1-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="79bb1-141">False</span><span class="sxs-lookup"><span data-stu-id="79bb1-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79bb1-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="79bb1-142">See also</span></span>

- [<span data-ttu-id="79bb1-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="79bb1-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="79bb1-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="79bb1-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="79bb1-145">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="79bb1-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

