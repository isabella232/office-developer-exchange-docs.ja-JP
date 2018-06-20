---
title: ID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ID
api_type:
- schema
ms.assetid: 8caf922f-56bd-466a-a68f-d6cb236f2eec
description: ID 要素は、予定表アイテムのエントリ ID を表します。
ms.openlocfilehash: bdfadcbe074135aca34a408e69ed4a69974eb5d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831855"
---
# <a name="id"></a><span data-ttu-id="38e45-103">ID</span><span class="sxs-lookup"><span data-stu-id="38e45-103">ID</span></span>

<span data-ttu-id="38e45-104">**ID**要素は、予定表アイテムのエントリ ID を表します。</span><span class="sxs-lookup"><span data-stu-id="38e45-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="38e45-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="38e45-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="38e45-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="38e45-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="38e45-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="38e45-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="38e45-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="38e45-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="38e45-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="38e45-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="38e45-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="38e45-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="38e45-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="38e45-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="38e45-112">ID</span><span class="sxs-lookup"><span data-stu-id="38e45-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="38e45-113">**string**</span><span class="sxs-lookup"><span data-stu-id="38e45-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38e45-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="38e45-114">Attributes and elements</span></span>

<span data-ttu-id="38e45-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38e45-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38e45-116">属性</span><span class="sxs-lookup"><span data-stu-id="38e45-116">Attributes</span></span>

<span data-ttu-id="38e45-117">なし。</span><span class="sxs-lookup"><span data-stu-id="38e45-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38e45-118">子要素</span><span class="sxs-lookup"><span data-stu-id="38e45-118">Child elements</span></span>

<span data-ttu-id="38e45-119">なし。</span><span class="sxs-lookup"><span data-stu-id="38e45-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38e45-120">親要素</span><span class="sxs-lookup"><span data-stu-id="38e45-120">Parent elements</span></span>

|<span data-ttu-id="38e45-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="38e45-121">**Element**</span></span>|<span data-ttu-id="38e45-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="38e45-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38e45-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="38e45-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="38e45-124">カレンダー イベントの追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="38e45-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="38e45-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="38e45-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38e45-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="38e45-126">Text value</span></span>

<span data-ttu-id="38e45-127">テキスト値は、この要素が応答で返された場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="38e45-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="38e45-128">[CalendarEventDetails](calendareventdetails.md)要素を使用する場合、この要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="38e45-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="38e45-129">備考</span><span class="sxs-lookup"><span data-stu-id="38e45-129">Remarks</span></span>

<span data-ttu-id="38e45-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="38e45-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38e45-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="38e45-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38e45-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="38e45-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38e45-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38e45-133">Schema Name</span></span>  <br/> |<span data-ttu-id="38e45-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="38e45-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="38e45-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38e45-135">Validation File</span></span>  <br/> |<span data-ttu-id="38e45-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38e45-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38e45-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="38e45-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="38e45-138">False</span><span class="sxs-lookup"><span data-stu-id="38e45-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38e45-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="38e45-139">See also</span></span>



[<span data-ttu-id="38e45-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="38e45-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="38e45-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="38e45-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="38e45-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="38e45-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

