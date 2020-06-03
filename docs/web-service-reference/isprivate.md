---
title: IsPrivate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPrivate
api_type:
- schema
ms.assetid: 1712bc94-9789-4507-8521-bde1be51e331
description: IsPrivate 要素は、予定表アイテムがプライベートであるかどうかを示します。
ms.openlocfilehash: c36c659414700439436cd2ca903e443164c1473b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457803"
---
# <a name="isprivate"></a><span data-ttu-id="e8ff4-103">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="e8ff4-103">IsPrivate</span></span>

<span data-ttu-id="e8ff4-104">**IsPrivate**要素は、予定表アイテムがプライベートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="e8ff4-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e8ff4-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e8ff4-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="e8ff4-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="e8ff4-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="e8ff4-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="e8ff4-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e8ff4-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="e8ff4-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="e8ff4-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="e8ff4-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="e8ff4-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="e8ff4-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="e8ff4-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="e8ff4-112">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="e8ff4-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="e8ff4-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e8ff4-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8ff4-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8ff4-114">Attributes and elements</span></span>

<span data-ttu-id="e8ff4-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8ff4-116">属性</span><span class="sxs-lookup"><span data-stu-id="e8ff4-116">Attributes</span></span>

<span data-ttu-id="e8ff4-117">なし。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8ff4-118">子要素</span><span class="sxs-lookup"><span data-stu-id="e8ff4-118">Child elements</span></span>

<span data-ttu-id="e8ff4-119">なし。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8ff4-120">親要素</span><span class="sxs-lookup"><span data-stu-id="e8ff4-120">Parent elements</span></span>

|<span data-ttu-id="e8ff4-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8ff4-121">**Element**</span></span>|<span data-ttu-id="e8ff4-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8ff4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8ff4-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="e8ff4-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="e8ff4-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="e8ff4-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8ff4-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e8ff4-126">Text value</span></span>

<span data-ttu-id="e8ff4-127">ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8ff4-128">注釈</span><span class="sxs-lookup"><span data-stu-id="e8ff4-128">Remarks</span></span>

<span data-ttu-id="e8ff4-129">この要素を使用すると、 [CalendarEventDetails](calendareventdetails.md)要素の他の要素は応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="e8ff4-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e8ff4-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8ff4-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8ff4-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8ff4-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8ff4-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8ff4-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8ff4-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e8ff4-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8ff4-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8ff4-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8ff4-135">Validation File</span></span>  <br/> |<span data-ttu-id="e8ff4-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8ff4-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8ff4-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e8ff4-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8ff4-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="e8ff4-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8ff4-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8ff4-139">See also</span></span>



[<span data-ttu-id="e8ff4-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e8ff4-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e8ff4-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e8ff4-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e8ff4-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="e8ff4-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

