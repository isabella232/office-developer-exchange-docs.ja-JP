---
title: 遷移のグループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: 推移 Tionsgroups 要素は、タイムゾーン遷移グループの配列を表します。
ms.openlocfilehash: 35244e122ee31045359afd0833459bbb94fd0aa1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467411"
---
# <a name="transitionsgroups"></a><span data-ttu-id="7e80f-103">遷移のグループ</span><span class="sxs-lookup"><span data-stu-id="7e80f-103">TransitionsGroups</span></span>

<span data-ttu-id="7e80f-104">**推移 Tionsgroups**要素は、タイムゾーン遷移グループの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="7e80f-105">**Arrayof遷移 Tionsgroupstype**</span><span class="sxs-lookup"><span data-stu-id="7e80f-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e80f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e80f-106">Attributes and elements</span></span>

<span data-ttu-id="7e80f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e80f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e80f-108">Attributes</span></span>

<span data-ttu-id="7e80f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e80f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e80f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e80f-110">Child elements</span></span>

|<span data-ttu-id="7e80f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7e80f-111">**Element**</span></span>|<span data-ttu-id="7e80f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e80f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e80f-113">遷移 Tionsgroup</span><span class="sxs-lookup"><span data-stu-id="7e80f-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="7e80f-114">タイムゾーンの切り替えの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e80f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7e80f-115">Parent elements</span></span>

|<span data-ttu-id="7e80f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e80f-116">**Element**</span></span>|<span data-ttu-id="7e80f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e80f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e80f-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e80f-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="7e80f-119">[Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="7e80f-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e80f-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="7e80f-121">[Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="7e80f-122">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="7e80f-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="7e80f-123">タイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="7e80f-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e80f-124">注釈</span><span class="sxs-lookup"><span data-stu-id="7e80f-124">Remarks</span></span>

<span data-ttu-id="7e80f-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e80f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e80f-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e80f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e80f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e80f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e80f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e80f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7e80f-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7e80f-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e80f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e80f-130">Validation File</span></span>  <br/> |<span data-ttu-id="7e80f-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7e80f-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e80f-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e80f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e80f-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="7e80f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e80f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e80f-134">See also</span></span>



- [<span data-ttu-id="7e80f-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e80f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

