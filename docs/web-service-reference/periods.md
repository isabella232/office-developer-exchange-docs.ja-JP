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
description: ピリオド要素では、タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832729"
---
# <a name="periods"></a><span data-ttu-id="29c85-103">期間</span><span class="sxs-lookup"><span data-stu-id="29c85-103">Periods</span></span>

<span data-ttu-id="29c85-104">**ピリオド**要素では、タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="29c85-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="29c85-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="29c85-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29c85-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="29c85-106">Attributes and elements</span></span>

<span data-ttu-id="29c85-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29c85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29c85-108">属性</span><span class="sxs-lookup"><span data-stu-id="29c85-108">Attributes</span></span>

<span data-ttu-id="29c85-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29c85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29c85-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29c85-110">Child elements</span></span>

|<span data-ttu-id="29c85-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="29c85-111">**Element**</span></span>|<span data-ttu-id="29c85-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="29c85-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29c85-113">Period</span><span class="sxs-lookup"><span data-stu-id="29c85-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="29c85-114">タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="29c85-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29c85-115">親要素</span><span class="sxs-lookup"><span data-stu-id="29c85-115">Parent elements</span></span>

|<span data-ttu-id="29c85-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="29c85-116">**Element**</span></span>|<span data-ttu-id="29c85-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="29c85-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29c85-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="29c85-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="29c85-119">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の開始時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="29c85-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="29c85-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="29c85-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="29c85-121">[カレンダー項目](calendaritem.md)または[MeetingRequest](meetingrequest.md)の終了時刻のタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="29c85-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="29c85-122">タイム</span><span class="sxs-lookup"><span data-stu-id="29c85-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="29c85-123">タイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="29c85-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29c85-124">備考</span><span class="sxs-lookup"><span data-stu-id="29c85-124">Remarks</span></span>

<span data-ttu-id="29c85-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="29c85-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29c85-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="29c85-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29c85-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="29c85-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29c85-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29c85-128">Schema Name</span></span>  <br/> |<span data-ttu-id="29c85-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="29c85-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="29c85-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29c85-130">Validation File</span></span>  <br/> |<span data-ttu-id="29c85-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="29c85-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29c85-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29c85-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="29c85-133">False</span><span class="sxs-lookup"><span data-stu-id="29c85-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29c85-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="29c85-134">See also</span></span>



- [<span data-ttu-id="29c85-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="29c85-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

