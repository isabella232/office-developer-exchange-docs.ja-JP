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
ms.openlocfilehash: 5346a65c432b8e96cb95e412e3e88fbc40ce36e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462368"
---
# <a name="originalstart"></a><span data-ttu-id="5d9e0-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="5d9e0-103">OriginalStart</span></span>

<span data-ttu-id="5d9e0-104">**Originalstart**要素は、予定表アイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="5d9e0-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="5d9e0-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d9e0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5d9e0-106">Attributes and elements</span></span>

<span data-ttu-id="5d9e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d9e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d9e0-108">Attributes</span></span>

<span data-ttu-id="5d9e0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d9e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d9e0-110">Child elements</span></span>

<span data-ttu-id="5d9e0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d9e0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5d9e0-112">Parent elements</span></span>

|<span data-ttu-id="5d9e0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d9e0-113">**Element**</span></span>|<span data-ttu-id="5d9e0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d9e0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d9e0-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5d9e0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5d9e0-116">Exchange ストア内の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d9e0-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="5d9e0-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="5d9e0-118">定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5d9e0-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="5d9e0-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="5d9e0-120">定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5d9e0-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5d9e0-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5d9e0-122">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d9e0-123">発生</span><span class="sxs-lookup"><span data-stu-id="5d9e0-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="5d9e0-124">定期的な予定表アイテムの1つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d9e0-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5d9e0-125">Text value</span></span>

<span data-ttu-id="5d9e0-126">この要素を使用する場合は、日付と時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d9e0-127">注釈</span><span class="sxs-lookup"><span data-stu-id="5d9e0-127">Remarks</span></span>

<span data-ttu-id="5d9e0-128">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5d9e0-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d9e0-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5d9e0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d9e0-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d9e0-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d9e0-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d9e0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5d9e0-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d9e0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d9e0-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d9e0-133">Validation File</span></span>  <br/> |<span data-ttu-id="5d9e0-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5d9e0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d9e0-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d9e0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d9e0-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="5d9e0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d9e0-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d9e0-137">See also</span></span>



- [<span data-ttu-id="5d9e0-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d9e0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

