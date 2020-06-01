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
description: StartTimeInMinutes 要素は、メールボックスユーザーの稼働日の開始を表します。
ms.openlocfilehash: b33cb12299a146b577dd17939a0585a15d50fb07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458531"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="edf70-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="edf70-103">StartTimeInMinutes</span></span>

<span data-ttu-id="edf70-104">**StartTimeInMinutes**要素は、メールボックスユーザーの稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="edf70-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="edf70-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="edf70-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="edf70-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="edf70-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="edf70-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="edf70-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="edf70-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="edf70-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="edf70-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="edf70-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="edf70-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="edf70-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="edf70-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="edf70-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="edf70-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="edf70-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="edf70-113">**int**</span><span class="sxs-lookup"><span data-stu-id="edf70-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="edf70-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="edf70-114">Attributes and elements</span></span>

<span data-ttu-id="edf70-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="edf70-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edf70-116">属性</span><span class="sxs-lookup"><span data-stu-id="edf70-116">Attributes</span></span>

<span data-ttu-id="edf70-117">なし。</span><span class="sxs-lookup"><span data-stu-id="edf70-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edf70-118">子要素</span><span class="sxs-lookup"><span data-stu-id="edf70-118">Child elements</span></span>

<span data-ttu-id="edf70-119">なし。</span><span class="sxs-lookup"><span data-stu-id="edf70-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="edf70-120">親要素</span><span class="sxs-lookup"><span data-stu-id="edf70-120">Parent elements</span></span>

|<span data-ttu-id="edf70-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="edf70-121">**Element**</span></span>|<span data-ttu-id="edf70-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="edf70-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edf70-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="edf70-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="edf70-124">メールボックスユーザーの勤務週の曜日と時間を含みます。</span><span class="sxs-lookup"><span data-stu-id="edf70-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="edf70-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="edf70-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="edf70-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="edf70-126">Text value</span></span>

<span data-ttu-id="edf70-127">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="edf70-127">A text value is required.</span></span> <span data-ttu-id="edf70-128">テキスト値は、1日から開始してからの経過時間 (分単位) による稼働日の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="edf70-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="edf70-129">たとえば、開始時刻の午前8時</span><span class="sxs-lookup"><span data-stu-id="edf70-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="edf70-130">は480分で表されます。</span><span class="sxs-lookup"><span data-stu-id="edf70-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="edf70-131">この要素で使用できる値の範囲は 0 ~ 1440 です。</span><span class="sxs-lookup"><span data-stu-id="edf70-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="edf70-132">注釈</span><span class="sxs-lookup"><span data-stu-id="edf70-132">Remarks</span></span>

<span data-ttu-id="edf70-133">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="edf70-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edf70-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="edf70-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edf70-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="edf70-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="edf70-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="edf70-136">Schema Name</span></span>  <br/> |<span data-ttu-id="edf70-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="edf70-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="edf70-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="edf70-138">Validation File</span></span>  <br/> |<span data-ttu-id="edf70-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="edf70-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="edf70-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="edf70-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="edf70-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="edf70-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edf70-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="edf70-142">See also</span></span>

- [<span data-ttu-id="edf70-143">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="edf70-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="edf70-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="edf70-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="edf70-145">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="edf70-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

