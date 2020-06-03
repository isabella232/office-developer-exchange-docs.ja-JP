---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: DailyRecurrence 要素は、予定表アイテムまたはタスクが繰り返される頻度 (日単位) を表します。
ms.openlocfilehash: d18a04ced19c87996c3a092f6668ab00c5a3f006
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462172"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="b4c8b-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b4c8b-103">DailyRecurrence</span></span>

<span data-ttu-id="b4c8b-104">**DailyRecurrence**要素は、予定表アイテムまたはタスクが繰り返される頻度 (日単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="b4c8b-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="b4c8b-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b4c8b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b4c8b-106">Attributes and elements</span></span>

<span data-ttu-id="b4c8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4c8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4c8b-108">Attributes</span></span>

<span data-ttu-id="b4c8b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4c8b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b4c8b-110">Child elements</span></span>

|<span data-ttu-id="b4c8b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b4c8b-111">**Element**</span></span>|<span data-ttu-id="b4c8b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4c8b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4c8b-113">間隔</span><span class="sxs-lookup"><span data-stu-id="b4c8b-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="b4c8b-114">連続する2つのアイテム間の間隔を日単位で定義します。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="b4c8b-115">この値は 1 ~ 999 の範囲内である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4c8b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b4c8b-116">Parent elements</span></span>

|<span data-ttu-id="b4c8b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4c8b-117">**Element**</span></span>|<span data-ttu-id="b4c8b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4c8b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4c8b-119">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b4c8b-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="b4c8b-120">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="b4c8b-121">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b4c8b-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="b4c8b-122">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4c8b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="b4c8b-123">Remarks</span></span>

<span data-ttu-id="b4c8b-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4c8b-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b4c8b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4c8b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b4c8b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4c8b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b4c8b-127">Schema name</span></span>  <br/> |<span data-ttu-id="b4c8b-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b4c8b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4c8b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b4c8b-129">Validation file</span></span>  <br/> |<span data-ttu-id="b4c8b-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b4c8b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4c8b-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b4c8b-131">Can be empty</span></span>  <br/> |<span data-ttu-id="b4c8b-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="b4c8b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4c8b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b4c8b-133">See also</span></span>

- [<span data-ttu-id="b4c8b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b4c8b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

