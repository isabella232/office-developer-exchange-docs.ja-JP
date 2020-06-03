---
title: WeeklyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRegeneration
api_type:
- schema
ms.assetid: f128fdaa-ca3d-4614-8e55-f25e76a67b6c
description: WeeklyRegeneration 要素は、タスクが再生成される頻度 (週単位) を表します。
ms.openlocfilehash: dc333e051fd2213942e629a3f2764c72abfaeba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459750"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="35a71-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="35a71-103">WeeklyRegeneration</span></span>

<span data-ttu-id="35a71-104">**WeeklyRegeneration**要素は、タスクが再生成される頻度 (週単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="35a71-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="35a71-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="35a71-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35a71-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="35a71-106">Attributes and elements</span></span>

<span data-ttu-id="35a71-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="35a71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35a71-108">属性</span><span class="sxs-lookup"><span data-stu-id="35a71-108">Attributes</span></span>

<span data-ttu-id="35a71-109">なし。</span><span class="sxs-lookup"><span data-stu-id="35a71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35a71-110">子要素</span><span class="sxs-lookup"><span data-stu-id="35a71-110">Child elements</span></span>

|<span data-ttu-id="35a71-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="35a71-111">**Element**</span></span>|<span data-ttu-id="35a71-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="35a71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35a71-113">間隔</span><span class="sxs-lookup"><span data-stu-id="35a71-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="35a71-114">タスクが完了してから、新しいタスクが再生成される間隔 (週単位) を定義します。</span><span class="sxs-lookup"><span data-stu-id="35a71-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35a71-115">親要素</span><span class="sxs-lookup"><span data-stu-id="35a71-115">Parent elements</span></span>

|<span data-ttu-id="35a71-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="35a71-116">**Element**</span></span>|<span data-ttu-id="35a71-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="35a71-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35a71-118">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="35a71-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="35a71-119">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="35a71-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35a71-120">注釈</span><span class="sxs-lookup"><span data-stu-id="35a71-120">Remarks</span></span>

<span data-ttu-id="35a71-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="35a71-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35a71-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="35a71-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35a71-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="35a71-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35a71-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="35a71-124">Schema Name</span></span>  <br/> |<span data-ttu-id="35a71-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="35a71-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="35a71-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="35a71-126">Validation File</span></span>  <br/> |<span data-ttu-id="35a71-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="35a71-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35a71-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="35a71-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="35a71-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="35a71-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35a71-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="35a71-130">See also</span></span>



- [<span data-ttu-id="35a71-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="35a71-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

