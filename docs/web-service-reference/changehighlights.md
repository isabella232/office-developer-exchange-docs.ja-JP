---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: 要素は、会議の 2 つのバージョン間で変更内容を指定します。 ChangeHighlights は、メッセージを要求します。
ms.openlocfilehash: 5fe7aa95f60ae95f1af24e8f7a0463ad49716f65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759617"
---
# <a name="changehighlights"></a><span data-ttu-id="cc3f2-103">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="cc3f2-103">ChangeHighlights</span></span>

<span data-ttu-id="cc3f2-104">**ChangeHighlights**要素で指定して、会議の 2 つのバージョン間での変更は、要求メッセージです。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 <span data-ttu-id="cc3f2-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="cc3f2-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc3f2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cc3f2-106">Attributes and elements</span></span>

<span data-ttu-id="cc3f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc3f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc3f2-108">Attributes</span></span>

<span data-ttu-id="cc3f2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc3f2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc3f2-110">Child elements</span></span>

|<span data-ttu-id="cc3f2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc3f2-111">**Element**</span></span>|<span data-ttu-id="cc3f2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc3f2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc3f2-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="cc3f2-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="cc3f2-114">会議の場所のプロパティが変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="cc3f2-115">場所</span><span class="sxs-lookup"><span data-stu-id="cc3f2-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="cc3f2-116">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="cc3f2-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="cc3f2-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="cc3f2-118">会議の開始時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="cc3f2-119">Start</span><span class="sxs-lookup"><span data-stu-id="cc3f2-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="cc3f2-120">期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="cc3f2-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="cc3f2-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="cc3f2-122">会議の終了時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="cc3f2-123">終わり</span><span class="sxs-lookup"><span data-stu-id="cc3f2-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cc3f2-124">期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc3f2-125">親要素</span><span class="sxs-lookup"><span data-stu-id="cc3f2-125">Parent elements</span></span>

|<span data-ttu-id="cc3f2-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc3f2-126">**Element**</span></span>|<span data-ttu-id="cc3f2-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc3f2-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc3f2-128">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cc3f2-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cc3f2-129">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc3f2-130">備考</span><span class="sxs-lookup"><span data-stu-id="cc3f2-130">Remarks</span></span>

<span data-ttu-id="cc3f2-131">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc3f2-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc3f2-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="cc3f2-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc3f2-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="cc3f2-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc3f2-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc3f2-135">Schema Name</span></span>  <br/> |<span data-ttu-id="cc3f2-136">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="cc3f2-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="cc3f2-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc3f2-137">Validation File</span></span>  <br/> |<span data-ttu-id="cc3f2-138">types.xsd</span><span class="sxs-lookup"><span data-stu-id="cc3f2-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc3f2-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cc3f2-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cc3f2-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc3f2-140">See also</span></span>



- [<span data-ttu-id="cc3f2-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc3f2-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

