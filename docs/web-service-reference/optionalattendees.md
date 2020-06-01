---
title: OptionalAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OptionalAttendees
api_type:
- schema
ms.assetid: e7c80c4d-3794-45e9-986f-6a8a687df0a4
description: 省略できる出席者要素は、会議に出席する必要がない出席者を表します。
ms.openlocfilehash: 9eeff7151042f26fe5b00b43ec16a27946680a9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468174"
---
# <a name="optionalattendees"></a><span data-ttu-id="cd263-103">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="cd263-103">OptionalAttendees</span></span>

<span data-ttu-id="cd263-104">省略できる**出席者**要素は、会議に出席する必要がない出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="cd263-104">The **OptionalAttendees** element represents attendees who are not required to attend a meeting.</span></span> 
  
```xml
<OptionalAttendees>
   <Attendee/>
</OptionalAttendees>
```

 <span data-ttu-id="cd263-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="cd263-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd263-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cd263-106">Attributes and elements</span></span>

<span data-ttu-id="cd263-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cd263-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd263-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd263-108">Attributes</span></span>

<span data-ttu-id="cd263-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cd263-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd263-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cd263-110">Child elements</span></span>

|<span data-ttu-id="cd263-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="cd263-111">**Element**</span></span>|<span data-ttu-id="cd263-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cd263-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd263-113">出席者</span><span class="sxs-lookup"><span data-stu-id="cd263-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="cd263-114">会議の出席者とリソースを表します。</span><span class="sxs-lookup"><span data-stu-id="cd263-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd263-115">親要素</span><span class="sxs-lookup"><span data-stu-id="cd263-115">Parent elements</span></span>

|<span data-ttu-id="cd263-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cd263-116">**Element**</span></span>|<span data-ttu-id="cd263-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cd263-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd263-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="cd263-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="cd263-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="cd263-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="cd263-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="cd263-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="cd263-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="cd263-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd263-122">注釈</span><span class="sxs-lookup"><span data-stu-id="cd263-122">Remarks</span></span>

<span data-ttu-id="cd263-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cd263-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd263-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cd263-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd263-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd263-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd263-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cd263-126">Schema name</span></span>  <br/> |<span data-ttu-id="cd263-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cd263-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd263-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cd263-128">Validation file</span></span>  <br/> |<span data-ttu-id="cd263-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cd263-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd263-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd263-130">Can be empty</span></span>  <br/> |<span data-ttu-id="cd263-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="cd263-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd263-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="cd263-132">See also</span></span>



- [<span data-ttu-id="cd263-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cd263-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

