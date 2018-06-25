---
title: IsRecurring (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: 42323940-0ccb-4a05-86e4-262bde5e41b0
description: IsRecurring 要素は、予定表のイベントが定期的な予定表アイテムまたは単一の予定表アイテムのインスタンスであるかどうかを示します。
ms.openlocfilehash: 87a168dc48bdd5ba2ea9398dd84f696e7729db44
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832103"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="bc491-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="bc491-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="bc491-104">**IsRecurring**要素は、予定表のイベントが定期的な予定表アイテムまたは単一の予定表アイテムのインスタンスであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bc491-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="bc491-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bc491-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="bc491-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="bc491-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="bc491-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="bc491-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="bc491-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="bc491-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="bc491-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="bc491-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="bc491-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="bc491-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="bc491-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="bc491-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="bc491-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="bc491-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="bc491-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="bc491-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc491-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="bc491-114">Attributes and elements</span></span>

<span data-ttu-id="bc491-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc491-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc491-116">属性</span><span class="sxs-lookup"><span data-stu-id="bc491-116">Attributes</span></span>

<span data-ttu-id="bc491-117">なし。</span><span class="sxs-lookup"><span data-stu-id="bc491-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc491-118">子要素</span><span class="sxs-lookup"><span data-stu-id="bc491-118">Child elements</span></span>

<span data-ttu-id="bc491-119">なし。</span><span class="sxs-lookup"><span data-stu-id="bc491-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc491-120">親要素</span><span class="sxs-lookup"><span data-stu-id="bc491-120">Parent elements</span></span>

|<span data-ttu-id="bc491-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc491-121">**Element**</span></span>|<span data-ttu-id="bc491-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc491-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc491-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="bc491-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="bc491-124">予定表のイベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="bc491-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="bc491-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="bc491-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc491-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bc491-126">Text value</span></span>

<span data-ttu-id="bc491-127">テキスト値は、この要素が応答で返された場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="bc491-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="bc491-128">[CalendarEventDetails](calendareventdetails.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc491-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bc491-129">備考</span><span class="sxs-lookup"><span data-stu-id="bc491-129">Remarks</span></span>

<span data-ttu-id="bc491-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="bc491-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc491-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="bc491-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc491-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="bc491-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc491-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc491-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bc491-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="bc491-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc491-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc491-135">Validation File</span></span>  <br/> |<span data-ttu-id="bc491-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc491-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc491-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bc491-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc491-138">False</span><span class="sxs-lookup"><span data-stu-id="bc491-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc491-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc491-139">See also</span></span>



[<span data-ttu-id="bc491-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="bc491-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bc491-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bc491-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="bc491-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="bc491-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

