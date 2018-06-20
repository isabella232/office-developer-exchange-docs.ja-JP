---
title: StartTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeZone
api_type:
- schema
ms.assetid: d38c4dc1-4ecb-42a1-8d57-a451b16a2de2
description: StartTimeZone 要素は、カレンダー項目または MeetingRequest の開始時刻のタイム ゾーンを定義します。
ms.openlocfilehash: 6d21869c4b3be048db27dcc9f128fff868aebcb5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833559"
---
# <a name="starttimezone"></a><span data-ttu-id="4d66d-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="4d66d-103">StartTimeZone</span></span>

<span data-ttu-id="4d66d-104">**StartTimeZone**要素は、[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の開始時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="4d66d-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="4d66d-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4d66d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4d66d-106">Attributes and elements</span></span>

<span data-ttu-id="4d66d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d66d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d66d-108">Attributes</span></span>

|<span data-ttu-id="4d66d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4d66d-109">**Attribute**</span></span>|<span data-ttu-id="4d66d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d66d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d66d-111">ID</span><span class="sxs-lookup"><span data-stu-id="4d66d-111">Id</span></span>  <br/> |<span data-ttu-id="4d66d-112">タイム ゾーン定義の一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="4d66d-113">名前</span><span class="sxs-lookup"><span data-stu-id="4d66d-113">Name</span></span>  <br/> |<span data-ttu-id="4d66d-114">タイム ゾーン定義のわかりやすい名前を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4d66d-115">子要素</span><span class="sxs-lookup"><span data-stu-id="4d66d-115">Child elements</span></span>

|<span data-ttu-id="4d66d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d66d-116">**Element**</span></span>|<span data-ttu-id="4d66d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d66d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d66d-118">Periods</span><span class="sxs-lookup"><span data-stu-id="4d66d-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="4d66d-119">タイム ゾーンのさまざまな段階での時刻のオフセットを定義する[期間](period.md)の要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="4d66d-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="4d66d-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="4d66d-121">タイムゾーンの遷移を指定する[TransitionsGroup](transitionsgroup.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="4d66d-122">遷移</span><span class="sxs-lookup"><span data-stu-id="4d66d-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="4d66d-123">タイム ゾーンの移行の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d66d-124">親要素</span><span class="sxs-lookup"><span data-stu-id="4d66d-124">Parent elements</span></span>

|<span data-ttu-id="4d66d-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="4d66d-125">**Element**</span></span>|<span data-ttu-id="4d66d-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="4d66d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d66d-127">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="4d66d-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4d66d-128">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4d66d-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4d66d-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4d66d-130">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="4d66d-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d66d-131">備考</span><span class="sxs-lookup"><span data-stu-id="4d66d-131">Remarks</span></span>

<span data-ttu-id="4d66d-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4d66d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d66d-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="4d66d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d66d-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="4d66d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d66d-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4d66d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="4d66d-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4d66d-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d66d-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4d66d-137">Validation File</span></span>  <br/> |<span data-ttu-id="4d66d-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d66d-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d66d-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4d66d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d66d-140">False</span><span class="sxs-lookup"><span data-stu-id="4d66d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d66d-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="4d66d-141">See also</span></span>

- [<span data-ttu-id="4d66d-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4d66d-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

