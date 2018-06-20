---
title: AbsoluteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDate
api_type:
- schema
ms.assetid: 8bc59a26-6fe1-42e9-968c-69a94a3fb0ae
description: AbsoluteDate 要素は、標準または夏時間から標準時から時間が変更されたときの日付を表します。
ms.openlocfilehash: d14cafb08297e5be3c8620c441f8b84b46ffe53e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759360"
---
# <a name="absolutedate"></a><span data-ttu-id="04c16-103">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="04c16-103">AbsoluteDate</span></span>

<span data-ttu-id="04c16-104">**AbsoluteDate**要素は、標準または夏時間から標準時から時間が変更されたときの日付を表します。</span><span class="sxs-lookup"><span data-stu-id="04c16-104">The **AbsoluteDate** element represents the date when the time changes from standard or daylight saving time.</span></span> 
  
```xml
<AbsoluteDate/>
```

<span data-ttu-id="04c16-105">**date**</span><span class="sxs-lookup"><span data-stu-id="04c16-105">**date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="04c16-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="04c16-106">Attributes and elements</span></span>

<span data-ttu-id="04c16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04c16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04c16-108">属性</span><span class="sxs-lookup"><span data-stu-id="04c16-108">Attributes</span></span>

<span data-ttu-id="04c16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="04c16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04c16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="04c16-110">Child elements</span></span>

<span data-ttu-id="04c16-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04c16-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04c16-112">親要素</span><span class="sxs-lookup"><span data-stu-id="04c16-112">Parent elements</span></span>

|<span data-ttu-id="04c16-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="04c16-113">**Element**</span></span>|<span data-ttu-id="04c16-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="04c16-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04c16-115">Standard</span><span class="sxs-lookup"><span data-stu-id="04c16-115">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="04c16-116">日付と時刻が変更されたとき夏時間から標準時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="04c16-116">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="04c16-117">(夏時間)</span><span class="sxs-lookup"><span data-stu-id="04c16-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="04c16-118">日付と時刻が変更されたとき標準時間から夏時間への時間を表します。</span><span class="sxs-lookup"><span data-stu-id="04c16-118">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04c16-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04c16-119">Text value</span></span>

<span data-ttu-id="04c16-120">テキスト値は、標準または夏時間から標準時との間の移行が発生した日付を表します。</span><span class="sxs-lookup"><span data-stu-id="04c16-120">The text value represents the date when the shift between standard or daylight saving time occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04c16-121">備考</span><span class="sxs-lookup"><span data-stu-id="04c16-121">Remarks</span></span>

<span data-ttu-id="04c16-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="04c16-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04c16-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="04c16-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04c16-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="04c16-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04c16-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04c16-125">Schema Name</span></span>  <br/> |<span data-ttu-id="04c16-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="04c16-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="04c16-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04c16-127">Validation File</span></span>  <br/> |<span data-ttu-id="04c16-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04c16-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04c16-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04c16-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="04c16-130">False</span><span class="sxs-lookup"><span data-stu-id="04c16-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04c16-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="04c16-131">See also</span></span>

- [<span data-ttu-id="04c16-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="04c16-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)




