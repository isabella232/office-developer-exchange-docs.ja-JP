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
description: FirstOccurrence 要素は、定期的な予定表アイテムが最初に見つかった位置を表します。
ms.openlocfilehash: e5244e74bdd5a4b8e22c6e63811db53b46fa353a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760548"
---
# <a name="firstoccurrence"></a><span data-ttu-id="7e08c-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="7e08c-103">FirstOccurrence</span></span>

<span data-ttu-id="7e08c-104">**FirstOccurrence**要素は、定期的な予定表アイテムが最初に見つかった位置を表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="7e08c-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="7e08c-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e08c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e08c-106">Attributes and elements</span></span>

<span data-ttu-id="7e08c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e08c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e08c-108">Attributes</span></span>

<span data-ttu-id="7e08c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e08c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e08c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e08c-110">Child elements</span></span>

|<span data-ttu-id="7e08c-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e08c-111">**Element**</span></span>|<span data-ttu-id="7e08c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e08c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e08c-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="7e08c-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7e08c-114">定期的な予定表アイテムが最初に見つかった一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e08c-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7e08c-115">Start</span><span class="sxs-lookup"><span data-stu-id="7e08c-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="7e08c-116">定期的な予定表アイテムが最初に見つかった位置の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7e08c-117">終わり</span><span class="sxs-lookup"><span data-stu-id="7e08c-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7e08c-118">最初に出現した定期的な予定表アイテムの終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7e08c-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="7e08c-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="7e08c-120">定期的な予定表アイテムが最初に見つかった位置の元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e08c-121">親要素</span><span class="sxs-lookup"><span data-stu-id="7e08c-121">Parent elements</span></span>

|<span data-ttu-id="7e08c-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e08c-122">**Element**</span></span>|<span data-ttu-id="7e08c-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e08c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e08c-124">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="7e08c-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7e08c-125">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7e08c-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7e08c-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7e08c-127">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7e08c-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e08c-128">備考</span><span class="sxs-lookup"><span data-stu-id="7e08c-128">Remarks</span></span>

<span data-ttu-id="7e08c-129">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="7e08c-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="7e08c-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7e08c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e08c-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e08c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e08c-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e08c-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e08c-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e08c-133">Schema name</span></span>  <br/> |<span data-ttu-id="7e08c-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e08c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e08c-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e08c-135">Validation file</span></span>  <br/> |<span data-ttu-id="7e08c-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e08c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e08c-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e08c-137">Can be empty</span></span>  <br/> |<span data-ttu-id="7e08c-138">False</span><span class="sxs-lookup"><span data-stu-id="7e08c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e08c-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e08c-139">See also</span></span>



- [<span data-ttu-id="7e08c-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e08c-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
<span data-ttu-id="7e08c-141">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="7e08c-141">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>

