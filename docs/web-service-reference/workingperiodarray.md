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
description: WorkingPeriodArray 要素には、メールボックス ユーザーの期間の情報を作業が含まれています。
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840043"
---
# <a name="workingperiodarray"></a><span data-ttu-id="d89b7-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d89b7-103">WorkingPeriodArray</span></span>

<span data-ttu-id="d89b7-104">**WorkingPeriodArray**要素には、メールボックス ユーザーの期間の情報を作業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d89b7-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="d89b7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d89b7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d89b7-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d89b7-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d89b7-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d89b7-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d89b7-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d89b7-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d89b7-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d89b7-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="d89b7-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d89b7-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="d89b7-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="d89b7-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d89b7-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d89b7-112">Attributes and elements</span></span>

<span data-ttu-id="d89b7-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89b7-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d89b7-114">属性</span><span class="sxs-lookup"><span data-stu-id="d89b7-114">Attributes</span></span>

<span data-ttu-id="d89b7-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d89b7-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d89b7-116">子要素</span><span class="sxs-lookup"><span data-stu-id="d89b7-116">Child elements</span></span>

|<span data-ttu-id="d89b7-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d89b7-117">**Element**</span></span>|<span data-ttu-id="d89b7-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89b7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89b7-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="d89b7-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="d89b7-120">日、およびメールボックス ユーザーの時間は、稼働日に含まれています。</span><span class="sxs-lookup"><span data-stu-id="d89b7-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d89b7-121">親要素</span><span class="sxs-lookup"><span data-stu-id="d89b7-121">Parent elements</span></span>

|<span data-ttu-id="d89b7-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="d89b7-122">**Element**</span></span>|<span data-ttu-id="d89b7-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89b7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89b7-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d89b7-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d89b7-125">要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="d89b7-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="d89b7-126">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d89b7-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d89b7-127">備考</span><span class="sxs-lookup"><span data-stu-id="d89b7-127">Remarks</span></span>

<span data-ttu-id="d89b7-128">[WorkingHours](workinghours-ex15websvcsotherref.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="d89b7-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="d89b7-129">発生したシーケンスは、すべての子要素の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d89b7-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="d89b7-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d89b7-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d89b7-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="d89b7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d89b7-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="d89b7-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d89b7-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d89b7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d89b7-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d89b7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d89b7-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d89b7-135">Validation File</span></span>  <br/> |<span data-ttu-id="d89b7-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d89b7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d89b7-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d89b7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d89b7-138">False</span><span class="sxs-lookup"><span data-stu-id="d89b7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d89b7-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="d89b7-139">See also</span></span>



[<span data-ttu-id="d89b7-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d89b7-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d89b7-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d89b7-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d89b7-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="d89b7-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

