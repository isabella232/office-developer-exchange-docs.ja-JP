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
description: NumberedRecurrence 要素は、開始日との定期的なアイテムの数について説明します。
ms.openlocfilehash: 01fbf831fa7ff378221d4db3d873af730ac564d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832628"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="aadab-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="aadab-103">NumberedRecurrence</span></span>

<span data-ttu-id="aadab-104">**NumberedRecurrence**要素は、開始日との定期的なアイテムの数について説明します。</span><span class="sxs-lookup"><span data-stu-id="aadab-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="aadab-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="aadab-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aadab-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aadab-106">Attributes and elements</span></span>

<span data-ttu-id="aadab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aadab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aadab-108">属性</span><span class="sxs-lookup"><span data-stu-id="aadab-108">Attributes</span></span>

<span data-ttu-id="aadab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aadab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aadab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aadab-110">Child elements</span></span>

|<span data-ttu-id="aadab-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="aadab-111">**Element**</span></span>|<span data-ttu-id="aadab-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="aadab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aadab-113">開始日 (繰り返し)</span><span class="sxs-lookup"><span data-stu-id="aadab-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="aadab-114">定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="aadab-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="aadab-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="aadab-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="aadab-116">定期的なアイテムの出現回数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aadab-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aadab-117">親要素</span><span class="sxs-lookup"><span data-stu-id="aadab-117">Parent elements</span></span>

|<span data-ttu-id="aadab-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="aadab-118">**Element**</span></span>|<span data-ttu-id="aadab-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="aadab-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aadab-120">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="aadab-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="aadab-121">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aadab-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="aadab-122">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="aadab-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="aadab-123">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aadab-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aadab-124">備考</span><span class="sxs-lookup"><span data-stu-id="aadab-124">Remarks</span></span>

<span data-ttu-id="aadab-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="aadab-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aadab-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="aadab-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aadab-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="aadab-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aadab-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aadab-128">Schema name</span></span>  <br/> |<span data-ttu-id="aadab-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="aadab-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="aadab-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aadab-130">Validation file</span></span>  <br/> |<span data-ttu-id="aadab-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aadab-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aadab-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="aadab-132">Can be empty</span></span>  <br/> |<span data-ttu-id="aadab-133">False</span><span class="sxs-lookup"><span data-stu-id="aadab-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aadab-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="aadab-134">See also</span></span>



- [<span data-ttu-id="aadab-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="aadab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

