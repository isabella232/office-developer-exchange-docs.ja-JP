---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: EndTimeZone 要素は、CalendarItem または会議の要求の終了時刻のタイムゾーンを定義します。
ms.openlocfilehash: 83ab2ab90e2bed7658fe83ed33a72b60d5f10135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462986"
---
# <a name="endtimezone"></a><span data-ttu-id="29b97-103">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="29b97-103">EndTimeZone</span></span>

<span data-ttu-id="29b97-104">**Endtimezone**要素は、 [Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="29b97-104">The **EndTimeZone** element defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 <span data-ttu-id="29b97-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="29b97-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29b97-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29b97-106">Attributes and elements</span></span>

<span data-ttu-id="29b97-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29b97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29b97-108">属性</span><span class="sxs-lookup"><span data-stu-id="29b97-108">Attributes</span></span>

|<span data-ttu-id="29b97-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="29b97-109">**Attribute**</span></span>|<span data-ttu-id="29b97-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="29b97-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29b97-111">ID</span><span class="sxs-lookup"><span data-stu-id="29b97-111">Id</span></span>  <br/> |<span data-ttu-id="29b97-112">タイムゾーン定義の一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="29b97-113">名前</span><span class="sxs-lookup"><span data-stu-id="29b97-113">Name</span></span>  <br/> |<span data-ttu-id="29b97-114">タイムゾーン定義のわかりやすい名前を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="29b97-115">子要素</span><span class="sxs-lookup"><span data-stu-id="29b97-115">Child elements</span></span>

|<span data-ttu-id="29b97-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="29b97-116">**Element**</span></span>|<span data-ttu-id="29b97-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="29b97-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29b97-118">Periods</span><span class="sxs-lookup"><span data-stu-id="29b97-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="29b97-119">タイムゾーンのさまざまな段階での時間のオフセットを定義する[Period](period.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="29b97-120">遷移のグループ</span><span class="sxs-lookup"><span data-stu-id="29b97-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="29b97-121">タイムゾーンの遷移を指定する、[推移 Tionsgroup](transitionsgroup.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="29b97-122">切り替わる</span><span class="sxs-lookup"><span data-stu-id="29b97-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="29b97-123">タイムゾーンの切り替えの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29b97-124">親要素</span><span class="sxs-lookup"><span data-stu-id="29b97-124">Parent elements</span></span>

|<span data-ttu-id="29b97-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="29b97-125">**Element**</span></span>|<span data-ttu-id="29b97-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="29b97-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29b97-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="29b97-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="29b97-128">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="29b97-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="29b97-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="29b97-130">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="29b97-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29b97-131">注釈</span><span class="sxs-lookup"><span data-stu-id="29b97-131">Remarks</span></span>

<span data-ttu-id="29b97-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="29b97-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29b97-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29b97-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29b97-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="29b97-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29b97-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29b97-135">Schema Name</span></span>  <br/> |<span data-ttu-id="29b97-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="29b97-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="29b97-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29b97-137">Validation File</span></span>  <br/> |<span data-ttu-id="29b97-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29b97-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29b97-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29b97-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="29b97-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="29b97-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29b97-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="29b97-141">See also</span></span>



- [<span data-ttu-id="29b97-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29b97-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

