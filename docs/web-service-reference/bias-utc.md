---
title: Bias (UTC)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: Bias 要素は、世界協定時刻 (UTC) からの一般的なオフセットを表します。 この値は分単位です。
ms.openlocfilehash: d95284aa28e59542d1a1ee40686163138b015702
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460247"
---
# <a name="bias-utc"></a><span data-ttu-id="538fd-104">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="538fd-104">Bias (UTC)</span></span>

<span data-ttu-id="538fd-105">**Bias**要素は、世界協定時刻 (UTC) からの一般的なオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="538fd-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="538fd-106">この値は分単位です。</span><span class="sxs-lookup"><span data-stu-id="538fd-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="538fd-107">**int**</span><span class="sxs-lookup"><span data-stu-id="538fd-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="538fd-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="538fd-108">Attributes and elements</span></span>

<span data-ttu-id="538fd-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="538fd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="538fd-110">属性</span><span class="sxs-lookup"><span data-stu-id="538fd-110">Attributes</span></span>

<span data-ttu-id="538fd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="538fd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="538fd-112">子要素</span><span class="sxs-lookup"><span data-stu-id="538fd-112">Child elements</span></span>

<span data-ttu-id="538fd-113">なし。</span><span class="sxs-lookup"><span data-stu-id="538fd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="538fd-114">親要素</span><span class="sxs-lookup"><span data-stu-id="538fd-114">Parent elements</span></span>

|<span data-ttu-id="538fd-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="538fd-115">**Element**</span></span>|<span data-ttu-id="538fd-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="538fd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="538fd-117">TimeZone (Availability)</span><span class="sxs-lookup"><span data-stu-id="538fd-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="538fd-118">要求の日付と時刻の情報を識別するコンテナー。</span><span class="sxs-lookup"><span data-stu-id="538fd-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="538fd-119">この要素には、標準時から夏時間への切り替えに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="538fd-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="538fd-120">この要素の XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="538fd-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="538fd-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="538fd-121">Text value</span></span>

<span data-ttu-id="538fd-122">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="538fd-122">A text value is required.</span></span> <span data-ttu-id="538fd-123">テキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="538fd-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="538fd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="538fd-124">Remarks</span></span>

<span data-ttu-id="538fd-125">スキーマの2番目の[バイアス](bias.md)要素は、世界協定時刻 (UTC) オフセットからのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="538fd-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="538fd-126">例</span><span class="sxs-lookup"><span data-stu-id="538fd-126">Example</span></span>

<span data-ttu-id="538fd-127">次の例は、クライアントアプリケーションの UTC から8時間のオフセットを識別する XML 要求の一部を示しています。</span><span class="sxs-lookup"><span data-stu-id="538fd-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="538fd-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="538fd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="538fd-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="538fd-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="538fd-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="538fd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="538fd-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="538fd-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="538fd-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="538fd-132">Validation File</span></span>  <br/> |<span data-ttu-id="538fd-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="538fd-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="538fd-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="538fd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="538fd-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="538fd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="538fd-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="538fd-136">See also</span></span>

- [<span data-ttu-id="538fd-137">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="538fd-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="538fd-138">バイアス</span><span class="sxs-lookup"><span data-stu-id="538fd-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="538fd-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="538fd-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

