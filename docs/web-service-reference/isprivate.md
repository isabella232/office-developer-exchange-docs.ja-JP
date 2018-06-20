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
description: IsPrivate 要素は、予定表アイテムがプライベートかどうかを示します。
ms.openlocfilehash: 37c0357b3eab2314ee74e1c98287b3dc05a3bf26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832095"
---
# <a name="isprivate"></a><span data-ttu-id="32419-103">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="32419-103">IsPrivate</span></span>

<span data-ttu-id="32419-104">**IsPrivate**要素は、予定表アイテムがプライベートかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="32419-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="32419-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32419-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="32419-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="32419-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="32419-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="32419-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="32419-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="32419-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="32419-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="32419-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="32419-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="32419-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="32419-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="32419-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="32419-112">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="32419-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="32419-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="32419-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32419-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32419-114">Attributes and elements</span></span>

<span data-ttu-id="32419-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32419-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32419-116">属性</span><span class="sxs-lookup"><span data-stu-id="32419-116">Attributes</span></span>

<span data-ttu-id="32419-117">なし。</span><span class="sxs-lookup"><span data-stu-id="32419-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32419-118">子要素</span><span class="sxs-lookup"><span data-stu-id="32419-118">Child elements</span></span>

<span data-ttu-id="32419-119">なし。</span><span class="sxs-lookup"><span data-stu-id="32419-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32419-120">親要素</span><span class="sxs-lookup"><span data-stu-id="32419-120">Parent elements</span></span>

|<span data-ttu-id="32419-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="32419-121">**Element**</span></span>|<span data-ttu-id="32419-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="32419-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32419-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="32419-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="32419-124">予定表のイベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="32419-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="32419-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="32419-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32419-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32419-126">Text value</span></span>

<span data-ttu-id="32419-127">ブール値を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="32419-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32419-128">備考</span><span class="sxs-lookup"><span data-stu-id="32419-128">Remarks</span></span>

<span data-ttu-id="32419-129">この要素を使用すると、 [CalendarEventDetails](calendareventdetails.md)要素内の他の要素は、応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="32419-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="32419-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="32419-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32419-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="32419-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32419-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="32419-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32419-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32419-133">Schema Name</span></span>  <br/> |<span data-ttu-id="32419-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="32419-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="32419-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32419-135">Validation File</span></span>  <br/> |<span data-ttu-id="32419-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32419-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32419-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32419-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="32419-138">False</span><span class="sxs-lookup"><span data-stu-id="32419-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32419-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="32419-139">See also</span></span>



[<span data-ttu-id="32419-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="32419-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="32419-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32419-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="32419-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="32419-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

