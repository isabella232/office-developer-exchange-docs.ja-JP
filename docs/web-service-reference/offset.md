---
title: オフセット
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
description: オフセット要素は、BaseOffset からのオフセットを示します。 BaseOffset 要素とは、オフセット要素は、時間が標準または夏時間から標準時であるかどうかを識別します。
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832642"
---
# <a name="offset"></a><span data-ttu-id="91c35-104">オフセット</span><span class="sxs-lookup"><span data-stu-id="91c35-104">Offset</span></span>

<span data-ttu-id="91c35-105">**オフセット**要素は、 [BaseOffset](baseoffset.md)からのオフセットを示します。</span><span class="sxs-lookup"><span data-stu-id="91c35-105">The **Offset** element describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="91c35-106">**BaseOffset**要素と要素の**オフセット**は、時間が標準または夏時間から標準時であるかどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="91c35-106">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard or daylight saving time.</span></span> 
  
```xml
<Offset/>
```

 <span data-ttu-id="91c35-107">**duration**</span><span class="sxs-lookup"><span data-stu-id="91c35-107">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91c35-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="91c35-108">Attributes and elements</span></span>

<span data-ttu-id="91c35-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91c35-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91c35-110">属性</span><span class="sxs-lookup"><span data-stu-id="91c35-110">Attributes</span></span>

<span data-ttu-id="91c35-111">なし。</span><span class="sxs-lookup"><span data-stu-id="91c35-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91c35-112">子要素</span><span class="sxs-lookup"><span data-stu-id="91c35-112">Child elements</span></span>

<span data-ttu-id="91c35-113">なし。</span><span class="sxs-lookup"><span data-stu-id="91c35-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91c35-114">親要素</span><span class="sxs-lookup"><span data-stu-id="91c35-114">Parent elements</span></span>

|<span data-ttu-id="91c35-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="91c35-115">**Element**</span></span>|<span data-ttu-id="91c35-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="91c35-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91c35-117">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="91c35-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="91c35-118">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="91c35-118">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="91c35-119">Standard</span><span class="sxs-lookup"><span data-stu-id="91c35-119">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="91c35-120">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="91c35-120">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91c35-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="91c35-121">Text value</span></span>

<span data-ttu-id="91c35-122">テキスト値は、世界協定時刻 (UTC) からのオフセットを表します。</span><span class="sxs-lookup"><span data-stu-id="91c35-122">The text value represents the offset from Coordinated Universal Time (UTC).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91c35-123">備考</span><span class="sxs-lookup"><span data-stu-id="91c35-123">Remarks</span></span>

<span data-ttu-id="91c35-124">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="91c35-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91c35-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="91c35-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91c35-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="91c35-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91c35-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="91c35-127">Schema Name</span></span>  <br/> |<span data-ttu-id="91c35-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="91c35-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="91c35-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="91c35-129">Validation File</span></span>  <br/> |<span data-ttu-id="91c35-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91c35-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91c35-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="91c35-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="91c35-132">False</span><span class="sxs-lookup"><span data-stu-id="91c35-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91c35-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="91c35-133">See also</span></span>



- [<span data-ttu-id="91c35-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="91c35-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

