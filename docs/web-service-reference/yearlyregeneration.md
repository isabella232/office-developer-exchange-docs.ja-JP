---
title: YearlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- YearlyRegeneration
api_type:
- schema
ms.assetid: 23538bca-738e-4319-944e-f459ff8a7eba
description: YearlyRegeneration 要素は、タスクが再生成される頻度 (年単位) を表します。
ms.openlocfilehash: 7a6796c433bc54d145d5a769e01f9bba46897735
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457880"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="b06c6-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="b06c6-103">YearlyRegeneration</span></span>

<span data-ttu-id="b06c6-104">**YearlyRegeneration**要素は、タスクが再生成される頻度 (年単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="b06c6-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="b06c6-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="b06c6-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b06c6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b06c6-106">Attributes and elements</span></span>

<span data-ttu-id="b06c6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b06c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b06c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="b06c6-108">Attributes</span></span>

<span data-ttu-id="b06c6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b06c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b06c6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b06c6-110">Child elements</span></span>

|<span data-ttu-id="b06c6-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b06c6-111">**Element**</span></span>|<span data-ttu-id="b06c6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b06c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b06c6-113">間隔</span><span class="sxs-lookup"><span data-stu-id="b06c6-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="b06c6-114">タスクの完了後に新しいタスクが再生成される間隔 (年単位) を定義します。</span><span class="sxs-lookup"><span data-stu-id="b06c6-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b06c6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b06c6-115">Parent elements</span></span>

|<span data-ttu-id="b06c6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b06c6-116">**Element**</span></span>|<span data-ttu-id="b06c6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b06c6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b06c6-118">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b06c6-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="b06c6-119">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b06c6-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b06c6-120">注釈</span><span class="sxs-lookup"><span data-stu-id="b06c6-120">Remarks</span></span>

<span data-ttu-id="b06c6-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b06c6-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b06c6-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b06c6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b06c6-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b06c6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b06c6-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b06c6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b06c6-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b06c6-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b06c6-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b06c6-126">Validation File</span></span>  <br/> |<span data-ttu-id="b06c6-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b06c6-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b06c6-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b06c6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="b06c6-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="b06c6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b06c6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b06c6-130">See also</span></span>

- [<span data-ttu-id="b06c6-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b06c6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

