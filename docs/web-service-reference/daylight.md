---
title: 日光
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: 夏時間要素は、時刻が標準時から夏時間に変更された日時を表します。
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457460"
---
# <a name="daylight"></a><span data-ttu-id="91c13-103">日光</span><span class="sxs-lookup"><span data-stu-id="91c13-103">Daylight</span></span>

<span data-ttu-id="91c13-104">**夏時間**要素は、時刻が標準時から夏時間に変更された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="91c13-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

<span data-ttu-id="91c13-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="91c13-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="91c13-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="91c13-106">Attributes and elements</span></span>

<span data-ttu-id="91c13-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91c13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91c13-108">属性</span><span class="sxs-lookup"><span data-stu-id="91c13-108">Attributes</span></span>

|<span data-ttu-id="91c13-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="91c13-109">**Attribute**</span></span>|<span data-ttu-id="91c13-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="91c13-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91c13-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="91c13-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="91c13-112">タイムゾーンの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="91c13-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="91c13-113">子要素</span><span class="sxs-lookup"><span data-stu-id="91c13-113">Child elements</span></span>

|<span data-ttu-id="91c13-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="91c13-114">**Element**</span></span>|<span data-ttu-id="91c13-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="91c13-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91c13-116">Offset</span><span class="sxs-lookup"><span data-stu-id="91c13-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="91c13-117">[Baseoffset](baseoffset.md)からのオフセットを記述します。</span><span class="sxs-lookup"><span data-stu-id="91c13-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="91c13-118">このオフセットに加えてベースオフセットを指定すると、標準または夏時間であるかどうかに応じて時刻が識別されます。</span><span class="sxs-lookup"><span data-stu-id="91c13-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="91c13-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="91c13-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="91c13-120">タイムゾーンの移行日パターンに関する相対的な年単位のパターンを記述します。</span><span class="sxs-lookup"><span data-stu-id="91c13-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="91c13-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="91c13-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="91c13-122">時刻が標準または夏時間から変化する日付を表します。</span><span class="sxs-lookup"><span data-stu-id="91c13-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="91c13-123">Time (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="91c13-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="91c13-124">時刻が標準時と夏時間の間に変化する時間を表します。</span><span class="sxs-lookup"><span data-stu-id="91c13-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="91c13-125">親要素</span><span class="sxs-lookup"><span data-stu-id="91c13-125">Parent elements</span></span>

|<span data-ttu-id="91c13-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="91c13-126">**Element**</span></span>|<span data-ttu-id="91c13-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="91c13-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91c13-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="91c13-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="91c13-129">会議がホストされている場所のタイムゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="91c13-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="91c13-130">注釈</span><span class="sxs-lookup"><span data-stu-id="91c13-130">Remarks</span></span>

<span data-ttu-id="91c13-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="91c13-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91c13-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="91c13-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91c13-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="91c13-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91c13-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91c13-134">Schema Name</span></span>  <br/> |<span data-ttu-id="91c13-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="91c13-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="91c13-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91c13-136">Validation File</span></span>  <br/> |<span data-ttu-id="91c13-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="91c13-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91c13-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="91c13-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="91c13-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="91c13-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91c13-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="91c13-140">See also</span></span>

- [<span data-ttu-id="91c13-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="91c13-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

