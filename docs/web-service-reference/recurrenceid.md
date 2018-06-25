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
description: RecurrenceId 要素を使用して、定期的な予定表アイテムの特定のインスタンスを識別します。
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833005"
---
# <a name="recurrenceid"></a><span data-ttu-id="9a9ae-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="9a9ae-103">RecurrenceId</span></span>

<span data-ttu-id="9a9ae-104">**RecurrenceId**要素を使用して、定期的な予定表アイテムの特定のインスタンスを識別します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="9a9ae-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="9a9ae-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a9ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9a9ae-106">Attributes and elements</span></span>

<span data-ttu-id="9a9ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a9ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a9ae-108">Attributes</span></span>

<span data-ttu-id="9a9ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a9ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9a9ae-110">Child elements</span></span>

<span data-ttu-id="9a9ae-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a9ae-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9a9ae-112">Parent elements</span></span>

|<span data-ttu-id="9a9ae-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a9ae-113">**Element**</span></span>|<span data-ttu-id="9a9ae-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a9ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a9ae-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="9a9ae-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9a9ae-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9a9ae-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9a9ae-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9a9ae-118">会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="9a9ae-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9a9ae-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9a9ae-120">会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="9a9ae-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9a9ae-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9a9ae-122">会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="9a9ae-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9a9ae-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9a9ae-124">会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a9ae-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9a9ae-125">Text value</span></span>

<span data-ttu-id="9a9ae-126">テキスト値は、予定表アイテムを識別するための日付/時刻値を表します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a9ae-127">備考</span><span class="sxs-lookup"><span data-stu-id="9a9ae-127">Remarks</span></span>

<span data-ttu-id="9a9ae-128">このプロパティは、定期的な予定表アイテムの特定のインスタンスを識別する[UID](uid.md)プロパティを使用して使用します。</span><span class="sxs-lookup"><span data-stu-id="9a9ae-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9a9ae-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="9a9ae-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a9ae-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="9a9ae-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a9ae-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a9ae-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9a9ae-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9a9ae-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a9ae-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a9ae-133">Validation File</span></span>  <br/> |<span data-ttu-id="9a9ae-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9a9ae-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a9ae-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9a9ae-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a9ae-136">False</span><span class="sxs-lookup"><span data-stu-id="9a9ae-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a9ae-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a9ae-137">See also</span></span>



- [<span data-ttu-id="9a9ae-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9a9ae-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

