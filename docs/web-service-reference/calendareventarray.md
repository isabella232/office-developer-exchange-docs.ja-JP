---
title: CalendarEventArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventArray
api_type:
- schema
ms.assetid: a00f7f56-d7f1-429d-ae02-97043718c864
description: CalendarEventArray 要素には、要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。
ms.openlocfilehash: 2e56b7b2b94e12401ba708dfca94101064d625e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759580"
---
# <a name="calendareventarray"></a><span data-ttu-id="cd4b1-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="cd4b1-103">CalendarEventArray</span></span>

<span data-ttu-id="cd4b1-104">**CalendarEventArray**要素には、要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="cd4b1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd4b1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cd4b1-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cd4b1-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="cd4b1-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="cd4b1-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="cd4b1-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="cd4b1-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="cd4b1-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="cd4b1-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="cd4b1-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="cd4b1-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd4b1-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cd4b1-111">Attributes and elements</span></span>

<span data-ttu-id="cd4b1-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd4b1-113">属性</span><span class="sxs-lookup"><span data-stu-id="cd4b1-113">Attributes</span></span>

<span data-ttu-id="cd4b1-114">なし。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd4b1-115">子要素</span><span class="sxs-lookup"><span data-stu-id="cd4b1-115">Child elements</span></span>

|<span data-ttu-id="cd4b1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cd4b1-116">**Element**</span></span>|<span data-ttu-id="cd4b1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cd4b1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd4b1-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="cd4b1-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="cd4b1-119">独自の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd4b1-120">親要素</span><span class="sxs-lookup"><span data-stu-id="cd4b1-120">Parent elements</span></span>

|<span data-ttu-id="cd4b1-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="cd4b1-121">**Element**</span></span>|<span data-ttu-id="cd4b1-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="cd4b1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd4b1-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="cd4b1-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="cd4b1-124">特定のユーザーの利用可能時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="cd4b1-125">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd4b1-126">備考</span><span class="sxs-lookup"><span data-stu-id="cd4b1-126">Remarks</span></span>

<span data-ttu-id="cd4b1-127">この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="cd4b1-128">[FreeBusyViewType](freebusyviewtype.md)要素は、**空き時間情報**、 **FreeBusyMerged**、**詳細**、または**DetailedMerged**に設定されている場合、この要素は含まれています。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="cd4b1-129">この要素では、予定表アイテムが要求された時間ウィンドウ内に存在しない場合、すべての子要素は含まれません。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="cd4b1-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd4b1-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="cd4b1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd4b1-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="cd4b1-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd4b1-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cd4b1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="cd4b1-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cd4b1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd4b1-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cd4b1-135">Validation File</span></span>  <br/> |<span data-ttu-id="cd4b1-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd4b1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd4b1-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cd4b1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd4b1-138">False</span><span class="sxs-lookup"><span data-stu-id="cd4b1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd4b1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="cd4b1-139">See also</span></span>



[<span data-ttu-id="cd4b1-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="cd4b1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cd4b1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd4b1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cd4b1-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="cd4b1-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

