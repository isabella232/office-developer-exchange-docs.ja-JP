---
title: LastOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: LastOccurrence 要素は、定期的な予定表アイテムの最後の発生を表します。
ms.openlocfilehash: 8771bbed166cfb6fdcf4d1dfe4fa0812013e2667
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459813"
---
# <a name="lastoccurrence"></a><span data-ttu-id="9e743-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="9e743-103">LastOccurrence</span></span>

<span data-ttu-id="9e743-104">**Lastoccurrence**要素は、定期的な予定表アイテムの最後の発生を表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="9e743-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="9e743-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e743-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9e743-106">Attributes and elements</span></span>

<span data-ttu-id="9e743-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e743-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e743-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e743-108">Attributes</span></span>

<span data-ttu-id="9e743-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e743-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e743-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e743-110">Child elements</span></span>

|<span data-ttu-id="9e743-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9e743-111">**Element**</span></span>|<span data-ttu-id="9e743-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e743-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e743-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="9e743-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9e743-114">定期的な予定表アイテムの最後の発生の一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9e743-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9e743-115">開始</span><span class="sxs-lookup"><span data-stu-id="9e743-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="9e743-116">定期的な予定表アイテムの最後の発生の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9e743-117">終わり</span><span class="sxs-lookup"><span data-stu-id="9e743-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9e743-118">定期的な予定表アイテムの最後の発生の終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9e743-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="9e743-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="9e743-120">定期的な予定表アイテムが最後に発生したときの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e743-121">親要素</span><span class="sxs-lookup"><span data-stu-id="9e743-121">Parent elements</span></span>

|<span data-ttu-id="9e743-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e743-122">**Element**</span></span>|<span data-ttu-id="9e743-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e743-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e743-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9e743-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9e743-125">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9e743-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9e743-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9e743-127">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="9e743-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e743-128">注釈</span><span class="sxs-lookup"><span data-stu-id="9e743-128">Remarks</span></span>

<span data-ttu-id="9e743-129">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="9e743-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="9e743-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9e743-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e743-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9e743-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e743-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e743-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e743-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e743-133">Schema name</span></span>  <br/> |<span data-ttu-id="9e743-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9e743-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e743-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e743-135">Validation file</span></span>  <br/> |<span data-ttu-id="9e743-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9e743-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e743-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9e743-137">Can be empty</span></span>  <br/> |<span data-ttu-id="9e743-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="9e743-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e743-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e743-139">See also</span></span>



- [<span data-ttu-id="9e743-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e743-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="9e743-141">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="9e743-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

