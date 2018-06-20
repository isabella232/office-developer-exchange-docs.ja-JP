---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: DateTimePrecision 要素は、返される日付と時刻の値の有効桁数を指定します。
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759918"
---
# <a name="datetimeprecision"></a><span data-ttu-id="d27ae-103">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="d27ae-103">DateTimePrecision</span></span>

<span data-ttu-id="d27ae-104">**DateTimePrecision**要素は、返される日付と時刻の値の有効桁数を指定します。</span><span class="sxs-lookup"><span data-stu-id="d27ae-104">The **DateTimePrecision** element specifies the precision for returned date/time values.</span></span> 
  
```XML
<DateTimePrecision />
```

<span data-ttu-id="d27ae-105">**DateTimePrecisionType**</span><span class="sxs-lookup"><span data-stu-id="d27ae-105">**DateTimePrecisionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d27ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d27ae-106">Attributes and elements</span></span>

<span data-ttu-id="d27ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d27ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d27ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="d27ae-108">Attributes</span></span>

<span data-ttu-id="d27ae-109">なし</span><span class="sxs-lookup"><span data-stu-id="d27ae-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d27ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d27ae-110">Child elements</span></span>

<span data-ttu-id="d27ae-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d27ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d27ae-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d27ae-112">Parent elements</span></span>

<span data-ttu-id="d27ae-113">**DateTimePrecision**要素は、SOAP ヘッダーに配置されます。</span><span class="sxs-lookup"><span data-stu-id="d27ae-113">The **DateTimePrecision** element is located in the SOAP header.</span></span> 
  
## <a name="text-value"></a><span data-ttu-id="d27ae-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d27ae-114">Text value</span></span>

<span data-ttu-id="d27ae-115">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="d27ae-115">A text value is required.</span></span> <span data-ttu-id="d27ae-116">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="d27ae-116">The following are the possible values:</span></span>
  
- <span data-ttu-id="d27ae-117">秒</span><span class="sxs-lookup"><span data-stu-id="d27ae-117">Seconds</span></span>
    
- <span data-ttu-id="d27ae-118">(ミリ秒)</span><span class="sxs-lookup"><span data-stu-id="d27ae-118">Milliseconds</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d27ae-119">備考</span><span class="sxs-lookup"><span data-stu-id="d27ae-119">Remarks</span></span>

<span data-ttu-id="d27ae-120">「秒」に設定する**DateTimePrecision**要素を使用して SOAP ヘッダーを使用すると日付/時刻値が最も近い秒に返されます (00: 00:00)。</span><span class="sxs-lookup"><span data-stu-id="d27ae-120">When a SOAP header with the **DateTimePrecision** element set to "Seconds" is used, date/time values are returned to the nearest seconds (00:00:00).</span></span> <span data-ttu-id="d27ae-121">「ミリ秒」を使用する場合の日付と時刻に最も近いミリ秒 (00:00:00.0000) の値が返されます。</span><span class="sxs-lookup"><span data-stu-id="d27ae-121">When "Milliseconds" is used, date/time values are returned to the nearest millisecond (00:00:00.0000).</span></span> 
  
<span data-ttu-id="d27ae-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d27ae-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="d27ae-123">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d27ae-123">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d27ae-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="d27ae-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d27ae-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="d27ae-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d27ae-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d27ae-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d27ae-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d27ae-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d27ae-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d27ae-128">Validation File</span></span>  <br/> |<span data-ttu-id="d27ae-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d27ae-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d27ae-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d27ae-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d27ae-131">いいえ</span><span class="sxs-lookup"><span data-stu-id="d27ae-131">False</span></span>  <br/> |
   

