---
title: Time (TimeChangeType)
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
description: Time 要素は、標準時と夏時間の間で時刻が変更された時刻を表します。
ms.openlocfilehash: c25d0bc3394fdfab42a29eab8b370bc4263618ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465738"
---
# <a name="time-timechangetype"></a><span data-ttu-id="f2669-103">Time (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="f2669-103">Time (TimeChangeType)</span></span>

<span data-ttu-id="f2669-104">**Time**要素は、標準時と夏時間の間で時刻が変更された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="f2669-104">The **Time** element describes the time when the time changes between standard time and daylight saving time.</span></span> 
  
```xml
<Time/>
```

 <span data-ttu-id="f2669-105">**Time**</span><span class="sxs-lookup"><span data-stu-id="f2669-105">**Time**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2669-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f2669-106">Attributes and elements</span></span>

<span data-ttu-id="f2669-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f2669-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2669-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2669-108">Attributes</span></span>

<span data-ttu-id="f2669-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f2669-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2669-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f2669-110">Child elements</span></span>

<span data-ttu-id="f2669-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f2669-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f2669-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f2669-112">Parent elements</span></span>

|<span data-ttu-id="f2669-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f2669-113">**Element**</span></span>|<span data-ttu-id="f2669-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f2669-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2669-115">日光</span><span class="sxs-lookup"><span data-stu-id="f2669-115">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="f2669-116">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="f2669-116">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="f2669-117">Standard</span><span class="sxs-lookup"><span data-stu-id="f2669-117">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="f2669-118">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="f2669-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f2669-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f2669-119">Text value</span></span>

<span data-ttu-id="f2669-120">Text 値は、標準時と夏時間の間で時刻が変更された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="f2669-120">The text value represents the time when the time changes between standard time and daylight saving time.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f2669-121">注釈</span><span class="sxs-lookup"><span data-stu-id="f2669-121">Remarks</span></span>

<span data-ttu-id="f2669-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f2669-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2669-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f2669-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2669-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2669-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2669-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f2669-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f2669-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f2669-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2669-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f2669-127">Validation File</span></span>  <br/> |<span data-ttu-id="f2669-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f2669-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2669-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f2669-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2669-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="f2669-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2669-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f2669-131">See also</span></span>



- [<span data-ttu-id="f2669-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f2669-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

