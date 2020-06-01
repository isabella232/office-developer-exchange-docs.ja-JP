---
title: TimeWindow
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
description: TimeWindow 要素は、ユーザーの空き時間情報を照会した期間を識別します。
ms.openlocfilehash: 5c66614520f9d616687d67ad609b3d55d9cf6571
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458930"
---
# <a name="timewindow"></a><span data-ttu-id="21635-103">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="21635-103">TimeWindow</span></span>

<span data-ttu-id="21635-104">**TimeWindow**要素は、ユーザーの空き時間情報を照会した期間を識別します。</span><span class="sxs-lookup"><span data-stu-id="21635-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="21635-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="21635-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="21635-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="21635-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="21635-107">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="21635-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="21635-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="21635-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21635-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21635-109">Attributes and elements</span></span>

<span data-ttu-id="21635-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21635-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21635-111">属性</span><span class="sxs-lookup"><span data-stu-id="21635-111">Attributes</span></span>

<span data-ttu-id="21635-112">なし。</span><span class="sxs-lookup"><span data-stu-id="21635-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21635-113">子要素</span><span class="sxs-lookup"><span data-stu-id="21635-113">Child elements</span></span>

|<span data-ttu-id="21635-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="21635-114">**Element**</span></span>|<span data-ttu-id="21635-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="21635-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21635-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="21635-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="21635-117">ユーザーの空き時間情報を照会した期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="21635-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="21635-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="21635-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="21635-119">ユーザーの空き時間情報を照会した期間の終わりを表します。</span><span class="sxs-lookup"><span data-stu-id="21635-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21635-120">親要素</span><span class="sxs-lookup"><span data-stu-id="21635-120">Parent elements</span></span>

|<span data-ttu-id="21635-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="21635-121">**Element**</span></span>|<span data-ttu-id="21635-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="21635-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21635-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="21635-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="21635-124">応答で返される空き時間情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="21635-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="21635-125">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21635-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21635-126">注釈</span><span class="sxs-lookup"><span data-stu-id="21635-126">Remarks</span></span>

<span data-ttu-id="21635-127">この期間の最大値は42日です。</span><span class="sxs-lookup"><span data-stu-id="21635-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="21635-128">この最大値は変更できます。</span><span class="sxs-lookup"><span data-stu-id="21635-128">This maximum value can be modified.</span></span> <span data-ttu-id="21635-129">最大値を超えるユーザーの空き時間情報を要求すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="21635-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="21635-130">[StartTime](starttime.md)要素と[EndTime](endtime.md)要素で定義されている時間帯に、予定が部分的に含まれている場合、その予定は全体に含まれます。</span><span class="sxs-lookup"><span data-stu-id="21635-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="21635-131">この要素を記述するスキーマは、Microsoft® Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="21635-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="21635-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21635-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21635-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="21635-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21635-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21635-134">Schema Name</span></span>  <br/> |<span data-ttu-id="21635-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="21635-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="21635-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21635-136">Validation File</span></span>  <br/> |<span data-ttu-id="21635-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="21635-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21635-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21635-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="21635-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="21635-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21635-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="21635-140">See also</span></span>



[<span data-ttu-id="21635-141">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="21635-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="21635-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="21635-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

