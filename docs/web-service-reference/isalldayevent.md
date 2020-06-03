---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: IsAllDayEvent 要素は、予定表アイテムまたは会議出席依頼が終日イベントを表しているかどうかを示します。
ms.openlocfilehash: f0c975deecf96e94599a47ef2c33e54a7d1a80b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526537"
---
# <a name="isalldayevent"></a><span data-ttu-id="c3301-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="c3301-103">IsAllDayEvent</span></span>

<span data-ttu-id="c3301-104">**Isalldayevent**要素は、予定表アイテムまたは会議出席依頼が終日イベントを表しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c3301-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="c3301-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c3301-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3301-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c3301-106">Attributes and elements</span></span>

<span data-ttu-id="c3301-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c3301-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3301-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3301-108">Attributes</span></span>

<span data-ttu-id="c3301-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c3301-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3301-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c3301-110">Child elements</span></span>

<span data-ttu-id="c3301-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c3301-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3301-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c3301-112">Parent elements</span></span>

|<span data-ttu-id="c3301-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c3301-113">**Element**</span></span>|<span data-ttu-id="c3301-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c3301-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3301-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c3301-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c3301-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c3301-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c3301-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c3301-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c3301-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c3301-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3301-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c3301-119">Text value</span></span>

<span data-ttu-id="c3301-120">この要素が含まれている場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3301-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="c3301-121">値が**true の場合**は、アイテムが終日イベントを表していることを示します。</span><span class="sxs-lookup"><span data-stu-id="c3301-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="c3301-122">値が**false**の場合は、アイテムがユーザーの稼働時間よりも小さいことを示します。</span><span class="sxs-lookup"><span data-stu-id="c3301-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c3301-123">注釈</span><span class="sxs-lookup"><span data-stu-id="c3301-123">Remarks</span></span>

<span data-ttu-id="c3301-124">終日イベントは、メールボックスに対して定義されている稼働時間の期間にまたがって発生します。</span><span class="sxs-lookup"><span data-stu-id="c3301-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="c3301-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c3301-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3301-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c3301-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3301-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c3301-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3301-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c3301-128">Schema name</span></span>  <br/> |<span data-ttu-id="c3301-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c3301-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c3301-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c3301-130">Validation file</span></span>  <br/> |<span data-ttu-id="c3301-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c3301-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3301-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c3301-132">Can be empty</span></span>  <br/> |<span data-ttu-id="c3301-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="c3301-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c3301-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3301-134">See also</span></span>



- [<span data-ttu-id="c3301-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c3301-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

