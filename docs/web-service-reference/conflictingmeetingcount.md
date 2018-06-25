---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: ConflictingMeetingCount 要素は、予定表のアイテムと競合する会議の数を表します。
ms.openlocfilehash: ace800982c284cf65ff22d92c711197ee5ee1d06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759652"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="c0142-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="c0142-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="c0142-104">**ConflictingMeetingCount**要素は、予定表のアイテムと競合する会議の数を表します。</span><span class="sxs-lookup"><span data-stu-id="c0142-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="c0142-105">**int**</span><span class="sxs-lookup"><span data-stu-id="c0142-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0142-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c0142-106">Attributes and elements</span></span>

<span data-ttu-id="c0142-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0142-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0142-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0142-108">Attributes</span></span>

<span data-ttu-id="c0142-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c0142-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0142-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c0142-110">Child elements</span></span>

<span data-ttu-id="c0142-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c0142-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0142-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c0142-112">Parent elements</span></span>

|<span data-ttu-id="c0142-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0142-113">**Element**</span></span>|<span data-ttu-id="c0142-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0142-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0142-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c0142-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c0142-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="c0142-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c0142-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c0142-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c0142-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c0142-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0142-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c0142-119">Text value</span></span>

<span data-ttu-id="c0142-120">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="c0142-120">The text value represents an integer.</span></span> <span data-ttu-id="c0142-121">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="c0142-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0142-122">備考</span><span class="sxs-lookup"><span data-stu-id="c0142-122">Remarks</span></span>

<span data-ttu-id="c0142-123">予定表アイテムが発生した場合、最低では、同じ予定表フォルダー内の別の予定表アイテムと同時に競合するいると見なされます。</span><span class="sxs-lookup"><span data-stu-id="c0142-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="c0142-124">Noncalendar フォルダー内の予定表アイテムの場合は、既定の予定表フォルダーの予定表アイテムが比較されます。</span><span class="sxs-lookup"><span data-stu-id="c0142-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="c0142-125">会議出席依頼は、既定の予定表フォルダーの予定表アイテムと比較されます。</span><span class="sxs-lookup"><span data-stu-id="c0142-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="c0142-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="c0142-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0142-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="c0142-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0142-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="c0142-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0142-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0142-129">Schema name</span></span>  <br/> |<span data-ttu-id="c0142-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c0142-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0142-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0142-131">Validation file</span></span>  <br/> |<span data-ttu-id="c0142-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c0142-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0142-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c0142-133">Can be empty</span></span>  <br/> |<span data-ttu-id="c0142-134">False</span><span class="sxs-lookup"><span data-stu-id="c0142-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0142-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0142-135">See also</span></span>



- [<span data-ttu-id="c0142-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c0142-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

