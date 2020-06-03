---
title: 標準
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Standard 要素は、夏時間から標準時に時刻が変更された日付と時刻を表します。
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467565"
---
# <a name="standard"></a><span data-ttu-id="a8fca-103">標準</span><span class="sxs-lookup"><span data-stu-id="a8fca-103">Standard</span></span>

<span data-ttu-id="a8fca-104">**Standard**要素は、夏時間から標準時に時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

<span data-ttu-id="a8fca-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="a8fca-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8fca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8fca-106">Attributes and elements</span></span>

<span data-ttu-id="a8fca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8fca-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8fca-108">Attributes</span></span>

|<span data-ttu-id="a8fca-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="a8fca-109">**Attribute**</span></span>|<span data-ttu-id="a8fca-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8fca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a8fca-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="a8fca-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="a8fca-112">タイムゾーンの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a8fca-113">子要素</span><span class="sxs-lookup"><span data-stu-id="a8fca-113">Child elements</span></span>

|<span data-ttu-id="a8fca-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="a8fca-114">**Element**</span></span>|<span data-ttu-id="a8fca-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8fca-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8fca-116">Offset</span><span class="sxs-lookup"><span data-stu-id="a8fca-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="a8fca-117">[Baseoffset](baseoffset.md)からのオフセットを記述します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="a8fca-118">**Baseoffset**要素と共に、 **Offset**要素は時刻が標準時であるか夏時間であるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a8fca-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a8fca-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="a8fca-120">タイムゾーンの移行日の相対的な年単位のパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="a8fca-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="a8fca-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="a8fca-122">標準時または夏時間から時刻が変更された日付を表します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="a8fca-123">Time (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="a8fca-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="a8fca-124">時刻が標準時と夏時間の間に変化する時間を表します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8fca-125">親要素</span><span class="sxs-lookup"><span data-stu-id="a8fca-125">Parent elements</span></span>

|<span data-ttu-id="a8fca-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8fca-126">**Element**</span></span>|<span data-ttu-id="a8fca-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8fca-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8fca-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="a8fca-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="a8fca-129">会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="a8fca-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8fca-130">注釈</span><span class="sxs-lookup"><span data-stu-id="a8fca-130">Remarks</span></span>

<span data-ttu-id="a8fca-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a8fca-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8fca-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8fca-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8fca-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8fca-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8fca-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8fca-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a8fca-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8fca-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8fca-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8fca-136">Validation File</span></span>  <br/> |<span data-ttu-id="a8fca-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8fca-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8fca-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8fca-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8fca-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8fca-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8fca-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8fca-140">See also</span></span>

- [<span data-ttu-id="a8fca-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8fca-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

