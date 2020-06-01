---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: IsOnlineMeeting 要素は、会議がオンラインかどうかを示します。
ms.openlocfilehash: d2d60c8a51ad7e03c33b57709d9173e79d162268
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460401"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="498f0-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="498f0-103">IsOnlineMeeting</span></span>

<span data-ttu-id="498f0-104">**IsOnlineMeeting**要素は、会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="498f0-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="498f0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="498f0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="498f0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="498f0-106">Attributes and elements</span></span>

<span data-ttu-id="498f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="498f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="498f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="498f0-108">Attributes</span></span>

<span data-ttu-id="498f0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="498f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="498f0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="498f0-110">Child elements</span></span>

<span data-ttu-id="498f0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="498f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="498f0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="498f0-112">Parent elements</span></span>

|<span data-ttu-id="498f0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="498f0-113">**Element**</span></span>|<span data-ttu-id="498f0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="498f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="498f0-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="498f0-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="498f0-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="498f0-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="498f0-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="498f0-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="498f0-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="498f0-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="498f0-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="498f0-119">Text value</span></span>

<span data-ttu-id="498f0-120">この要素を使用する場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="498f0-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="498f0-121">値が**true の場合**は、会議がオンラインであることを示します。</span><span class="sxs-lookup"><span data-stu-id="498f0-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="498f0-122">値が**false**の場合は、会議がオンラインになっていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="498f0-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="498f0-123">注釈</span><span class="sxs-lookup"><span data-stu-id="498f0-123">Remarks</span></span>

<span data-ttu-id="498f0-124">IsOnlineMeeting プロパティは、開催者の予定表アイテムの読み取り/書き込みが可能です。</span><span class="sxs-lookup"><span data-stu-id="498f0-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="498f0-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="498f0-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="498f0-126">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="498f0-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="498f0-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="498f0-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="498f0-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="498f0-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="498f0-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="498f0-129">Schema name</span></span>  <br/> |<span data-ttu-id="498f0-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="498f0-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="498f0-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="498f0-131">Validation file</span></span>  <br/> |<span data-ttu-id="498f0-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="498f0-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="498f0-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="498f0-133">Can be empty</span></span>  <br/> |<span data-ttu-id="498f0-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="498f0-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="498f0-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="498f0-135">See also</span></span>



- [<span data-ttu-id="498f0-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="498f0-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

