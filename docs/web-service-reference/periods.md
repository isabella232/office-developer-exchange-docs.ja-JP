---
title: 期間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: ピリオド要素は、タイムゾーンのさまざまな段階での時間オフセットを定義する期間の配列を表します。
ms.openlocfilehash: 773457a6e4c0237eaeaf23109a7022427cc7dd0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467775"
---
# <a name="periods"></a><span data-ttu-id="1dc4f-103">期間</span><span class="sxs-lookup"><span data-stu-id="1dc4f-103">Periods</span></span>

<span data-ttu-id="1dc4f-104">**ピリオド**要素は、タイムゾーンのさまざまな段階での時間オフセットを定義する期間の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="1dc4f-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="1dc4f-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dc4f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1dc4f-106">Attributes and elements</span></span>

<span data-ttu-id="1dc4f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dc4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dc4f-108">Attributes</span></span>

<span data-ttu-id="1dc4f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dc4f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1dc4f-110">Child elements</span></span>

|<span data-ttu-id="1dc4f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1dc4f-111">**Element**</span></span>|<span data-ttu-id="1dc4f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dc4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dc4f-113">Period</span><span class="sxs-lookup"><span data-stu-id="1dc4f-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="1dc4f-114">タイムゾーンの特定のステージの名前、時刻オフセット、および一意識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dc4f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1dc4f-115">Parent elements</span></span>

|<span data-ttu-id="1dc4f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1dc4f-116">**Element**</span></span>|<span data-ttu-id="1dc4f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dc4f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dc4f-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="1dc4f-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="1dc4f-119">[Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="1dc4f-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="1dc4f-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="1dc4f-121">[Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="1dc4f-122">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="1dc4f-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="1dc4f-123">タイムゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1dc4f-124">注釈</span><span class="sxs-lookup"><span data-stu-id="1dc4f-124">Remarks</span></span>

<span data-ttu-id="1dc4f-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1dc4f-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dc4f-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1dc4f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dc4f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dc4f-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dc4f-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1dc4f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1dc4f-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1dc4f-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dc4f-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1dc4f-130">Validation File</span></span>  <br/> |<span data-ttu-id="1dc4f-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1dc4f-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dc4f-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1dc4f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dc4f-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="1dc4f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dc4f-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dc4f-134">See also</span></span>



- [<span data-ttu-id="1dc4f-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1dc4f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

