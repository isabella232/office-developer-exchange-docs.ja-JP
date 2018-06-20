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
description: WeeklyRegeneration 要素では、タスクが再生成される、数週間で、頻度について説明します。
ms.openlocfilehash: 36cd3cc5c180f2b2cf53708e7787d0595f518def
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840023"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="7c559-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="7c559-103">WeeklyRegeneration</span></span>

<span data-ttu-id="7c559-104">**WeeklyRegeneration**要素では、タスクが再生成される、数週間で、頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c559-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="7c559-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="7c559-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c559-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c559-106">Attributes and elements</span></span>

<span data-ttu-id="7c559-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c559-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c559-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c559-108">Attributes</span></span>

<span data-ttu-id="7c559-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c559-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c559-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c559-110">Child elements</span></span>

|<span data-ttu-id="7c559-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c559-111">**Element**</span></span>|<span data-ttu-id="7c559-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c559-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c559-113">間隔</span><span class="sxs-lookup"><span data-stu-id="7c559-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7c559-114">タスクが完了した後、新しいタスクが再生成されるために数週間、間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="7c559-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c559-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7c559-115">Parent elements</span></span>

|<span data-ttu-id="7c559-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c559-116">**Element**</span></span>|<span data-ttu-id="7c559-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c559-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c559-118">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7c559-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7c559-119">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c559-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c559-120">備考</span><span class="sxs-lookup"><span data-stu-id="7c559-120">Remarks</span></span>

<span data-ttu-id="7c559-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7c559-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c559-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c559-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c559-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c559-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c559-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c559-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7c559-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7c559-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c559-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c559-126">Validation File</span></span>  <br/> |<span data-ttu-id="7c559-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c559-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c559-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c559-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c559-129">False</span><span class="sxs-lookup"><span data-stu-id="7c559-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c559-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c559-130">See also</span></span>



- [<span data-ttu-id="7c559-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c559-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

