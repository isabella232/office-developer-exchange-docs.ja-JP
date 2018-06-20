---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: TimeOffset 要素は、タイム ゾーンの移行の世界協定時刻 (UTC) からの時刻のオフセットを表します。
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839677"
---
# <a name="timeoffset"></a><span data-ttu-id="44b16-103">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="44b16-103">TimeOffset</span></span>

<span data-ttu-id="44b16-104">**TimeOffset**要素は、タイム ゾーンの移行の世界協定時刻 (UTC) からの時刻のオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="44b16-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="44b16-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="44b16-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44b16-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="44b16-106">Attributes and elements</span></span>

<span data-ttu-id="44b16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="44b16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44b16-108">属性</span><span class="sxs-lookup"><span data-stu-id="44b16-108">Attributes</span></span>

<span data-ttu-id="44b16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="44b16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44b16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="44b16-110">Child elements</span></span>

<span data-ttu-id="44b16-111">なし。</span><span class="sxs-lookup"><span data-stu-id="44b16-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="44b16-112">親要素</span><span class="sxs-lookup"><span data-stu-id="44b16-112">Parent elements</span></span>

|<span data-ttu-id="44b16-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="44b16-113">**Element**</span></span>|<span data-ttu-id="44b16-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="44b16-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44b16-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="44b16-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="44b16-116">毎年特定の日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="44b16-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="44b16-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="44b16-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="44b16-118">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="44b16-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44b16-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="44b16-119">Text value</span></span>

<span data-ttu-id="44b16-120">**TimeOffset**要素のテキスト値は、タイム ゾーンの移行については、UTC からのオフセット時間を指定する期間です。</span><span class="sxs-lookup"><span data-stu-id="44b16-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="44b16-121">備考</span><span class="sxs-lookup"><span data-stu-id="44b16-121">Remarks</span></span>

<span data-ttu-id="44b16-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="44b16-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44b16-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="44b16-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44b16-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="44b16-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44b16-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="44b16-125">Schema Name</span></span>  <br/> |<span data-ttu-id="44b16-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="44b16-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="44b16-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="44b16-127">Validation File</span></span>  <br/> |<span data-ttu-id="44b16-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44b16-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44b16-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="44b16-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="44b16-130">False</span><span class="sxs-lookup"><span data-stu-id="44b16-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44b16-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="44b16-131">See also</span></span>



- [<span data-ttu-id="44b16-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="44b16-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

