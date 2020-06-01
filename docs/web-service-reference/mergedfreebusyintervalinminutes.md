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
description: MergedFreeBusyIntervalInMinutes 要素は、FreeBusyMerged ビューの2つの連続するスロット間の時間差を表します。
ms.openlocfilehash: 6228ee5b66202634e6bb3b6c1ad6b8897a109d58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468790"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="dddaf-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="dddaf-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="dddaf-104">**MergedFreeBusyIntervalInMinutes**要素は、 **FreeBusyMerged**ビューの2つの連続するスロット間の時間差を表します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="dddaf-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="dddaf-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="dddaf-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="dddaf-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="dddaf-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="dddaf-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="dddaf-108">**int**</span><span class="sxs-lookup"><span data-stu-id="dddaf-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dddaf-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dddaf-109">Attributes and elements</span></span>

<span data-ttu-id="dddaf-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dddaf-111">属性</span><span class="sxs-lookup"><span data-stu-id="dddaf-111">Attributes</span></span>

<span data-ttu-id="dddaf-112">なし。</span><span class="sxs-lookup"><span data-stu-id="dddaf-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dddaf-113">子要素</span><span class="sxs-lookup"><span data-stu-id="dddaf-113">Child elements</span></span>

<span data-ttu-id="dddaf-114">なし。</span><span class="sxs-lookup"><span data-stu-id="dddaf-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dddaf-115">親要素</span><span class="sxs-lookup"><span data-stu-id="dddaf-115">Parent elements</span></span>

|<span data-ttu-id="dddaf-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="dddaf-116">**Element**</span></span>|<span data-ttu-id="dddaf-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="dddaf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dddaf-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="dddaf-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="dddaf-119">応答で返される空き時間情報の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="dddaf-120">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dddaf-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dddaf-121">Text value</span></span>

<span data-ttu-id="dddaf-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="dddaf-122">A text value is required.</span></span> <span data-ttu-id="dddaf-123">テキスト値は、時間を分単位で表します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-123">The text value represents time in minutes.</span></span> <span data-ttu-id="dddaf-124">既定値は 30 分です。</span><span class="sxs-lookup"><span data-stu-id="dddaf-124">The default value is 30 minutes.</span></span> <span data-ttu-id="dddaf-125">この要素の最大間隔は、6分で、最小間隔と1日 (1440 分) で指定します。</span><span class="sxs-lookup"><span data-stu-id="dddaf-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dddaf-126">注釈</span><span class="sxs-lookup"><span data-stu-id="dddaf-126">Remarks</span></span>

<span data-ttu-id="dddaf-127">この値は、 [Requestedview](requestedview.md)要素が**MergedOnly**、 **FreeBusyMerged**、または**DetailedMerge**と等しい場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="dddaf-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="dddaf-128">これは integer データ型です。</span><span class="sxs-lookup"><span data-stu-id="dddaf-128">This is an integer data type.</span></span> <span data-ttu-id="dddaf-129">この要素で定義されている間隔を含むストリームは、 [MergedFreeBusy](mergedfreebusy.md)要素で返されます。</span><span class="sxs-lookup"><span data-stu-id="dddaf-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="dddaf-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dddaf-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dddaf-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="dddaf-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dddaf-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dddaf-132">Schema Name</span></span>  <br/> |<span data-ttu-id="dddaf-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dddaf-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="dddaf-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dddaf-134">Validation File</span></span>  <br/> |<span data-ttu-id="dddaf-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dddaf-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dddaf-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dddaf-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="dddaf-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="dddaf-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dddaf-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="dddaf-138">See also</span></span>



[<span data-ttu-id="dddaf-139">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="dddaf-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="dddaf-140">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="dddaf-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="dddaf-141">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="dddaf-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

