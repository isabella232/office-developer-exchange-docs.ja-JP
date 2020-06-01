---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: Offset 要素は、BaseOffset からのオフセットを表します。 BaseOffset 要素と共に、Offset 要素は時刻が標準時であるか夏時間であるかを識別します。
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459757"
---
# <a name="offset"></a><span data-ttu-id="6c8b2-104">Offset</span><span class="sxs-lookup"><span data-stu-id="6c8b2-104">Offset</span></span>

<span data-ttu-id="6c8b2-105">**Offset**要素は、 [baseoffset](baseoffset.md)からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="6c8b2-106">**Baseoffset**要素と共に、 **Offset**要素は時刻が標準時であるか夏時間であるかを識別します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="6c8b2-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="6c8b2-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c8b2-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c8b2-108">Attributes and elements</span></span>

<span data-ttu-id="6c8b2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c8b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c8b2-110">Attributes</span></span>

<span data-ttu-id="6c8b2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c8b2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c8b2-112">Child elements</span></span>

<span data-ttu-id="6c8b2-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c8b2-114">親要素</span><span class="sxs-lookup"><span data-stu-id="6c8b2-114">Parent elements</span></span>

|<span data-ttu-id="6c8b2-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c8b2-115">**Element**</span></span>|<span data-ttu-id="6c8b2-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c8b2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c8b2-117">日光</span><span class="sxs-lookup"><span data-stu-id="6c8b2-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="6c8b2-118">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="6c8b2-119">Standard</span><span class="sxs-lookup"><span data-stu-id="6c8b2-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="6c8b2-120">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c8b2-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6c8b2-121">Text value</span></span>

<span data-ttu-id="6c8b2-122">テキスト値は、協定世界時 (UTC) からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c8b2-123">注釈</span><span class="sxs-lookup"><span data-stu-id="6c8b2-123">Remarks</span></span>

<span data-ttu-id="6c8b2-124">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6c8b2-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c8b2-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c8b2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c8b2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c8b2-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6c8b2-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c8b2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6c8b2-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6c8b2-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6c8b2-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c8b2-129">Validation File</span></span>  <br/> |<span data-ttu-id="6c8b2-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6c8b2-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6c8b2-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c8b2-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c8b2-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c8b2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c8b2-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c8b2-133">See also</span></span>



- [<span data-ttu-id="6c8b2-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c8b2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

