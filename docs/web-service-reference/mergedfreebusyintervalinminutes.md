---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: MergedFreeBusyIntervalInMinutes 要素は、FreeBusyMerged のビューで連続する 2 つのスロット間の時間差を表します。
ms.openlocfilehash: 99c8c69424a0a9d9594005fdf6b2ceba53e6288a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832451"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="9c180-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="9c180-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="9c180-104">**MergedFreeBusyIntervalInMinutes**要素は、 **FreeBusyMerged**のビューで連続する 2 つのスロット間の時間差を表します。</span><span class="sxs-lookup"><span data-stu-id="9c180-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="9c180-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="9c180-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="9c180-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="9c180-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="9c180-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="9c180-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="9c180-108">**int**</span><span class="sxs-lookup"><span data-stu-id="9c180-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c180-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9c180-109">Attributes and elements</span></span>

<span data-ttu-id="9c180-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c180-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c180-111">属性</span><span class="sxs-lookup"><span data-stu-id="9c180-111">Attributes</span></span>

<span data-ttu-id="9c180-112">なし。</span><span class="sxs-lookup"><span data-stu-id="9c180-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c180-113">子要素</span><span class="sxs-lookup"><span data-stu-id="9c180-113">Child elements</span></span>

<span data-ttu-id="9c180-114">なし。</span><span class="sxs-lookup"><span data-stu-id="9c180-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c180-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9c180-115">Parent elements</span></span>

|<span data-ttu-id="9c180-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c180-116">**Element**</span></span>|<span data-ttu-id="9c180-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c180-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c180-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="9c180-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="9c180-119">応答で返される空き時間情報の情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c180-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="9c180-120">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="9c180-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c180-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9c180-121">Text value</span></span>

<span data-ttu-id="9c180-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="9c180-122">A text value is required.</span></span> <span data-ttu-id="9c180-123">テキスト値は、分単位の時間を表します。</span><span class="sxs-lookup"><span data-stu-id="9c180-123">The text value represents time in minutes.</span></span> <span data-ttu-id="9c180-124">既定値は、30 分です。</span><span class="sxs-lookup"><span data-stu-id="9c180-124">The default value is 30 minutes.</span></span> <span data-ttu-id="9c180-125">6 分間隔の最小値は、1 日 (1440 分) この要素の最大間隔。</span><span class="sxs-lookup"><span data-stu-id="9c180-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9c180-126">備考</span><span class="sxs-lookup"><span data-stu-id="9c180-126">Remarks</span></span>

<span data-ttu-id="9c180-127">[RequestedView](requestedview.md)要素は、 **MergedOnly**、 **FreeBusyMerged**、または**DetailedMerge**に等しい場合にのみ、この値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="9c180-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="9c180-128">これは、整数データ型です。</span><span class="sxs-lookup"><span data-stu-id="9c180-128">This is an integer data type.</span></span> <span data-ttu-id="9c180-129">[MergedFreeBusy](mergedfreebusy.md)要素では、この要素で定義された間隔を格納しているストリームが返されます。</span><span class="sxs-lookup"><span data-stu-id="9c180-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9c180-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="9c180-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c180-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="9c180-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c180-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c180-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9c180-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9c180-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c180-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c180-134">Validation File</span></span>  <br/> |<span data-ttu-id="9c180-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c180-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c180-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9c180-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c180-137">False</span><span class="sxs-lookup"><span data-stu-id="9c180-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c180-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c180-138">See also</span></span>



[<span data-ttu-id="9c180-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="9c180-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="9c180-140">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="9c180-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="9c180-141">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="9c180-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

