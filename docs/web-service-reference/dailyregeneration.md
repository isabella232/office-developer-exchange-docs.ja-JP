---
title: DailyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRegeneration
api_type:
- schema
ms.assetid: cafb57e4-c518-45e0-b565-2babd0dab1df
description: DailyRegeneration 要素では、日、タスクが再生成される頻度について説明します。
ms.openlocfilehash: 356f7fd2672b2ad87d17e597c52e9f12273ce3c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759904"
---
# <a name="dailyregeneration"></a><span data-ttu-id="b8166-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="b8166-103">DailyRegeneration</span></span>

<span data-ttu-id="b8166-104">**DailyRegeneration**要素では、日、タスクが再生成される頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8166-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="b8166-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="b8166-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b8166-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b8166-106">Attributes and elements</span></span>

<span data-ttu-id="b8166-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b8166-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8166-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8166-108">Attributes</span></span>

<span data-ttu-id="b8166-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b8166-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8166-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b8166-110">Child elements</span></span>

|<span data-ttu-id="b8166-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8166-111">**Element**</span></span>|<span data-ttu-id="b8166-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8166-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8166-113">間隔</span><span class="sxs-lookup"><span data-stu-id="b8166-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="b8166-114">差の日数、連続する 2 つの定期的なアイテムの間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="b8166-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="b8166-115">値は、1 ~ 999 の範囲である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8166-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8166-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b8166-116">Parent elements</span></span>

|<span data-ttu-id="b8166-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b8166-117">**Element**</span></span>|<span data-ttu-id="b8166-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b8166-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8166-119">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b8166-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="b8166-120">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b8166-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8166-121">備考</span><span class="sxs-lookup"><span data-stu-id="b8166-121">Remarks</span></span>

<span data-ttu-id="b8166-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b8166-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8166-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="b8166-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8166-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="b8166-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8166-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b8166-125">Schema name</span></span>  <br/> |<span data-ttu-id="b8166-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b8166-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8166-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b8166-127">Validation file</span></span>  <br/> |<span data-ttu-id="b8166-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8166-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8166-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8166-129">Can be empty</span></span>  <br/> |<span data-ttu-id="b8166-130">False</span><span class="sxs-lookup"><span data-stu-id="b8166-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8166-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="b8166-131">See also</span></span>

- [<span data-ttu-id="b8166-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b8166-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

