---
title: IsException
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsException
api_type:
- schema
ms.assetid: e7bd8ae2-2643-411e-ae08-358bac445800
description: IsException 要素は、定期的な予定表アイテムのインスタンスがマスターから変更されているかどうかを示します。
ms.openlocfilehash: f2e45e0f1010449d4a494f5e15ecd0b22dc598e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457586"
---
# <a name="isexception"></a><span data-ttu-id="70453-103">IsException</span><span class="sxs-lookup"><span data-stu-id="70453-103">IsException</span></span>

<span data-ttu-id="70453-104">**IsException**要素は、定期的な予定表アイテムのインスタンスがマスターから変更されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="70453-104">The **IsException** element indicates whether an instance of a recurring calendar item is changed from the master.</span></span> 
  
[<span data-ttu-id="70453-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="70453-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="70453-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="70453-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="70453-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="70453-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="70453-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="70453-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="70453-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="70453-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="70453-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="70453-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="70453-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="70453-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="70453-112">IsException</span><span class="sxs-lookup"><span data-stu-id="70453-112">IsException</span></span>](isexception.md)
  
```xml
<IsException/>
```

 <span data-ttu-id="70453-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="70453-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70453-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70453-114">Attributes and elements</span></span>

<span data-ttu-id="70453-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70453-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70453-116">属性</span><span class="sxs-lookup"><span data-stu-id="70453-116">Attributes</span></span>

<span data-ttu-id="70453-117">なし。</span><span class="sxs-lookup"><span data-stu-id="70453-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70453-118">子要素</span><span class="sxs-lookup"><span data-stu-id="70453-118">Child elements</span></span>

<span data-ttu-id="70453-119">なし。</span><span class="sxs-lookup"><span data-stu-id="70453-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70453-120">親要素</span><span class="sxs-lookup"><span data-stu-id="70453-120">Parent elements</span></span>

|<span data-ttu-id="70453-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="70453-121">**Element**</span></span>|<span data-ttu-id="70453-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="70453-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70453-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="70453-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="70453-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="70453-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="70453-125">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="70453-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70453-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70453-126">Text value</span></span>

<span data-ttu-id="70453-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="70453-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="70453-128">この要素は、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="70453-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="70453-129">注釈</span><span class="sxs-lookup"><span data-stu-id="70453-129">Remarks</span></span>

<span data-ttu-id="70453-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="70453-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70453-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70453-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70453-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="70453-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70453-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70453-133">Schema Name</span></span>  <br/> |<span data-ttu-id="70453-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70453-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="70453-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70453-135">Validation File</span></span>  <br/> |<span data-ttu-id="70453-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70453-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70453-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70453-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="70453-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="70453-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70453-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="70453-139">See also</span></span>



[<span data-ttu-id="70453-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="70453-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="70453-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="70453-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="70453-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="70453-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

