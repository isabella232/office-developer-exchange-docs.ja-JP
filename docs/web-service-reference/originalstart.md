---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: OriginalStart 要素は、予定表アイテムの元の開始時刻を表します。
ms.openlocfilehash: 9e5facb3df87ab08e05f23258abdf1767fae64e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832668"
---
# <a name="originalstart"></a><span data-ttu-id="df832-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="df832-103">OriginalStart</span></span>

<span data-ttu-id="df832-104">**OriginalStart**要素は、予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="df832-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="df832-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="df832-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df832-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="df832-106">Attributes and elements</span></span>

<span data-ttu-id="df832-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df832-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df832-108">属性</span><span class="sxs-lookup"><span data-stu-id="df832-108">Attributes</span></span>

<span data-ttu-id="df832-109">なし。</span><span class="sxs-lookup"><span data-stu-id="df832-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df832-110">子要素</span><span class="sxs-lookup"><span data-stu-id="df832-110">Child elements</span></span>

<span data-ttu-id="df832-111">なし。</span><span class="sxs-lookup"><span data-stu-id="df832-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df832-112">親要素</span><span class="sxs-lookup"><span data-stu-id="df832-112">Parent elements</span></span>

|<span data-ttu-id="df832-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="df832-113">**Element**</span></span>|<span data-ttu-id="df832-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="df832-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df832-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="df832-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="df832-116">Exchange ストア内の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="df832-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="df832-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="df832-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="df832-118">定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="df832-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="df832-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="df832-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="df832-120">定期的な予定表アイテムが最後に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="df832-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="df832-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="df832-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="df832-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="df832-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="df832-123">出現</span><span class="sxs-lookup"><span data-stu-id="df832-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="df832-124">定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="df832-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df832-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="df832-125">Text value</span></span>

<span data-ttu-id="df832-126">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="df832-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df832-127">備考</span><span class="sxs-lookup"><span data-stu-id="df832-127">Remarks</span></span>

<span data-ttu-id="df832-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="df832-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df832-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="df832-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df832-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="df832-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df832-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df832-131">Schema Name</span></span>  <br/> |<span data-ttu-id="df832-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="df832-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="df832-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df832-133">Validation File</span></span>  <br/> |<span data-ttu-id="df832-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="df832-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df832-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="df832-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="df832-136">False</span><span class="sxs-lookup"><span data-stu-id="df832-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df832-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="df832-137">See also</span></span>



- [<span data-ttu-id="df832-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="df832-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

