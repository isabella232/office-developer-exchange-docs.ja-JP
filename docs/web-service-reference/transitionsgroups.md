---
title: TransitionsGroups
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
description: TransitionsGroups 要素は、タイム ゾーンの移行グループの配列を表します。
ms.openlocfilehash: 546dd3c96187bf9f1ebf574b37b689e26e3af997
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839752"
---
# <a name="transitionsgroups"></a><span data-ttu-id="a4517-103">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="a4517-103">TransitionsGroups</span></span>

<span data-ttu-id="a4517-104">**TransitionsGroups**要素は、タイム ゾーンの移行グループの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="a4517-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="a4517-105">**ArrayOfTransitionsGroupsType**</span><span class="sxs-lookup"><span data-stu-id="a4517-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4517-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4517-106">Attributes and elements</span></span>

<span data-ttu-id="a4517-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4517-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4517-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4517-108">Attributes</span></span>

<span data-ttu-id="a4517-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4517-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4517-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4517-110">Child elements</span></span>

|<span data-ttu-id="a4517-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4517-111">**Element**</span></span>|<span data-ttu-id="a4517-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4517-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4517-113">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="a4517-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="a4517-114">タイム ゾーンの移行の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="a4517-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4517-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a4517-115">Parent elements</span></span>

|<span data-ttu-id="a4517-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a4517-116">**Element**</span></span>|<span data-ttu-id="a4517-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4517-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4517-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="a4517-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="a4517-119">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の開始時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="a4517-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="a4517-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="a4517-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="a4517-121">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の終了時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="a4517-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="a4517-122">タイム</span><span class="sxs-lookup"><span data-stu-id="a4517-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="a4517-123">タイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="a4517-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a4517-124">備考</span><span class="sxs-lookup"><span data-stu-id="a4517-124">Remarks</span></span>

<span data-ttu-id="a4517-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4517-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4517-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4517-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4517-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4517-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4517-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4517-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a4517-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a4517-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4517-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4517-130">Validation File</span></span>  <br/> |<span data-ttu-id="a4517-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4517-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4517-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4517-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4517-133">False</span><span class="sxs-lookup"><span data-stu-id="a4517-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4517-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4517-134">See also</span></span>



- [<span data-ttu-id="a4517-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4517-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

