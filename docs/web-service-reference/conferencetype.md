---
title: ConferenceType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConferenceType
api_type:
- schema
ms.assetid: 6bcf6c18-2695-44b1-aabe-dadc52b2633a
description: ConferenceType 要素は、予定表アイテムで実行される会議の種類を表します。
ms.openlocfilehash: 482fc09d709e2b151b255107af59cb98de236aec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463931"
---
# <a name="conferencetype"></a><span data-ttu-id="df942-103">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="df942-103">ConferenceType</span></span>

<span data-ttu-id="df942-104">**ConferenceType**要素は、予定表アイテムで実行される会議の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="df942-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="df942-105">**int**</span><span class="sxs-lookup"><span data-stu-id="df942-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df942-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="df942-106">Attributes and elements</span></span>

<span data-ttu-id="df942-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df942-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df942-108">属性</span><span class="sxs-lookup"><span data-stu-id="df942-108">Attributes</span></span>

<span data-ttu-id="df942-109">なし。</span><span class="sxs-lookup"><span data-stu-id="df942-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df942-110">子要素</span><span class="sxs-lookup"><span data-stu-id="df942-110">Child elements</span></span>

<span data-ttu-id="df942-111">なし。</span><span class="sxs-lookup"><span data-stu-id="df942-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df942-112">親要素</span><span class="sxs-lookup"><span data-stu-id="df942-112">Parent elements</span></span>

|<span data-ttu-id="df942-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="df942-113">**Element**</span></span>|<span data-ttu-id="df942-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="df942-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df942-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="df942-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="df942-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="df942-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="df942-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="df942-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="df942-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="df942-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df942-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="df942-119">Text value</span></span>

<span data-ttu-id="df942-120">この要素を使用する場合は、整数値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="df942-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="df942-121">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="df942-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="df942-122">0 = NetMeeting</span><span class="sxs-lookup"><span data-stu-id="df942-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="df942-123">1 = NetShow</span><span class="sxs-lookup"><span data-stu-id="df942-123">1 = NetShow</span></span>
    
- <span data-ttu-id="df942-124">2 = チャット</span><span class="sxs-lookup"><span data-stu-id="df942-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="df942-125">注釈</span><span class="sxs-lookup"><span data-stu-id="df942-125">Remarks</span></span>

<span data-ttu-id="df942-126">**MeetingWorkspaceUrl**プロパティは、開催者の予定表アイテムの読み取り/書き込みが可能です。</span><span class="sxs-lookup"><span data-stu-id="df942-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="df942-127">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="df942-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="df942-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="df942-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="df942-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="df942-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df942-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="df942-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df942-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df942-131">Schema Name</span></span>  <br/> |<span data-ttu-id="df942-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="df942-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="df942-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df942-133">Validation File</span></span>  <br/> |<span data-ttu-id="df942-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="df942-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df942-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="df942-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="df942-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="df942-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df942-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="df942-137">See also</span></span>



- [<span data-ttu-id="df942-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="df942-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

