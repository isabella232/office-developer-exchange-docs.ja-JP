---
title: 時間 (TimeChangeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: be12e41e-6871-4f6b-b2d4-3dfa404f9ea1
description: 時間要素では、標準時と夏時間との間の時間が変更されたときの時間について説明します。
ms.openlocfilehash: db44ef494561b75dc55c93229cec3901f04235ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839669"
---
# <a name="time-timechangetype"></a><span data-ttu-id="27363-103">時間 (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="27363-103">Time (TimeChangeType)</span></span>

<span data-ttu-id="27363-104">**時間**要素では、標準時と夏時間との間の時間が変更されたときの時間について説明します。</span><span class="sxs-lookup"><span data-stu-id="27363-104">The **Time** element describes the time when the time changes between standard time and daylight saving time.</span></span> 
  
```xml
<Time/>
```

 <span data-ttu-id="27363-105">**時間**</span><span class="sxs-lookup"><span data-stu-id="27363-105">**Time**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27363-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="27363-106">Attributes and elements</span></span>

<span data-ttu-id="27363-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27363-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27363-108">属性</span><span class="sxs-lookup"><span data-stu-id="27363-108">Attributes</span></span>

<span data-ttu-id="27363-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27363-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27363-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27363-110">Child elements</span></span>

<span data-ttu-id="27363-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27363-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27363-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27363-112">Parent elements</span></span>

|<span data-ttu-id="27363-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="27363-113">**Element**</span></span>|<span data-ttu-id="27363-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="27363-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27363-115">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="27363-115">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="27363-116">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="27363-116">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="27363-117">Standard</span><span class="sxs-lookup"><span data-stu-id="27363-117">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="27363-118">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="27363-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27363-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27363-119">Text value</span></span>

<span data-ttu-id="27363-120">テキスト値は、標準時と夏時間との間の時間が変更されたときの時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="27363-120">The text value represents the time when the time changes between standard time and daylight saving time.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="27363-121">備考</span><span class="sxs-lookup"><span data-stu-id="27363-121">Remarks</span></span>

<span data-ttu-id="27363-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="27363-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27363-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="27363-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27363-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="27363-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="27363-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27363-125">Schema Name</span></span>  <br/> |<span data-ttu-id="27363-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="27363-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="27363-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27363-127">Validation File</span></span>  <br/> |<span data-ttu-id="27363-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="27363-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="27363-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27363-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="27363-130">False</span><span class="sxs-lookup"><span data-stu-id="27363-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27363-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="27363-131">See also</span></span>



- [<span data-ttu-id="27363-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="27363-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

