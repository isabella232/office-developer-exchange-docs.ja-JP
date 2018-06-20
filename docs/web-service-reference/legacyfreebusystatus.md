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
description: LegacyFreeBusyStatus 要素は、空き/予約済み予定表アイテムの状態を表します。
ms.openlocfilehash: 681d7256dbef09c6c43d33ea1fc92b5d05e73a41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832247"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="570bb-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="570bb-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="570bb-104">**LegacyFreeBusyStatus**要素は、空き/予約済み予定表アイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="570bb-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="570bb-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="570bb-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="570bb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="570bb-106">Attributes and elements</span></span>

<span data-ttu-id="570bb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="570bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="570bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="570bb-108">Attributes</span></span>

<span data-ttu-id="570bb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="570bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="570bb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="570bb-110">Child elements</span></span>

<span data-ttu-id="570bb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="570bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="570bb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="570bb-112">Parent elements</span></span>

|<span data-ttu-id="570bb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="570bb-113">**Element**</span></span>|<span data-ttu-id="570bb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="570bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="570bb-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="570bb-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="570bb-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="570bb-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="570bb-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="570bb-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="570bb-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="570bb-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="570bb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="570bb-119">Text value</span></span>

<span data-ttu-id="570bb-120">テキスト値は、この要素の必要があります。</span><span class="sxs-lookup"><span data-stu-id="570bb-120">A text value is required for this element.</span></span> <span data-ttu-id="570bb-121">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="570bb-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="570bb-122">Free</span><span class="sxs-lookup"><span data-stu-id="570bb-122">Free</span></span> 
- <span data-ttu-id="570bb-123">Tentative</span><span class="sxs-lookup"><span data-stu-id="570bb-123">Tentative</span></span>
- <span data-ttu-id="570bb-124">Busy</span><span class="sxs-lookup"><span data-stu-id="570bb-124">Busy</span></span>
- <span data-ttu-id="570bb-125">不在時</span><span class="sxs-lookup"><span data-stu-id="570bb-125">OOF</span></span>
- <span data-ttu-id="570bb-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="570bb-126">WorkingElsewhere</span></span>
- <span data-ttu-id="570bb-127">NoData</span><span class="sxs-lookup"><span data-stu-id="570bb-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="570bb-128">備考</span><span class="sxs-lookup"><span data-stu-id="570bb-128">Remarks</span></span>

<span data-ttu-id="570bb-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="570bb-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="570bb-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="570bb-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="570bb-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="570bb-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="570bb-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="570bb-132">Schema name</span></span>  <br/> |<span data-ttu-id="570bb-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="570bb-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="570bb-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="570bb-134">Validation file</span></span>  <br/> |<span data-ttu-id="570bb-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="570bb-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="570bb-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="570bb-136">Can be empty</span></span>  <br/> |<span data-ttu-id="570bb-137">False</span><span class="sxs-lookup"><span data-stu-id="570bb-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="570bb-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="570bb-138">See also</span></span>

- [<span data-ttu-id="570bb-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="570bb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

