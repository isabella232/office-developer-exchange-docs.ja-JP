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
description: ピリオド要素は、タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。
ms.openlocfilehash: 3b5d5877e6d9baffdfe536a0feec3b25b6d2883f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832726"
---
# <a name="period"></a><span data-ttu-id="ace96-103">ピリオド</span><span class="sxs-lookup"><span data-stu-id="ace96-103">Period</span></span>

<span data-ttu-id="ace96-104">**期間**要素は、タイム ゾーンの特定の段階の名前、時間のオフセット、および一意の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="ace96-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="ace96-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="ace96-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ace96-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ace96-106">Attributes and elements</span></span>

<span data-ttu-id="ace96-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ace96-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ace96-108">属性</span><span class="sxs-lookup"><span data-stu-id="ace96-108">Attributes</span></span>

|<span data-ttu-id="ace96-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ace96-109">**Attribute**</span></span>|<span data-ttu-id="ace96-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ace96-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ace96-111">Bias</span><span class="sxs-lookup"><span data-stu-id="ace96-111">Bias</span></span>  <br/> |<span data-ttu-id="ace96-112">期間の世界協定時刻 (UTC) からの時間のオフセットを表す文字列型 (xs:duration) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ace96-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="ace96-113">名前</span><span class="sxs-lookup"><span data-stu-id="ace96-113">Name</span></span>  <br/> |<span data-ttu-id="ace96-114">期間のわかりやすい名前を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="ace96-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="ace96-115">ID</span><span class="sxs-lookup"><span data-stu-id="ace96-115">Id</span></span>  <br/> |<span data-ttu-id="ace96-116">期間の識別子を表す文字列値。</span><span class="sxs-lookup"><span data-stu-id="ace96-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ace96-117">子要素</span><span class="sxs-lookup"><span data-stu-id="ace96-117">Child elements</span></span>

<span data-ttu-id="ace96-118">なし。</span><span class="sxs-lookup"><span data-stu-id="ace96-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ace96-119">親要素</span><span class="sxs-lookup"><span data-stu-id="ace96-119">Parent elements</span></span>

|<span data-ttu-id="ace96-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="ace96-120">**Element**</span></span>|<span data-ttu-id="ace96-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="ace96-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ace96-122">Periods</span><span class="sxs-lookup"><span data-stu-id="ace96-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="ace96-123">タイム ゾーンのさまざまな段階での時刻のオフセットを定義する期間の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="ace96-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ace96-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ace96-124">Text value</span></span>

<span data-ttu-id="ace96-125">なし。</span><span class="sxs-lookup"><span data-stu-id="ace96-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ace96-126">備考</span><span class="sxs-lookup"><span data-stu-id="ace96-126">Remarks</span></span>

<span data-ttu-id="ace96-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ace96-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ace96-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="ace96-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ace96-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="ace96-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ace96-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ace96-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ace96-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ace96-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ace96-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ace96-132">Validation File</span></span>  <br/> |<span data-ttu-id="ace96-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ace96-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ace96-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ace96-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ace96-135">False</span><span class="sxs-lookup"><span data-stu-id="ace96-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ace96-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ace96-136">See also</span></span>



- [<span data-ttu-id="ace96-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ace96-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

