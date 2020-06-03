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
description: AbsoluteDate 要素は、標準または夏時間から時刻が変更された日付を表します。
ms.openlocfilehash: 1874fea02c1eeeb41522046963e1d1b2fcea645a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461731"
---
# <a name="absolutedate"></a><span data-ttu-id="85c58-103">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="85c58-103">AbsoluteDate</span></span>

<span data-ttu-id="85c58-104">**AbsoluteDate**要素は、標準または夏時間から時刻が変更された日付を表します。</span><span class="sxs-lookup"><span data-stu-id="85c58-104">The **AbsoluteDate** element represents the date when the time changes from standard or daylight saving time.</span></span> 
  
```xml
<AbsoluteDate/>
```

<span data-ttu-id="85c58-105">**date**</span><span class="sxs-lookup"><span data-stu-id="85c58-105">**date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="85c58-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="85c58-106">Attributes and elements</span></span>

<span data-ttu-id="85c58-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="85c58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85c58-108">属性</span><span class="sxs-lookup"><span data-stu-id="85c58-108">Attributes</span></span>

<span data-ttu-id="85c58-109">なし。</span><span class="sxs-lookup"><span data-stu-id="85c58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85c58-110">子要素</span><span class="sxs-lookup"><span data-stu-id="85c58-110">Child elements</span></span>

<span data-ttu-id="85c58-111">なし。</span><span class="sxs-lookup"><span data-stu-id="85c58-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85c58-112">親要素</span><span class="sxs-lookup"><span data-stu-id="85c58-112">Parent elements</span></span>

|<span data-ttu-id="85c58-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="85c58-113">**Element**</span></span>|<span data-ttu-id="85c58-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="85c58-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85c58-115">Standard</span><span class="sxs-lookup"><span data-stu-id="85c58-115">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="85c58-116">夏時間から標準時までの時刻が変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="85c58-116">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="85c58-117">日光</span><span class="sxs-lookup"><span data-stu-id="85c58-117">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="85c58-118">時刻が標準時から夏時間に変更された日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="85c58-118">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85c58-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="85c58-119">Text value</span></span>

<span data-ttu-id="85c58-120">Text 値は、標準時または夏時間間の切り替えが行われる日付を表します。</span><span class="sxs-lookup"><span data-stu-id="85c58-120">The text value represents the date when the shift between standard or daylight saving time occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85c58-121">注釈</span><span class="sxs-lookup"><span data-stu-id="85c58-121">Remarks</span></span>

<span data-ttu-id="85c58-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="85c58-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85c58-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="85c58-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85c58-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="85c58-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85c58-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="85c58-125">Schema Name</span></span>  <br/> |<span data-ttu-id="85c58-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="85c58-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="85c58-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="85c58-127">Validation File</span></span>  <br/> |<span data-ttu-id="85c58-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="85c58-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85c58-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="85c58-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="85c58-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="85c58-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85c58-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="85c58-131">See also</span></span>

- [<span data-ttu-id="85c58-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="85c58-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)




