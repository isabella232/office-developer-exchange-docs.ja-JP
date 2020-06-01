---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: RecurrenceId 要素は、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。
ms.openlocfilehash: 58a379f2cffa7ff37181e93ad1c45c9752e84f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461612"
---
# <a name="recurrenceid"></a><span data-ttu-id="f73ab-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="f73ab-103">RecurrenceId</span></span>

<span data-ttu-id="f73ab-104">**RecurrenceId**要素は、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f73ab-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="f73ab-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f73ab-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f73ab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f73ab-106">Attributes and elements</span></span>

<span data-ttu-id="f73ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f73ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="f73ab-108">Attributes</span></span>

<span data-ttu-id="f73ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f73ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f73ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f73ab-110">Child elements</span></span>

<span data-ttu-id="f73ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f73ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f73ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f73ab-112">Parent elements</span></span>

|<span data-ttu-id="f73ab-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f73ab-113">**Element**</span></span>|<span data-ttu-id="f73ab-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f73ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ab-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f73ab-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f73ab-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f73ab-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f73ab-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f73ab-118">会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="f73ab-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f73ab-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f73ab-120">会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="f73ab-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f73ab-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f73ab-122">会議出席依頼の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="f73ab-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f73ab-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f73ab-124">会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f73ab-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f73ab-125">Text value</span></span>

<span data-ttu-id="f73ab-126">テキスト値は、予定表の発生を識別する日付/時刻の値を表します。</span><span class="sxs-lookup"><span data-stu-id="f73ab-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f73ab-127">注釈</span><span class="sxs-lookup"><span data-stu-id="f73ab-127">Remarks</span></span>

<span data-ttu-id="f73ab-128">このプロパティは、定期的な予定表アイテムの特定のインスタンスを識別するために、 [UID](uid.md)プロパティと共に使用されます。</span><span class="sxs-lookup"><span data-stu-id="f73ab-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f73ab-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f73ab-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f73ab-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="f73ab-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f73ab-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f73ab-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f73ab-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f73ab-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f73ab-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f73ab-133">Validation File</span></span>  <br/> |<span data-ttu-id="f73ab-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f73ab-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f73ab-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f73ab-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f73ab-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="f73ab-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f73ab-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="f73ab-137">See also</span></span>



- [<span data-ttu-id="f73ab-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f73ab-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

