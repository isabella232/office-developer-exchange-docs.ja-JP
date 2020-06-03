---
title: ピリオド
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: Period 要素は、タイムゾーンの特定のステージの名前、時刻オフセット、および一意識別子を定義します。
ms.openlocfilehash: a7c36a9de01fd0484a7df75de3b5525992ef7ee7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459722"
---
# <a name="period"></a><span data-ttu-id="7619c-103">ピリオド</span><span class="sxs-lookup"><span data-stu-id="7619c-103">Period</span></span>

<span data-ttu-id="7619c-104">**Period**要素は、タイムゾーンの特定のステージの名前、時刻オフセット、および一意識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="7619c-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="7619c-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="7619c-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7619c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7619c-106">Attributes and elements</span></span>

<span data-ttu-id="7619c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7619c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7619c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7619c-108">Attributes</span></span>

|<span data-ttu-id="7619c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7619c-109">**Attribute**</span></span>|<span data-ttu-id="7619c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7619c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7619c-111">バイアス</span><span class="sxs-lookup"><span data-stu-id="7619c-111">Bias</span></span>  <br/> |<span data-ttu-id="7619c-112">期間の協定世界時 (UTC) からの時間オフセットを表す xs: duration 値。</span><span class="sxs-lookup"><span data-stu-id="7619c-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="7619c-113">名前</span><span class="sxs-lookup"><span data-stu-id="7619c-113">Name</span></span>  <br/> |<span data-ttu-id="7619c-114">期間のわかりやすい名前を表す文字列型 (string) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7619c-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="7619c-115">ID</span><span class="sxs-lookup"><span data-stu-id="7619c-115">Id</span></span>  <br/> |<span data-ttu-id="7619c-116">期間の識別子を表す文字列型 (string) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7619c-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7619c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="7619c-117">Child elements</span></span>

<span data-ttu-id="7619c-118">なし。</span><span class="sxs-lookup"><span data-stu-id="7619c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7619c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7619c-119">Parent elements</span></span>

|<span data-ttu-id="7619c-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="7619c-120">**Element**</span></span>|<span data-ttu-id="7619c-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="7619c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7619c-122">Periods</span><span class="sxs-lookup"><span data-stu-id="7619c-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="7619c-123">タイムゾーンのさまざまな段階での時間オフセットを定義する期間の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="7619c-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7619c-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7619c-124">Text value</span></span>

<span data-ttu-id="7619c-125">なし。</span><span class="sxs-lookup"><span data-stu-id="7619c-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7619c-126">注釈</span><span class="sxs-lookup"><span data-stu-id="7619c-126">Remarks</span></span>

<span data-ttu-id="7619c-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7619c-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7619c-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7619c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7619c-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="7619c-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7619c-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7619c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7619c-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7619c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7619c-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7619c-132">Validation File</span></span>  <br/> |<span data-ttu-id="7619c-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7619c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7619c-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7619c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7619c-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="7619c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7619c-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="7619c-136">See also</span></span>



- [<span data-ttu-id="7619c-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7619c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

