---
title: 月 (タイムゾーン切り替え)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: Month 要素は、タイムゾーンの切り替えが行われる月を表します。
ms.openlocfilehash: 1fa32ea355cc3fe826f9c34b2fd147a0d8201673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467740"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="359d9-103">月 (タイムゾーン切り替え)</span><span class="sxs-lookup"><span data-stu-id="359d9-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="359d9-104">**Month**要素は、タイムゾーンの切り替えが行われる月を表します。</span><span class="sxs-lookup"><span data-stu-id="359d9-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="359d9-105">**int**</span><span class="sxs-lookup"><span data-stu-id="359d9-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="359d9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="359d9-106">Attributes and elements</span></span>

<span data-ttu-id="359d9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="359d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="359d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="359d9-108">Attributes</span></span>

<span data-ttu-id="359d9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="359d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="359d9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="359d9-110">Child elements</span></span>

<span data-ttu-id="359d9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="359d9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="359d9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="359d9-112">Parent elements</span></span>

|<span data-ttu-id="359d9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="359d9-113">**Element**</span></span>|<span data-ttu-id="359d9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="359d9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="359d9-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="359d9-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="359d9-116">各年に特定の日付に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="359d9-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="359d9-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="359d9-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="359d9-118">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="359d9-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="359d9-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="359d9-119">Text value</span></span>

<span data-ttu-id="359d9-120">テキスト値は、タイムゾーンの切り替えが行われる月を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="359d9-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="359d9-121">注釈</span><span class="sxs-lookup"><span data-stu-id="359d9-121">Remarks</span></span>

<span data-ttu-id="359d9-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="359d9-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="359d9-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="359d9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="359d9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="359d9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="359d9-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="359d9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="359d9-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="359d9-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="359d9-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="359d9-127">Validation File</span></span>  <br/> |<span data-ttu-id="359d9-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="359d9-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="359d9-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="359d9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="359d9-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="359d9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="359d9-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="359d9-131">See also</span></span>



- [<span data-ttu-id="359d9-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="359d9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

