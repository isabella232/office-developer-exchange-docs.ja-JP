---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: WorkingPeriodArray 要素には、メールボックスユーザーの勤務期間情報が含まれています。
ms.openlocfilehash: a9ca55866a574c5208d8561fca6daf417867fef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465199"
---
# <a name="workingperiodarray"></a><span data-ttu-id="fd27e-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="fd27e-103">WorkingPeriodArray</span></span>

<span data-ttu-id="fd27e-104">**WorkingPeriodArray**要素には、メールボックスユーザーの勤務期間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fd27e-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="fd27e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fd27e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fd27e-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="fd27e-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="fd27e-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="fd27e-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="fd27e-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="fd27e-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="fd27e-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="fd27e-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="fd27e-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="fd27e-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="fd27e-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="fd27e-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd27e-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fd27e-112">Attributes and elements</span></span>

<span data-ttu-id="fd27e-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd27e-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd27e-114">属性</span><span class="sxs-lookup"><span data-stu-id="fd27e-114">Attributes</span></span>

<span data-ttu-id="fd27e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="fd27e-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd27e-116">子要素</span><span class="sxs-lookup"><span data-stu-id="fd27e-116">Child elements</span></span>

|<span data-ttu-id="fd27e-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="fd27e-117">**Element**</span></span>|<span data-ttu-id="fd27e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd27e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd27e-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="fd27e-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="fd27e-120">メールボックスユーザーの勤務週の曜日と時間を含みます。</span><span class="sxs-lookup"><span data-stu-id="fd27e-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd27e-121">親要素</span><span class="sxs-lookup"><span data-stu-id="fd27e-121">Parent elements</span></span>

|<span data-ttu-id="fd27e-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="fd27e-122">**Element**</span></span>|<span data-ttu-id="fd27e-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="fd27e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd27e-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="fd27e-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fd27e-125">要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。</span><span class="sxs-lookup"><span data-stu-id="fd27e-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="fd27e-126">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd27e-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd27e-127">注釈</span><span class="sxs-lookup"><span data-stu-id="fd27e-127">Remarks</span></span>

<span data-ttu-id="fd27e-128">この要素は、 [WorkingHours](workinghours-ex15websvcsotherref.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="fd27e-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="fd27e-129">すべての子要素が発生する順序で一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="fd27e-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="fd27e-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fd27e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd27e-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fd27e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd27e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd27e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd27e-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fd27e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fd27e-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fd27e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd27e-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fd27e-135">Validation File</span></span>  <br/> |<span data-ttu-id="fd27e-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fd27e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd27e-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fd27e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd27e-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="fd27e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd27e-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="fd27e-139">See also</span></span>



[<span data-ttu-id="fd27e-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="fd27e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fd27e-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fd27e-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fd27e-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="fd27e-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

