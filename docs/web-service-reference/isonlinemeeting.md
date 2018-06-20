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
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832061"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="45538-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="45538-103">IsOnlineMeeting</span></span>

<span data-ttu-id="45538-104">**IsOnlineMeeting**要素は、会議がオンラインかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="45538-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="45538-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="45538-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45538-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45538-106">Attributes and elements</span></span>

<span data-ttu-id="45538-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45538-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45538-108">属性</span><span class="sxs-lookup"><span data-stu-id="45538-108">Attributes</span></span>

<span data-ttu-id="45538-109">なし。</span><span class="sxs-lookup"><span data-stu-id="45538-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45538-110">子要素</span><span class="sxs-lookup"><span data-stu-id="45538-110">Child elements</span></span>

<span data-ttu-id="45538-111">なし。</span><span class="sxs-lookup"><span data-stu-id="45538-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="45538-112">親要素</span><span class="sxs-lookup"><span data-stu-id="45538-112">Parent elements</span></span>

|<span data-ttu-id="45538-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="45538-113">**Element**</span></span>|<span data-ttu-id="45538-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="45538-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45538-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="45538-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="45538-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="45538-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="45538-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="45538-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="45538-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="45538-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45538-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45538-119">Text value</span></span>

<span data-ttu-id="45538-120">ブール値を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="45538-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="45538-121">**True**の場合は、会議がオンラインであることを示します。</span><span class="sxs-lookup"><span data-stu-id="45538-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="45538-122">**False**の値は、会議がオンラインではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="45538-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="45538-123">備考</span><span class="sxs-lookup"><span data-stu-id="45538-123">Remarks</span></span>

<span data-ttu-id="45538-124">IsOnlineMeeting プロパティは、開催者の予定表アイテムの読み取り-書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="45538-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="45538-125">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="45538-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="45538-126">MicrosoftExchange 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="45538-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45538-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="45538-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45538-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="45538-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="45538-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45538-129">Schema name</span></span>  <br/> |<span data-ttu-id="45538-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="45538-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="45538-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45538-131">Validation file</span></span>  <br/> |<span data-ttu-id="45538-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="45538-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="45538-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="45538-133">Can be empty</span></span>  <br/> |<span data-ttu-id="45538-134">False</span><span class="sxs-lookup"><span data-stu-id="45538-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45538-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="45538-135">See also</span></span>



- [<span data-ttu-id="45538-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45538-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

