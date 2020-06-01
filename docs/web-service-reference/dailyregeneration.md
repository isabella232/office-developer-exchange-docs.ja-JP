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
description: DailyRegeneration 要素は、タスクが再生成される頻度 (日単位) を表します。
ms.openlocfilehash: 518e4666031131f4a5fc80cc72c28a2110b468c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462165"
---
# <a name="dailyregeneration"></a><span data-ttu-id="806e2-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="806e2-103">DailyRegeneration</span></span>

<span data-ttu-id="806e2-104">**DailyRegeneration**要素は、タスクが再生成される頻度 (日単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="806e2-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="806e2-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="806e2-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="806e2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="806e2-106">Attributes and elements</span></span>

<span data-ttu-id="806e2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="806e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="806e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="806e2-108">Attributes</span></span>

<span data-ttu-id="806e2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="806e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="806e2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="806e2-110">Child elements</span></span>

|<span data-ttu-id="806e2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="806e2-111">**Element**</span></span>|<span data-ttu-id="806e2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="806e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="806e2-113">間隔</span><span class="sxs-lookup"><span data-stu-id="806e2-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="806e2-114">連続する2つのアイテム間の間隔を日単位で定義します。</span><span class="sxs-lookup"><span data-stu-id="806e2-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="806e2-115">この値は、1 ~ 999 の範囲にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="806e2-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="806e2-116">親要素</span><span class="sxs-lookup"><span data-stu-id="806e2-116">Parent elements</span></span>

|<span data-ttu-id="806e2-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="806e2-117">**Element**</span></span>|<span data-ttu-id="806e2-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="806e2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="806e2-119">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="806e2-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="806e2-120">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="806e2-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="806e2-121">注釈</span><span class="sxs-lookup"><span data-stu-id="806e2-121">Remarks</span></span>

<span data-ttu-id="806e2-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="806e2-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="806e2-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="806e2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="806e2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="806e2-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="806e2-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="806e2-125">Schema name</span></span>  <br/> |<span data-ttu-id="806e2-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="806e2-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="806e2-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="806e2-127">Validation file</span></span>  <br/> |<span data-ttu-id="806e2-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="806e2-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="806e2-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="806e2-129">Can be empty</span></span>  <br/> |<span data-ttu-id="806e2-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="806e2-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="806e2-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="806e2-131">See also</span></span>

- [<span data-ttu-id="806e2-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="806e2-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

