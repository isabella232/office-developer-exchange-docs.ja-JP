---
title: Year
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: Year 要素は、年に応じて変化するタイムゾーンを定義するために使用されます。 この要素は省略できます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: cc83f9b2137f151f3f8ef0ceaf603ec036989961
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465171"
---
# <a name="year"></a><span data-ttu-id="863da-105">Year</span><span class="sxs-lookup"><span data-stu-id="863da-105">Year</span></span>

<span data-ttu-id="863da-106">**Year**要素は、年に応じて変化するタイムゾーンを定義するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="863da-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="863da-107">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="863da-107">This element is optional.</span></span> <span data-ttu-id="863da-108">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="863da-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="863da-109">**string**</span><span class="sxs-lookup"><span data-stu-id="863da-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="863da-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="863da-110">Attributes and elements</span></span>

<span data-ttu-id="863da-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="863da-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="863da-112">属性</span><span class="sxs-lookup"><span data-stu-id="863da-112">Attributes</span></span>

<span data-ttu-id="863da-113">なし。</span><span class="sxs-lookup"><span data-stu-id="863da-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="863da-114">子要素</span><span class="sxs-lookup"><span data-stu-id="863da-114">Child elements</span></span>

<span data-ttu-id="863da-115">なし。</span><span class="sxs-lookup"><span data-stu-id="863da-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="863da-116">親要素</span><span class="sxs-lookup"><span data-stu-id="863da-116">Parent elements</span></span>

|<span data-ttu-id="863da-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="863da-117">**Element**</span></span>|<span data-ttu-id="863da-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="863da-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="863da-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="863da-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="863da-120">時間のオフセット (協定世界時 (UTC) を基準として、 [Bias (utc)](bias-utc.md)要素で表される時刻からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="863da-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="863da-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="863da-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="863da-122">夏時間が計測される地域[で、協定](bias-utc.md)世界時 (utc) からの相対時刻からのオフセットを表します (utc)。</span><span class="sxs-lookup"><span data-stu-id="863da-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="863da-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="863da-123">Text value</span></span>

<span data-ttu-id="863da-124">Year 要素は年を表す文字列を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="863da-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="863da-125">年の形式は YYYY 年です。</span><span class="sxs-lookup"><span data-stu-id="863da-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="863da-126">注釈</span><span class="sxs-lookup"><span data-stu-id="863da-126">Remarks</span></span>

<span data-ttu-id="863da-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="863da-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="863da-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="863da-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="863da-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="863da-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="863da-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="863da-130">Schema Name</span></span>  <br/> |<span data-ttu-id="863da-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="863da-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="863da-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="863da-132">Validation File</span></span>  <br/> |<span data-ttu-id="863da-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="863da-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="863da-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="863da-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="863da-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="863da-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="863da-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="863da-136">See also</span></span>

- [<span data-ttu-id="863da-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="863da-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

