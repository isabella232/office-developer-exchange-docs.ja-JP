---
title: EndDateRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateRecurrence
api_type:
- schema
ms.assetid: a5ee2504-db84-49ee-870c-cca9269f2e26
description: EndDateRecurrence 要素は、アイテムの定期的なパターンの開始日と終了日を表します。
ms.openlocfilehash: e8ae72012e5bcac8d8b2a06b6d3a9b3a7caf30d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460149"
---
# <a name="enddaterecurrence"></a><span data-ttu-id="0f4c9-103">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="0f4c9-103">EndDateRecurrence</span></span>

<span data-ttu-id="0f4c9-104">**EndDateRecurrence**要素は、アイテムの定期的なパターンの開始日と終了日を表します。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-104">The **EndDateRecurrence** element describes the start date and the end date of an item recurrence pattern.</span></span> 
  
```xml
<EndDateRecurrence>
   <StartDate/>
   <EndDate/>
</EndDateRecurrence>
```

 <span data-ttu-id="0f4c9-105">**EndDateRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="0f4c9-105">**EndDateRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f4c9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0f4c9-106">Attributes and elements</span></span>

<span data-ttu-id="0f4c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f4c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f4c9-108">Attributes</span></span>

<span data-ttu-id="0f4c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f4c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0f4c9-110">Child elements</span></span>

|<span data-ttu-id="0f4c9-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0f4c9-111">**Element**</span></span>|<span data-ttu-id="0f4c9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f4c9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f4c9-113">StartDate (定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="0f4c9-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="0f4c9-114">定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0f4c9-115">EndDate (定期的なアイテム)</span><span class="sxs-lookup"><span data-stu-id="0f4c9-115">EndDate (Recurrence)</span></span>](enddate-recurrence.md) <br/> |<span data-ttu-id="0f4c9-116">定期的な仕事または予定表アイテムの終了日を表します。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-116">Represents the end date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f4c9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0f4c9-117">Parent elements</span></span>

|<span data-ttu-id="0f4c9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="0f4c9-118">**Element**</span></span>|<span data-ttu-id="0f4c9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f4c9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f4c9-120">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="0f4c9-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="0f4c9-121">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="0f4c9-122">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="0f4c9-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="0f4c9-123">定期的なタスクの定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-123">Contains the recurrence pattern for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f4c9-124">注釈</span><span class="sxs-lookup"><span data-stu-id="0f4c9-124">Remarks</span></span>

<span data-ttu-id="0f4c9-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f4c9-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0f4c9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f4c9-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f4c9-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f4c9-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0f4c9-128">Schema name</span></span>  <br/> |<span data-ttu-id="0f4c9-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0f4c9-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f4c9-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0f4c9-130">Validation file</span></span>  <br/> |<span data-ttu-id="0f4c9-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0f4c9-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f4c9-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0f4c9-132">Can be empty</span></span>  <br/> |<span data-ttu-id="0f4c9-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="0f4c9-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f4c9-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f4c9-134">See also</span></span>



- [<span data-ttu-id="0f4c9-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0f4c9-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

