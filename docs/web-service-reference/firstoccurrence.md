---
title: FirstOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstOccurrence
api_type:
- schema
ms.assetid: d6748860-ce0d-4d2e-b7e4-9ed834f1e45a
description: FirstOccurrence 要素は、定期的な予定表アイテムの最初の出現を表します。
ms.openlocfilehash: 22ee9018df1e89a3783c4dfb56aaf065b2c8ea6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466298"
---
# <a name="firstoccurrence"></a><span data-ttu-id="77787-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="77787-103">FirstOccurrence</span></span>

<span data-ttu-id="77787-104">**Firstoccurrence**要素は、定期的な予定表アイテムの最初の出現を表します。</span><span class="sxs-lookup"><span data-stu-id="77787-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="77787-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="77787-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77787-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="77787-106">Attributes and elements</span></span>

<span data-ttu-id="77787-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="77787-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77787-108">属性</span><span class="sxs-lookup"><span data-stu-id="77787-108">Attributes</span></span>

<span data-ttu-id="77787-109">なし。</span><span class="sxs-lookup"><span data-stu-id="77787-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77787-110">子要素</span><span class="sxs-lookup"><span data-stu-id="77787-110">Child elements</span></span>

|<span data-ttu-id="77787-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="77787-111">**Element**</span></span>|<span data-ttu-id="77787-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="77787-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77787-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="77787-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="77787-114">定期的な予定表アイテムのうち、最初に出現したものの一意識別子および変更キーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="77787-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77787-115">開始</span><span class="sxs-lookup"><span data-stu-id="77787-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="77787-116">定期的な予定表アイテムの最初の発生の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="77787-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77787-117">終わり</span><span class="sxs-lookup"><span data-stu-id="77787-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77787-118">定期的な予定表アイテムの最初の発生の終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="77787-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77787-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="77787-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="77787-120">定期的な予定表アイテムが最初に発生したときの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="77787-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77787-121">親要素</span><span class="sxs-lookup"><span data-stu-id="77787-121">Parent elements</span></span>

|<span data-ttu-id="77787-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="77787-122">**Element**</span></span>|<span data-ttu-id="77787-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="77787-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77787-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="77787-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="77787-125">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="77787-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77787-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="77787-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="77787-127">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="77787-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77787-128">注釈</span><span class="sxs-lookup"><span data-stu-id="77787-128">Remarks</span></span>

<span data-ttu-id="77787-129">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="77787-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="77787-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="77787-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77787-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="77787-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77787-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="77787-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77787-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="77787-133">Schema name</span></span>  <br/> |<span data-ttu-id="77787-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="77787-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="77787-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="77787-135">Validation file</span></span>  <br/> |<span data-ttu-id="77787-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="77787-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77787-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="77787-137">Can be empty</span></span>  <br/> |<span data-ttu-id="77787-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="77787-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77787-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="77787-139">See also</span></span>



- [<span data-ttu-id="77787-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="77787-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="77787-141">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="77787-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

