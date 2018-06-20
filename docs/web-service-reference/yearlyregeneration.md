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
description: YearlyRegeneration 要素は、年間で、タスクが再生成される頻度をについて説明します。
ms.openlocfilehash: d034be1ff70e92fd5e96118b9fd1eb3033737f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840049"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="083dc-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="083dc-103">YearlyRegeneration</span></span>

<span data-ttu-id="083dc-104">**YearlyRegeneration**要素は、年間で、タスクが再生成される頻度をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="083dc-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="083dc-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="083dc-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="083dc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="083dc-106">Attributes and elements</span></span>

<span data-ttu-id="083dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="083dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="083dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="083dc-108">Attributes</span></span>

<span data-ttu-id="083dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="083dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="083dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="083dc-110">Child elements</span></span>

|<span data-ttu-id="083dc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="083dc-111">**Element**</span></span>|<span data-ttu-id="083dc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="083dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="083dc-113">間隔</span><span class="sxs-lookup"><span data-stu-id="083dc-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="083dc-114">年間で、タスクの完了後、新しいタスクが再生成される間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="083dc-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="083dc-115">親要素</span><span class="sxs-lookup"><span data-stu-id="083dc-115">Parent elements</span></span>

|<span data-ttu-id="083dc-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="083dc-116">**Element**</span></span>|<span data-ttu-id="083dc-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="083dc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="083dc-118">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="083dc-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="083dc-119">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="083dc-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="083dc-120">備考</span><span class="sxs-lookup"><span data-stu-id="083dc-120">Remarks</span></span>

<span data-ttu-id="083dc-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="083dc-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="083dc-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="083dc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="083dc-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="083dc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="083dc-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="083dc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="083dc-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="083dc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="083dc-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="083dc-126">Validation File</span></span>  <br/> |<span data-ttu-id="083dc-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="083dc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="083dc-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="083dc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="083dc-129">False</span><span class="sxs-lookup"><span data-stu-id="083dc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="083dc-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="083dc-130">See also</span></span>

- [<span data-ttu-id="083dc-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="083dc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

