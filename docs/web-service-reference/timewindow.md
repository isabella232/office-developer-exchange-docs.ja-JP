---
title: 時間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: 時間要素は、ユーザーの利用可能時間情報を照会する期間を指定します。
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839701"
---
# <a name="timewindow"></a><span data-ttu-id="57087-103">時間</span><span class="sxs-lookup"><span data-stu-id="57087-103">TimeWindow</span></span>

<span data-ttu-id="57087-104">**時間**要素は、ユーザーの利用可能時間情報を照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="57087-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="57087-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="57087-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="57087-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="57087-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="57087-107">時間</span><span class="sxs-lookup"><span data-stu-id="57087-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="57087-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="57087-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57087-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57087-109">Attributes and elements</span></span>

<span data-ttu-id="57087-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57087-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57087-111">属性</span><span class="sxs-lookup"><span data-stu-id="57087-111">Attributes</span></span>

<span data-ttu-id="57087-112">なし。</span><span class="sxs-lookup"><span data-stu-id="57087-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57087-113">子要素</span><span class="sxs-lookup"><span data-stu-id="57087-113">Child elements</span></span>

|<span data-ttu-id="57087-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="57087-114">**Element**</span></span>|<span data-ttu-id="57087-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="57087-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57087-116">開始時刻</span><span class="sxs-lookup"><span data-stu-id="57087-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="57087-117">ユーザーの可用性について照会する期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="57087-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="57087-118">終了時刻</span><span class="sxs-lookup"><span data-stu-id="57087-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="57087-119">ユーザーの可用性について照会する期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="57087-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57087-120">親要素</span><span class="sxs-lookup"><span data-stu-id="57087-120">Parent elements</span></span>

|<span data-ttu-id="57087-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="57087-121">**Element**</span></span>|<span data-ttu-id="57087-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="57087-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57087-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="57087-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="57087-124">応答で返される空き時間情報の情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="57087-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="57087-125">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="57087-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57087-126">備考</span><span class="sxs-lookup"><span data-stu-id="57087-126">Remarks</span></span>

<span data-ttu-id="57087-127">この期間の最大値は、42 日です。</span><span class="sxs-lookup"><span data-stu-id="57087-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="57087-128">この最大値を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="57087-128">This maximum value can be modified.</span></span> <span data-ttu-id="57087-129">最大値を超えたユーザーの利用可能時間情報の要求はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="57087-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="57087-130">予定は[開始時刻](starttime.md)と[終了時刻](endtime.md)の要素で定義された期間の一部が、完全にその予定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="57087-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="57087-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft® Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="57087-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="57087-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="57087-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57087-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="57087-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57087-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57087-134">Schema Name</span></span>  <br/> |<span data-ttu-id="57087-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="57087-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="57087-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57087-136">Validation File</span></span>  <br/> |<span data-ttu-id="57087-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57087-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57087-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57087-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="57087-139">False</span><span class="sxs-lookup"><span data-stu-id="57087-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57087-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="57087-140">See also</span></span>



[<span data-ttu-id="57087-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="57087-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="57087-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="57087-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

