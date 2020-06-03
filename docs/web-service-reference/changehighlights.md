---
title: ChangeHighlights 強調表示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: ChangeHighlights 要素は、2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463280"
---
# <a name="changehighlights"></a><span data-ttu-id="d4fe1-103">ChangeHighlights 強調表示</span><span class="sxs-lookup"><span data-stu-id="d4fe1-103">ChangeHighlights</span></span>

<span data-ttu-id="d4fe1-104">**Changehighlights**要素は、2つのバージョンの会議出席依頼メッセージの間で変更されたものを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
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

 <span data-ttu-id="d4fe1-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="d4fe1-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4fe1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d4fe1-106">Attributes and elements</span></span>

<span data-ttu-id="d4fe1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4fe1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4fe1-108">Attributes</span></span>

<span data-ttu-id="d4fe1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4fe1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4fe1-110">Child elements</span></span>

|<span data-ttu-id="d4fe1-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d4fe1-111">**Element**</span></span>|<span data-ttu-id="d4fe1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fe1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fe1-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="d4fe1-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="d4fe1-114">会議の場所プロパティが変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="d4fe1-115">場所</span><span class="sxs-lookup"><span data-stu-id="d4fe1-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="d4fe1-116">会議または予定の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="d4fe1-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="d4fe1-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="d4fe1-118">会議の開始時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="d4fe1-119">開始</span><span class="sxs-lookup"><span data-stu-id="d4fe1-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="d4fe1-120">期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="d4fe1-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="d4fe1-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="d4fe1-122">会議の終了時刻が変更されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="d4fe1-123">終わり</span><span class="sxs-lookup"><span data-stu-id="d4fe1-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d4fe1-124">期間の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4fe1-125">親要素</span><span class="sxs-lookup"><span data-stu-id="d4fe1-125">Parent elements</span></span>

|<span data-ttu-id="d4fe1-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4fe1-126">**Element**</span></span>|<span data-ttu-id="d4fe1-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fe1-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fe1-128">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d4fe1-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d4fe1-129">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4fe1-130">注釈</span><span class="sxs-lookup"><span data-stu-id="d4fe1-130">Remarks</span></span>

<span data-ttu-id="d4fe1-131">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d4fe1-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4fe1-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d4fe1-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4fe1-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4fe1-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4fe1-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4fe1-135">Schema Name</span></span>  <br/> |<span data-ttu-id="d4fe1-136">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="d4fe1-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="d4fe1-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4fe1-137">Validation File</span></span>  <br/> |<span data-ttu-id="d4fe1-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d4fe1-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4fe1-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d4fe1-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d4fe1-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4fe1-140">See also</span></span>



- [<span data-ttu-id="d4fe1-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4fe1-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

