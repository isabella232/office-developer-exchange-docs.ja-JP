---
title: NumberedRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberedRecurrence
api_type:
- schema
ms.assetid: 53746909-ef21-4764-8715-a7769b943cca
description: Number Ed繰返し要素は、定期的なアイテムの開始日と発生回数を表します。
ms.openlocfilehash: 000674e5b0bad9deea5aa4ac78d41135a922c755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465941"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="fa0aa-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="fa0aa-103">NumberedRecurrence</span></span>

<span data-ttu-id="fa0aa-104">**Number ed繰返し**要素は、定期的なアイテムの開始日と発生回数を表します。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="fa0aa-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="fa0aa-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa0aa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fa0aa-106">Attributes and elements</span></span>

<span data-ttu-id="fa0aa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa0aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa0aa-108">Attributes</span></span>

<span data-ttu-id="fa0aa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa0aa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fa0aa-110">Child elements</span></span>

|<span data-ttu-id="fa0aa-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="fa0aa-111">**Element**</span></span>|<span data-ttu-id="fa0aa-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa0aa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa0aa-113">StartDate (定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="fa0aa-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="fa0aa-114">定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fa0aa-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="fa0aa-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="fa0aa-116">定期的なアイテムの発生回数を含みます。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa0aa-117">親要素</span><span class="sxs-lookup"><span data-stu-id="fa0aa-117">Parent elements</span></span>

|<span data-ttu-id="fa0aa-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa0aa-118">**Element**</span></span>|<span data-ttu-id="fa0aa-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa0aa-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa0aa-120">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="fa0aa-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="fa0aa-121">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="fa0aa-122">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="fa0aa-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="fa0aa-123">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa0aa-124">注釈</span><span class="sxs-lookup"><span data-stu-id="fa0aa-124">Remarks</span></span>

<span data-ttu-id="fa0aa-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa0aa-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fa0aa-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa0aa-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa0aa-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa0aa-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa0aa-128">Schema name</span></span>  <br/> |<span data-ttu-id="fa0aa-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fa0aa-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa0aa-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa0aa-130">Validation file</span></span>  <br/> |<span data-ttu-id="fa0aa-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fa0aa-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa0aa-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa0aa-132">Can be empty</span></span>  <br/> |<span data-ttu-id="fa0aa-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="fa0aa-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa0aa-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa0aa-134">See also</span></span>



- [<span data-ttu-id="fa0aa-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa0aa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

