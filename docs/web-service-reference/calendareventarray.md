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
description: CalendarEventArray 要素には、要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムが含まれています。
ms.openlocfilehash: 6badba2477a9d48c6d109740de454e2815d3c211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463371"
---
# <a name="calendareventarray"></a><span data-ttu-id="ba34f-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="ba34f-103">CalendarEventArray</span></span>

<span data-ttu-id="ba34f-104">**CalendarEventArray**要素には、要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba34f-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="ba34f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ba34f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ba34f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ba34f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ba34f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ba34f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ba34f-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ba34f-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ba34f-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="ba34f-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="ba34f-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="ba34f-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba34f-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ba34f-111">Attributes and elements</span></span>

<span data-ttu-id="ba34f-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba34f-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba34f-113">属性</span><span class="sxs-lookup"><span data-stu-id="ba34f-113">Attributes</span></span>

<span data-ttu-id="ba34f-114">なし。</span><span class="sxs-lookup"><span data-stu-id="ba34f-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba34f-115">子要素</span><span class="sxs-lookup"><span data-stu-id="ba34f-115">Child elements</span></span>

|<span data-ttu-id="ba34f-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="ba34f-116">**Element**</span></span>|<span data-ttu-id="ba34f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba34f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba34f-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="ba34f-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="ba34f-119">一意の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="ba34f-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba34f-120">親要素</span><span class="sxs-lookup"><span data-stu-id="ba34f-120">Parent elements</span></span>

|<span data-ttu-id="ba34f-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="ba34f-121">**Element**</span></span>|<span data-ttu-id="ba34f-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba34f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba34f-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ba34f-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="ba34f-124">特定のユーザーの空き時間情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="ba34f-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="ba34f-125">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba34f-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba34f-126">注釈</span><span class="sxs-lookup"><span data-stu-id="ba34f-126">Remarks</span></span>

<span data-ttu-id="ba34f-127">この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。</span><span class="sxs-lookup"><span data-stu-id="ba34f-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="ba34f-128">この要素は、 [FreeBusyViewType](freebusyviewtype.md)要素が**FreeBusy**、 **FreeBusyMerged**、 **Detailed**、または**DetailedMerged**に設定されている場合に含まれます。</span><span class="sxs-lookup"><span data-stu-id="ba34f-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="ba34f-129">要求された時間枠に予定表アイテムが存在しない場合、この要素には子要素は含まれません。</span><span class="sxs-lookup"><span data-stu-id="ba34f-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="ba34f-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ba34f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba34f-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ba34f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba34f-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba34f-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba34f-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba34f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ba34f-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ba34f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba34f-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba34f-135">Validation File</span></span>  <br/> |<span data-ttu-id="ba34f-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ba34f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba34f-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ba34f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba34f-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="ba34f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba34f-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba34f-139">See also</span></span>



[<span data-ttu-id="ba34f-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="ba34f-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ba34f-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ba34f-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ba34f-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="ba34f-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

