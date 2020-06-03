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
description: StartTimeZone 要素は、CalendarItem または会議要求の開始時刻のタイムゾーンを定義します。
ms.openlocfilehash: fa88f676c0f6a7a2e934f51274942ed3bccbc789
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458524"
---
# <a name="starttimezone"></a><span data-ttu-id="70874-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="70874-103">StartTimeZone</span></span>

<span data-ttu-id="70874-104">**Starttimezone**要素は、 [Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="70874-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="70874-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="70874-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="70874-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70874-106">Attributes and elements</span></span>

<span data-ttu-id="70874-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70874-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70874-108">属性</span><span class="sxs-lookup"><span data-stu-id="70874-108">Attributes</span></span>

|<span data-ttu-id="70874-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="70874-109">**Attribute**</span></span>|<span data-ttu-id="70874-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="70874-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70874-111">ID</span><span class="sxs-lookup"><span data-stu-id="70874-111">Id</span></span>  <br/> |<span data-ttu-id="70874-112">タイムゾーン定義の一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="70874-113">名前</span><span class="sxs-lookup"><span data-stu-id="70874-113">Name</span></span>  <br/> |<span data-ttu-id="70874-114">タイムゾーン定義のわかりやすい名前を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70874-115">子要素</span><span class="sxs-lookup"><span data-stu-id="70874-115">Child elements</span></span>

|<span data-ttu-id="70874-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="70874-116">**Element**</span></span>|<span data-ttu-id="70874-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="70874-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70874-118">Periods</span><span class="sxs-lookup"><span data-stu-id="70874-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="70874-119">タイムゾーンのさまざまな段階での時間のオフセットを定義する[Period](period.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="70874-120">遷移のグループ</span><span class="sxs-lookup"><span data-stu-id="70874-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="70874-121">タイムゾーンの遷移を指定する、[推移 Tionsgroup](transitionsgroup.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="70874-122">切り替わる</span><span class="sxs-lookup"><span data-stu-id="70874-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="70874-123">タイムゾーンの切り替えの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70874-124">親要素</span><span class="sxs-lookup"><span data-stu-id="70874-124">Parent elements</span></span>

|<span data-ttu-id="70874-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="70874-125">**Element**</span></span>|<span data-ttu-id="70874-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="70874-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70874-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="70874-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="70874-128">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="70874-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="70874-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="70874-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="70874-130">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="70874-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="70874-131">注釈</span><span class="sxs-lookup"><span data-stu-id="70874-131">Remarks</span></span>

<span data-ttu-id="70874-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="70874-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70874-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70874-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70874-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="70874-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70874-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70874-135">Schema Name</span></span>  <br/> |<span data-ttu-id="70874-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70874-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="70874-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70874-137">Validation File</span></span>  <br/> |<span data-ttu-id="70874-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70874-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70874-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70874-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="70874-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="70874-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70874-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="70874-141">See also</span></span>

- [<span data-ttu-id="70874-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="70874-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

