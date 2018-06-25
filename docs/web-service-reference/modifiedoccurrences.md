---
title: ModifiedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedOccurrences
api_type:
- schema
ms.assetid: 552932fc-b3b4-486e-8d73-32c0bb10bd68
description: ModifiedOccurrences 要素には、定期的な予定のマスター アイテムとは異なるものに変更された定期的な予定表アイテム アイテムの配列が含まれています。
ms.openlocfilehash: 53f60740bcaa2de6713e1b6a3d2874153285645a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832472"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="5cdd2-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="5cdd2-103">ModifiedOccurrences</span></span>

<span data-ttu-id="5cdd2-104">**ModifiedOccurrences**要素には、定期的な予定のマスター アイテムとは異なるものに変更された定期的な予定表アイテム アイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="5cdd2-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="5cdd2-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cdd2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5cdd2-106">Attributes and elements</span></span>

<span data-ttu-id="5cdd2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cdd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cdd2-108">Attributes</span></span>

<span data-ttu-id="5cdd2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cdd2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5cdd2-110">Child elements</span></span>

|<span data-ttu-id="5cdd2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cdd2-111">**Element**</span></span>|<span data-ttu-id="5cdd2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cdd2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cdd2-113">出現</span><span class="sxs-lookup"><span data-stu-id="5cdd2-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="5cdd2-114">定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cdd2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5cdd2-115">Parent elements</span></span>

|<span data-ttu-id="5cdd2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cdd2-116">**Element**</span></span>|<span data-ttu-id="5cdd2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cdd2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cdd2-118">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="5cdd2-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5cdd2-119">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5cdd2-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5cdd2-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5cdd2-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5cdd2-122">備考</span><span class="sxs-lookup"><span data-stu-id="5cdd2-122">Remarks</span></span>

<span data-ttu-id="5cdd2-123">この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="5cdd2-124">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cdd2-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="5cdd2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cdd2-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="5cdd2-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cdd2-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cdd2-127">Schema name</span></span>  <br/> |<span data-ttu-id="5cdd2-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5cdd2-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="5cdd2-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cdd2-129">Validation file</span></span>  <br/> |<span data-ttu-id="5cdd2-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cdd2-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cdd2-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5cdd2-131">Can be empty</span></span>  <br/> |<span data-ttu-id="5cdd2-132">False</span><span class="sxs-lookup"><span data-stu-id="5cdd2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cdd2-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cdd2-133">See also</span></span>



- [<span data-ttu-id="5cdd2-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5cdd2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

