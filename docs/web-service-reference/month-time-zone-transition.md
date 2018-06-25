---
title: 月 (タイム ゾーンの切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: 月要素では、タイム ゾーンの切り替えが発生する月を表します。
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832483"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="34a52-103">月 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="34a52-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="34a52-104">**月**要素では、タイム ゾーンの切り替えが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="34a52-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="34a52-105">**int**</span><span class="sxs-lookup"><span data-stu-id="34a52-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34a52-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="34a52-106">Attributes and elements</span></span>

<span data-ttu-id="34a52-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="34a52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34a52-108">属性</span><span class="sxs-lookup"><span data-stu-id="34a52-108">Attributes</span></span>

<span data-ttu-id="34a52-109">なし。</span><span class="sxs-lookup"><span data-stu-id="34a52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34a52-110">子要素</span><span class="sxs-lookup"><span data-stu-id="34a52-110">Child elements</span></span>

<span data-ttu-id="34a52-111">なし。</span><span class="sxs-lookup"><span data-stu-id="34a52-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34a52-112">親要素</span><span class="sxs-lookup"><span data-stu-id="34a52-112">Parent elements</span></span>

|<span data-ttu-id="34a52-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="34a52-113">**Element**</span></span>|<span data-ttu-id="34a52-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="34a52-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34a52-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="34a52-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="34a52-116">毎年特定の日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="34a52-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="34a52-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="34a52-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="34a52-118">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="34a52-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34a52-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="34a52-119">Text value</span></span>

<span data-ttu-id="34a52-120">テキスト値は、タイム ゾーンの切り替えが発生する月を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="34a52-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34a52-121">備考</span><span class="sxs-lookup"><span data-stu-id="34a52-121">Remarks</span></span>

<span data-ttu-id="34a52-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="34a52-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34a52-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="34a52-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34a52-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="34a52-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="34a52-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="34a52-125">Schema Name</span></span>  <br/> |<span data-ttu-id="34a52-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="34a52-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="34a52-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="34a52-127">Validation File</span></span>  <br/> |<span data-ttu-id="34a52-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="34a52-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="34a52-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="34a52-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="34a52-130">False</span><span class="sxs-lookup"><span data-stu-id="34a52-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34a52-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="34a52-131">See also</span></span>



- [<span data-ttu-id="34a52-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="34a52-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

