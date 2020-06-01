---
title: UID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UID
api_type:
- schema
ms.assetid: b1c43c1e-b773-4dd1-9a32-32b3b8efeaf9
description: UID 要素は、予定表アイテムを一意に識別します。
ms.openlocfilehash: c2eb8d9cbb238132bdce2eedf7a41f90fcd20460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455913"
---
# <a name="uid"></a><span data-ttu-id="8bfe0-103">UID</span><span class="sxs-lookup"><span data-stu-id="8bfe0-103">UID</span></span>

<span data-ttu-id="8bfe0-104">**UID**要素は、予定表アイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-104">The **UID** element uniquely identifies a calendar item.</span></span> 
  
```xml
<UID>   </UID>
```

 <span data-ttu-id="8bfe0-105">**string**</span><span class="sxs-lookup"><span data-stu-id="8bfe0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8bfe0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8bfe0-106">Attributes and elements</span></span>

<span data-ttu-id="8bfe0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bfe0-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bfe0-108">Attributes</span></span>

<span data-ttu-id="8bfe0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8bfe0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8bfe0-110">Child elements</span></span>

<span data-ttu-id="8bfe0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8bfe0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8bfe0-112">Parent elements</span></span>

|<span data-ttu-id="8bfe0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8bfe0-113">**Element**</span></span>|<span data-ttu-id="8bfe0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8bfe0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bfe0-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8bfe0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8bfe0-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8bfe0-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8bfe0-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8bfe0-118">会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="8bfe0-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8bfe0-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8bfe0-120">会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8bfe0-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8bfe0-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="8bfe0-122">会議出席依頼の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="8bfe0-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="8bfe0-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="8bfe0-124">会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8bfe0-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8bfe0-125">Text value</span></span>

<span data-ttu-id="8bfe0-126">テキスト値は、一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="8bfe0-126">The text value represents a unique identifier.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bfe0-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8bfe0-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bfe0-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="8bfe0-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8bfe0-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8bfe0-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8bfe0-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8bfe0-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8bfe0-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8bfe0-131">Validation File</span></span>  <br/> |<span data-ttu-id="8bfe0-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8bfe0-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8bfe0-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8bfe0-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8bfe0-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="8bfe0-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8bfe0-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="8bfe0-135">See also</span></span>



- [<span data-ttu-id="8bfe0-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8bfe0-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

