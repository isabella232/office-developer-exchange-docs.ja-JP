---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: DateTimePrecision 要素は、返される日付/時刻の値の精度を指定します。
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529225"
---
# <a name="datetimeprecision"></a><span data-ttu-id="05334-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="05334-103">DateTimePrecision</span></span>

<span data-ttu-id="05334-104">**DateTimePrecision**要素は、返される日付/時刻の値の精度を指定します。</span><span class="sxs-lookup"><span data-stu-id="05334-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="05334-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="05334-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="05334-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="05334-106">Attributes and elements</span></span>

<span data-ttu-id="05334-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05334-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05334-108">属性</span><span class="sxs-lookup"><span data-stu-id="05334-108">Attributes</span></span>

<span data-ttu-id="05334-109">なし</span><span class="sxs-lookup"><span data-stu-id="05334-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05334-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05334-110">Child elements</span></span>

<span data-ttu-id="05334-111">なし。</span><span class="sxs-lookup"><span data-stu-id="05334-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05334-112">親要素</span><span class="sxs-lookup"><span data-stu-id="05334-112">Parent elements</span></span>

<span data-ttu-id="05334-113">**DateTimePrecision**要素は、SOAP ヘッダーにあります。</span><span class="sxs-lookup"><span data-stu-id="05334-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="05334-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05334-114">Text value</span></span>

<span data-ttu-id="05334-115">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="05334-115">A text value is required.</span></span> <span data-ttu-id="05334-116">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="05334-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="05334-117">秒</span><span class="sxs-lookup"><span data-stu-id="05334-117">Seconds</span></span>
    
- <span data-ttu-id="05334-118">(</span><span class="sxs-lookup"><span data-stu-id="05334-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="05334-119">注釈</span><span class="sxs-lookup"><span data-stu-id="05334-119">Remarks</span></span>

<span data-ttu-id="05334-120">**DateTimePrecision**要素を "Seconds" に設定した SOAP ヘッダーを使用すると、日付/時刻の値が最も近い秒 (00:00:00) に戻されます。</span><span class="sxs-lookup"><span data-stu-id="05334-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="05334-121">"Milliseconds" が使用されている場合は、日付/時刻値が最も近いミリ秒 (00:00: 00.0000) に返されます。</span><span class="sxs-lookup"><span data-stu-id="05334-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="05334-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="05334-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="05334-123">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="05334-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05334-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="05334-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05334-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="05334-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05334-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05334-126">Schema Name</span></span>  <br/> |<span data-ttu-id="05334-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="05334-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="05334-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05334-128">Validation File</span></span>  <br/> |<span data-ttu-id="05334-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="05334-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05334-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="05334-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="05334-131">いいえ</span><span class="sxs-lookup"><span data-stu-id="05334-131">False</span></span>  <br/> |
   

