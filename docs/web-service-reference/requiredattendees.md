---
title: RequiredAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequiredAttendees
api_type:
- schema
ms.assetid: 422f8d44-b0eb-49ca-af0f-0e22b54c78d2
description: Requiredatthe Dees 要素は、会議に出席するために必要な出席者を表します。
ms.openlocfilehash: a67800687f24dc323c3d80e4166ca9dd34dfc4fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468293"
---
# <a name="requiredattendees"></a><span data-ttu-id="63ca0-103">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="63ca0-103">RequiredAttendees</span></span>

<span data-ttu-id="63ca0-104">**Requiredatthe Dees**要素は、会議に出席するために必要な出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="63ca0-104">The **RequiredAttendees** element represents attendees that are required to attend a meeting.</span></span> 
  
```xml
<RequiredAttendees>
   <Attendee/>
</RequiredAttendees>
```

 <span data-ttu-id="63ca0-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="63ca0-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63ca0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63ca0-106">Attributes and elements</span></span>

<span data-ttu-id="63ca0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63ca0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63ca0-108">属性</span><span class="sxs-lookup"><span data-stu-id="63ca0-108">Attributes</span></span>

<span data-ttu-id="63ca0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63ca0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63ca0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63ca0-110">Child elements</span></span>

|<span data-ttu-id="63ca0-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="63ca0-111">**Element**</span></span>|<span data-ttu-id="63ca0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63ca0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63ca0-113">出席者</span><span class="sxs-lookup"><span data-stu-id="63ca0-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="63ca0-114">会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="63ca0-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63ca0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="63ca0-115">Parent elements</span></span>

|<span data-ttu-id="63ca0-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="63ca0-116">**Element**</span></span>|<span data-ttu-id="63ca0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="63ca0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63ca0-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="63ca0-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="63ca0-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="63ca0-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="63ca0-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="63ca0-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="63ca0-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="63ca0-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63ca0-122">注釈</span><span class="sxs-lookup"><span data-stu-id="63ca0-122">Remarks</span></span>

<span data-ttu-id="63ca0-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="63ca0-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63ca0-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63ca0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63ca0-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="63ca0-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63ca0-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63ca0-126">Schema name</span></span>  <br/> |<span data-ttu-id="63ca0-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="63ca0-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="63ca0-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63ca0-128">Validation file</span></span>  <br/> |<span data-ttu-id="63ca0-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="63ca0-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63ca0-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="63ca0-130">Can be empty</span></span>  <br/> |<span data-ttu-id="63ca0-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="63ca0-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63ca0-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="63ca0-132">See also</span></span>



- [<span data-ttu-id="63ca0-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="63ca0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

