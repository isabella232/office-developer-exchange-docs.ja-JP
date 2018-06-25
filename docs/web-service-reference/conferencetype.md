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
description: ConferenceType 要素では、予定表アイテムで実行される会議の種類について説明します。
ms.openlocfilehash: d312420606c5e1914fe321ae7c7c512f0833199c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759648"
---
# <a name="conferencetype"></a><span data-ttu-id="12e66-103">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="12e66-103">ConferenceType</span></span>

<span data-ttu-id="12e66-104">**ConferenceType**要素では、予定表アイテムで実行される会議の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="12e66-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="12e66-105">**int**</span><span class="sxs-lookup"><span data-stu-id="12e66-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12e66-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="12e66-106">Attributes and elements</span></span>

<span data-ttu-id="12e66-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12e66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12e66-108">属性</span><span class="sxs-lookup"><span data-stu-id="12e66-108">Attributes</span></span>

<span data-ttu-id="12e66-109">なし。</span><span class="sxs-lookup"><span data-stu-id="12e66-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12e66-110">子要素</span><span class="sxs-lookup"><span data-stu-id="12e66-110">Child elements</span></span>

<span data-ttu-id="12e66-111">なし。</span><span class="sxs-lookup"><span data-stu-id="12e66-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12e66-112">親要素</span><span class="sxs-lookup"><span data-stu-id="12e66-112">Parent elements</span></span>

|<span data-ttu-id="12e66-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="12e66-113">**Element**</span></span>|<span data-ttu-id="12e66-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="12e66-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12e66-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="12e66-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="12e66-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="12e66-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="12e66-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="12e66-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="12e66-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="12e66-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12e66-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="12e66-119">Text value</span></span>

<span data-ttu-id="12e66-120">整数値を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="12e66-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="12e66-121">以下は、この要素の有効な値です。</span><span class="sxs-lookup"><span data-stu-id="12e66-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="12e66-122">0 NetMeeting を =</span><span class="sxs-lookup"><span data-stu-id="12e66-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="12e66-123">1 NetShow を =</span><span class="sxs-lookup"><span data-stu-id="12e66-123">1 = NetShow</span></span>
    
- <span data-ttu-id="12e66-124">2 = チャット</span><span class="sxs-lookup"><span data-stu-id="12e66-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="12e66-125">備考</span><span class="sxs-lookup"><span data-stu-id="12e66-125">Remarks</span></span>

<span data-ttu-id="12e66-126">**MeetingWorkspaceUrl**プロパティは、開催者の予定表アイテムの読み取り-書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="12e66-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="12e66-127">会議出席依頼と出席者の予定表アイテムに対しては読み取り専用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="12e66-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="12e66-128">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="12e66-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="12e66-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="12e66-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12e66-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="12e66-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12e66-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12e66-131">Schema Name</span></span>  <br/> |<span data-ttu-id="12e66-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="12e66-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="12e66-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12e66-133">Validation File</span></span>  <br/> |<span data-ttu-id="12e66-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12e66-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12e66-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="12e66-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="12e66-136">False</span><span class="sxs-lookup"><span data-stu-id="12e66-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12e66-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="12e66-137">See also</span></span>



- [<span data-ttu-id="12e66-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="12e66-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

