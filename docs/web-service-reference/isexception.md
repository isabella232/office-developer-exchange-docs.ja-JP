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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457586"
---
# <a name="isexception"></a><span data-ttu-id="0d493-103">IsException</span><span class="sxs-lookup"><span data-stu-id="0d493-103">IsException</span></span>

<span data-ttu-id="0d493-104">**IsException**要素は、定期的な予定表アイテムのインスタンスがマスターから変更されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0d493-104">The **IsException** element indicates whether an instance of a recurring calendar item is changed from the master.</span></span> 
  
[<span data-ttu-id="0d493-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0d493-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0d493-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0d493-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="0d493-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="0d493-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="0d493-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="0d493-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="0d493-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="0d493-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="0d493-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0d493-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="0d493-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0d493-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="0d493-112">IsException</span><span class="sxs-lookup"><span data-stu-id="0d493-112">IsException</span></span>](isexception.md)
  
```xml
<IsException/>
```

 <span data-ttu-id="0d493-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0d493-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d493-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0d493-114">Attributes and elements</span></span>

<span data-ttu-id="0d493-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0d493-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d493-116">属性</span><span class="sxs-lookup"><span data-stu-id="0d493-116">Attributes</span></span>

<span data-ttu-id="0d493-117">なし。</span><span class="sxs-lookup"><span data-stu-id="0d493-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d493-118">子要素</span><span class="sxs-lookup"><span data-stu-id="0d493-118">Child elements</span></span>

<span data-ttu-id="0d493-119">なし。</span><span class="sxs-lookup"><span data-stu-id="0d493-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d493-120">親要素</span><span class="sxs-lookup"><span data-stu-id="0d493-120">Parent elements</span></span>

|<span data-ttu-id="0d493-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="0d493-121">**Element**</span></span>|<span data-ttu-id="0d493-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0d493-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d493-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0d493-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="0d493-124">予定表イベントに関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0d493-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="0d493-125">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d493-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d493-126">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0d493-126">Text value</span></span>

<span data-ttu-id="0d493-127">この要素が応答で返される場合は、テキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d493-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="0d493-128">この要素は、 [CalendarEventDetails](calendareventdetails.md)要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="0d493-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0d493-129">注釈</span><span class="sxs-lookup"><span data-stu-id="0d493-129">Remarks</span></span>

<span data-ttu-id="0d493-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0d493-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d493-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0d493-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d493-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d493-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d493-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0d493-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0d493-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0d493-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d493-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0d493-135">Validation File</span></span>  <br/> |<span data-ttu-id="0d493-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0d493-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d493-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0d493-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d493-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="0d493-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d493-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="0d493-139">See also</span></span>



[<span data-ttu-id="0d493-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="0d493-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0d493-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0d493-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0d493-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="0d493-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

