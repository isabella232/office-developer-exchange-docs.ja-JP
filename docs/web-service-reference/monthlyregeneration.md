---
title: MonthlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: MonthlyRegeneration 要素では、数か月、タスクが再生成されるので、頻度について説明します。
ms.openlocfilehash: 3de8ab5a6a2134ad5c596bf2bcb073d881c89746
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832488"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="7a7e3-103">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="7a7e3-103">MonthlyRegeneration</span></span>

<span data-ttu-id="7a7e3-104">**MonthlyRegeneration**要素では、数か月、タスクが再生成されるので、頻度について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="7a7e3-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="7a7e3-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a7e3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7a7e3-106">Attributes and elements</span></span>

<span data-ttu-id="7a7e3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a7e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a7e3-108">Attributes</span></span>

<span data-ttu-id="7a7e3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a7e3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7a7e3-110">Child elements</span></span>

|<span data-ttu-id="7a7e3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a7e3-111">**Element**</span></span>|<span data-ttu-id="7a7e3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a7e3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a7e3-113">間隔</span><span class="sxs-lookup"><span data-stu-id="7a7e3-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7a7e3-114">月の連続する 2 つの定期的なアイテムとの間の間隔を定義します。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a7e3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7a7e3-115">Parent elements</span></span>

|<span data-ttu-id="7a7e3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a7e3-116">**Element**</span></span>|<span data-ttu-id="7a7e3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a7e3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a7e3-118">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7a7e3-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7a7e3-119">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a7e3-120">備考</span><span class="sxs-lookup"><span data-stu-id="7a7e3-120">Remarks</span></span>

<span data-ttu-id="7a7e3-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a7e3-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="7a7e3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a7e3-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="7a7e3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a7e3-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a7e3-124">Schema name</span></span>  <br/> |<span data-ttu-id="7a7e3-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7a7e3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a7e3-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a7e3-126">Validation file</span></span>  <br/> |<span data-ttu-id="7a7e3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a7e3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a7e3-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7a7e3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7a7e3-129">False</span><span class="sxs-lookup"><span data-stu-id="7a7e3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a7e3-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a7e3-130">See also</span></span>



- [<span data-ttu-id="7a7e3-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a7e3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

