---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: NetShowUrl 要素は、ブロードキャストのオンライン会議の URL を指定します。
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832519"
---
# <a name="netshowurl"></a><span data-ttu-id="91a95-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="91a95-103">NetShowUrl</span></span>

<span data-ttu-id="91a95-104">**NetShowUrl**要素は、ブロードキャストのオンライン会議の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="91a95-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="91a95-105">**string**</span><span class="sxs-lookup"><span data-stu-id="91a95-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91a95-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="91a95-106">Attributes and elements</span></span>

<span data-ttu-id="91a95-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91a95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91a95-108">属性</span><span class="sxs-lookup"><span data-stu-id="91a95-108">Attributes</span></span>

<span data-ttu-id="91a95-109">なし。</span><span class="sxs-lookup"><span data-stu-id="91a95-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91a95-110">子要素</span><span class="sxs-lookup"><span data-stu-id="91a95-110">Child elements</span></span>

<span data-ttu-id="91a95-111">なし。</span><span class="sxs-lookup"><span data-stu-id="91a95-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91a95-112">親要素</span><span class="sxs-lookup"><span data-stu-id="91a95-112">Parent elements</span></span>

|<span data-ttu-id="91a95-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="91a95-113">**Element**</span></span>|<span data-ttu-id="91a95-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="91a95-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91a95-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="91a95-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="91a95-116">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="91a95-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="91a95-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="91a95-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="91a95-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="91a95-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91a95-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="91a95-119">Text value</span></span>

<span data-ttu-id="91a95-120">URL を表す文字列値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="91a95-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91a95-121">備考</span><span class="sxs-lookup"><span data-stu-id="91a95-121">Remarks</span></span>

<span data-ttu-id="91a95-122">この NetShowUrl プロパティでは、開催者の予定表アイテムの読み取り-書き込み可能です。</span><span class="sxs-lookup"><span data-stu-id="91a95-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="91a95-123">会議出席依頼の出席者のために読み取り専用をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="91a95-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="91a95-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="91a95-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91a95-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="91a95-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91a95-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="91a95-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91a95-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91a95-127">Schema name</span></span>  <br/> |<span data-ttu-id="91a95-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="91a95-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="91a95-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91a95-129">Validation file</span></span>  <br/> |<span data-ttu-id="91a95-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91a95-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91a95-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="91a95-131">Can be empty</span></span>  <br/> |<span data-ttu-id="91a95-132">False</span><span class="sxs-lookup"><span data-stu-id="91a95-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91a95-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="91a95-133">See also</span></span>



- [<span data-ttu-id="91a95-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="91a95-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

