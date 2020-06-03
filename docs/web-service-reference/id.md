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
ms.openlocfilehash: 429413bbfb0206effc3ea97eb11527449c67211c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456487"
---
# <a name="id"></a><span data-ttu-id="f7143-103">ID</span><span class="sxs-lookup"><span data-stu-id="f7143-103">ID</span></span>

<span data-ttu-id="f7143-104">**ID**要素は、予定表アイテムのエントリ ID を表します。</span><span class="sxs-lookup"><span data-stu-id="f7143-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="f7143-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f7143-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f7143-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f7143-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f7143-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f7143-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f7143-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f7143-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f7143-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="f7143-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="f7143-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="f7143-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="f7143-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="f7143-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="f7143-112">ID</span><span class="sxs-lookup"><span data-stu-id="f7143-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="f7143-113">**string**</span><span class="sxs-lookup"><span data-stu-id="f7143-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7143-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f7143-114">Attributes and elements</span></span>

<span data-ttu-id="f7143-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7143-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7143-116">属性</span><span class="sxs-lookup"><span data-stu-id="f7143-116">Attributes</span></span>

<span data-ttu-id="f7143-117">なし。</span><span class="sxs-lookup"><span data-stu-id="f7143-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7143-118">子要素</span><span class="sxs-lookup"><span data-stu-id="f7143-118">Child elements</span></span>

<span data-ttu-id="f7143-119">なし。</span><span class="sxs-lookup"><span data-stu-id="f7143-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7143-120">親要素</span><span class="sxs-lookup"><span data-stu-id="f7143-120">Parent elements</span></span>

|<span data-ttu-id="f7143-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="f7143-121">**Element**</span></span>|<span data-ttu-id="f7143-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7143-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7143-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="f7143-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="f7143-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f7143-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="f7143-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7143-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7143-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f7143-126">Text value</span></span>

<span data-ttu-id="f7143-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="f7143-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="f7143-128">この要素は、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="f7143-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f7143-129">注釈</span><span class="sxs-lookup"><span data-stu-id="f7143-129">Remarks</span></span>

<span data-ttu-id="f7143-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f7143-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7143-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f7143-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7143-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7143-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7143-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7143-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f7143-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f7143-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7143-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7143-135">Validation File</span></span>  <br/> |<span data-ttu-id="f7143-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f7143-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7143-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f7143-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7143-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="f7143-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7143-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="f7143-139">See also</span></span>



[<span data-ttu-id="f7143-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="f7143-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f7143-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f7143-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f7143-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="f7143-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

