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
description: ModifiedOccurrences 要素には、定期的な予定表アイテムの定期的なアイテムの配列が含まれています。
ms.openlocfilehash: d599e3d232bfffc5bedd37f3dae4d8b10a82ffde
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530423"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="7da39-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="7da39-103">ModifiedOccurrences</span></span>

<span data-ttu-id="7da39-104">**ModifiedOccurrences**要素には、定期的な予定表アイテムの定期的なアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7da39-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="7da39-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="7da39-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7da39-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7da39-106">Attributes and elements</span></span>

<span data-ttu-id="7da39-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7da39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da39-108">属性</span><span class="sxs-lookup"><span data-stu-id="7da39-108">Attributes</span></span>

<span data-ttu-id="7da39-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7da39-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7da39-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7da39-110">Child elements</span></span>

|<span data-ttu-id="7da39-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7da39-111">**Element**</span></span>|<span data-ttu-id="7da39-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7da39-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da39-113">発生</span><span class="sxs-lookup"><span data-stu-id="7da39-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="7da39-114">定期的な予定表アイテムの1つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7da39-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7da39-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7da39-115">Parent elements</span></span>

|<span data-ttu-id="7da39-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7da39-116">**Element**</span></span>|<span data-ttu-id="7da39-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7da39-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da39-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7da39-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7da39-119">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7da39-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7da39-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7da39-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7da39-121">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="7da39-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7da39-122">注釈</span><span class="sxs-lookup"><span data-stu-id="7da39-122">Remarks</span></span>

<span data-ttu-id="7da39-123">[Calendaritemtype](calendaritemtype.md)に示す値が指定されている場合、この要素は有効です。</span><span class="sxs-lookup"><span data-stu-id="7da39-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="7da39-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7da39-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7da39-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7da39-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7da39-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="7da39-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7da39-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7da39-127">Schema name</span></span>  <br/> |<span data-ttu-id="7da39-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7da39-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7da39-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7da39-129">Validation file</span></span>  <br/> |<span data-ttu-id="7da39-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7da39-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7da39-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7da39-131">Can be empty</span></span>  <br/> |<span data-ttu-id="7da39-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="7da39-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7da39-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7da39-133">See also</span></span>



- [<span data-ttu-id="7da39-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7da39-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

