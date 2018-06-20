---
title: Year/年
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
description: Year 要素を使用して、年によって変更されるタイム ゾーンを定義します。 この要素はオプションです。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 95d75f9c6166fc26e86534346fb07292a7fb3dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840053"
---
# <a name="year"></a><span data-ttu-id="d9739-105">Year/年</span><span class="sxs-lookup"><span data-stu-id="d9739-105">Year</span></span>

<span data-ttu-id="d9739-106">**Year**要素を使用して、年によって変更されるタイム ゾーンを定義します。</span><span class="sxs-lookup"><span data-stu-id="d9739-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="d9739-107">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="d9739-107">This element is optional.</span></span> <span data-ttu-id="d9739-108">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d9739-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="d9739-109">**string**</span><span class="sxs-lookup"><span data-stu-id="d9739-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d9739-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d9739-110">Attributes and elements</span></span>

<span data-ttu-id="d9739-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9739-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9739-112">属性</span><span class="sxs-lookup"><span data-stu-id="d9739-112">Attributes</span></span>

<span data-ttu-id="d9739-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d9739-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9739-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d9739-114">Child elements</span></span>

<span data-ttu-id="d9739-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d9739-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9739-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d9739-116">Parent elements</span></span>

|<span data-ttu-id="d9739-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9739-117">**Element**</span></span>|<span data-ttu-id="d9739-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9739-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9739-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="d9739-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="d9739-120">基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="d9739-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="d9739-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="d9739-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="d9739-122">基準にして世界協定時刻 (UTC) 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="d9739-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9739-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d9739-123">Text value</span></span>

<span data-ttu-id="d9739-124">年の要素は、1 年を表す文字列を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="d9739-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="d9739-125">年の形式は、YYYY です。</span><span class="sxs-lookup"><span data-stu-id="d9739-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9739-126">備考</span><span class="sxs-lookup"><span data-stu-id="d9739-126">Remarks</span></span>

<span data-ttu-id="d9739-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d9739-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9739-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="d9739-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9739-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="d9739-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9739-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9739-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d9739-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9739-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9739-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9739-132">Validation File</span></span>  <br/> |<span data-ttu-id="d9739-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9739-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9739-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9739-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9739-135">False</span><span class="sxs-lookup"><span data-stu-id="d9739-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9739-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9739-136">See also</span></span>

- [<span data-ttu-id="d9739-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9739-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

