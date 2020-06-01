---
title: Day
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Day
api_type:
- schema
ms.assetid: d3b2dc66-486a-41d1-bff3-606f0bf92715
description: Day 要素は、タイムゾーンの切り替えが発生する月の日付を表します。
ms.openlocfilehash: 8ee5ed2e996a6a4b84648df41faf2718784b9d30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457481"
---
# <a name="day"></a><span data-ttu-id="dcb63-103">Day</span><span class="sxs-lookup"><span data-stu-id="dcb63-103">Day</span></span>

<span data-ttu-id="dcb63-104">**Day**要素は、タイムゾーンの切り替えが発生する月の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="dcb63-104">The **Day** element represents the day of the month on which the time zone transition occurs.</span></span> 
  
```xml
<Day/>
```

<span data-ttu-id="dcb63-105">**int**</span><span class="sxs-lookup"><span data-stu-id="dcb63-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dcb63-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dcb63-106">Attributes and elements</span></span>

<span data-ttu-id="dcb63-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dcb63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcb63-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcb63-108">Attributes</span></span>

<span data-ttu-id="dcb63-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dcb63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcb63-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dcb63-110">Child elements</span></span>

<span data-ttu-id="dcb63-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dcb63-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dcb63-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dcb63-112">Parent elements</span></span>

|<span data-ttu-id="dcb63-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dcb63-113">**Element**</span></span>|<span data-ttu-id="dcb63-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dcb63-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcb63-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="dcb63-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="dcb63-116">各年に特定の日付に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="dcb63-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dcb63-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dcb63-117">Text value</span></span>

<span data-ttu-id="dcb63-118">**Day**要素のテキスト値は、タイムゾーンの切り替えが発生する月の日付を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="dcb63-118">The text value of the **Day** element is an integer that represents the day of the month on which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dcb63-119">注釈</span><span class="sxs-lookup"><span data-stu-id="dcb63-119">Remarks</span></span>

<span data-ttu-id="dcb63-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dcb63-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcb63-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dcb63-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcb63-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="dcb63-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcb63-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dcb63-123">Schema Name</span></span>  <br/> |<span data-ttu-id="dcb63-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dcb63-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="dcb63-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dcb63-125">Validation File</span></span>  <br/> |<span data-ttu-id="dcb63-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dcb63-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcb63-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dcb63-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="dcb63-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="dcb63-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcb63-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="dcb63-129">See also</span></span>

- [<span data-ttu-id="dcb63-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dcb63-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

