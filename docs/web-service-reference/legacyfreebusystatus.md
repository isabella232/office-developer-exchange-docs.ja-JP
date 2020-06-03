---
title: LegacyFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LegacyFreeBusyStatus
api_type:
- schema
ms.assetid: ee5f3046-b79f-4f68-9455-1a688cee2745
description: LegacyFreeBusyStatus 要素は、予定表アイテムの空き時間状態を表します。
ms.openlocfilehash: ecbcae0862c9c02c0a4a61012816e4c2c6ea07b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463231"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="f4f80-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f4f80-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="f4f80-104">**LegacyFreeBusyStatus**要素は、予定表アイテムの空き時間状態を表します。</span><span class="sxs-lookup"><span data-stu-id="f4f80-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="f4f80-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="f4f80-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f4f80-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f4f80-106">Attributes and elements</span></span>

<span data-ttu-id="f4f80-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4f80-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4f80-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4f80-108">Attributes</span></span>

<span data-ttu-id="f4f80-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f4f80-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4f80-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f4f80-110">Child elements</span></span>

<span data-ttu-id="f4f80-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f4f80-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4f80-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f4f80-112">Parent elements</span></span>

|<span data-ttu-id="f4f80-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4f80-113">**Element**</span></span>|<span data-ttu-id="f4f80-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4f80-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4f80-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f4f80-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f4f80-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f4f80-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f4f80-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f4f80-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f4f80-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f4f80-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4f80-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f4f80-119">Text value</span></span>

<span data-ttu-id="f4f80-120">この要素にはテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4f80-120">A text value is required for this element.</span></span> <span data-ttu-id="f4f80-121">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f4f80-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="f4f80-122">空き</span><span class="sxs-lookup"><span data-stu-id="f4f80-122">Free</span></span> 
- <span data-ttu-id="f4f80-123">仮の予定</span><span class="sxs-lookup"><span data-stu-id="f4f80-123">Tentative</span></span>
- <span data-ttu-id="f4f80-124">多忙</span><span class="sxs-lookup"><span data-stu-id="f4f80-124">Busy</span></span>
- <span data-ttu-id="f4f80-125">OOF</span><span class="sxs-lookup"><span data-stu-id="f4f80-125">OOF</span></span>
- <span data-ttu-id="f4f80-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="f4f80-126">WorkingElsewhere</span></span>
- <span data-ttu-id="f4f80-127">NoData</span><span class="sxs-lookup"><span data-stu-id="f4f80-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f4f80-128">注釈</span><span class="sxs-lookup"><span data-stu-id="f4f80-128">Remarks</span></span>

<span data-ttu-id="f4f80-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f4f80-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4f80-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f4f80-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4f80-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4f80-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4f80-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4f80-132">Schema name</span></span>  <br/> |<span data-ttu-id="f4f80-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f4f80-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4f80-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4f80-134">Validation file</span></span>  <br/> |<span data-ttu-id="f4f80-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f4f80-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4f80-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f4f80-136">Can be empty</span></span>  <br/> |<span data-ttu-id="f4f80-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="f4f80-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4f80-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4f80-138">See also</span></span>

- [<span data-ttu-id="f4f80-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f4f80-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

