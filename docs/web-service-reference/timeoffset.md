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
description: TimeOffset 要素は、時間帯の切り替えについて協定世界時 (UTC) からの時間オフセットを表します。
ms.openlocfilehash: 8cfd43477f0548227204da9ebc6d7e9307786845
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460289"
---
# <a name="timeoffset"></a><span data-ttu-id="ef414-103">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef414-103">TimeOffset</span></span>

<span data-ttu-id="ef414-104">**Timeoffset**要素は、時間帯の切り替えについて協定世界時 (UTC) からの時間オフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="ef414-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="ef414-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="ef414-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef414-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ef414-106">Attributes and elements</span></span>

<span data-ttu-id="ef414-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef414-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef414-108">Attributes</span></span>

<span data-ttu-id="ef414-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ef414-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef414-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ef414-110">Child elements</span></span>

<span data-ttu-id="ef414-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ef414-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef414-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ef414-112">Parent elements</span></span>

|<span data-ttu-id="ef414-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ef414-113">**Element**</span></span>|<span data-ttu-id="ef414-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef414-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef414-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="ef414-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="ef414-116">各年に特定の日付に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="ef414-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="ef414-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="ef414-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="ef414-118">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="ef414-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef414-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ef414-119">Text value</span></span>

<span data-ttu-id="ef414-120">**Timeoffset**要素のテキスト値は、タイムゾーン遷移の UTC からの時間オフセットを指定する期間です。</span><span class="sxs-lookup"><span data-stu-id="ef414-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ef414-121">注釈</span><span class="sxs-lookup"><span data-stu-id="ef414-121">Remarks</span></span>

<span data-ttu-id="ef414-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ef414-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef414-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ef414-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef414-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef414-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef414-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef414-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ef414-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ef414-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef414-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef414-127">Validation File</span></span>  <br/> |<span data-ttu-id="ef414-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ef414-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef414-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ef414-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef414-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="ef414-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef414-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef414-131">See also</span></span>



- [<span data-ttu-id="ef414-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ef414-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

