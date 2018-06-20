---
title: 月 (タイム ゾーンの切り替え)
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
description: 月要素では、タイム ゾーンの切り替えが発生する月を表します。
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832483"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="88eeb-103">月 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="88eeb-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="88eeb-104">**月**要素では、タイム ゾーンの切り替えが発生する月を表します。</span><span class="sxs-lookup"><span data-stu-id="88eeb-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="88eeb-105">**int**</span><span class="sxs-lookup"><span data-stu-id="88eeb-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88eeb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="88eeb-106">Attributes and elements</span></span>

<span data-ttu-id="88eeb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="88eeb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88eeb-108">属性</span><span class="sxs-lookup"><span data-stu-id="88eeb-108">Attributes</span></span>

<span data-ttu-id="88eeb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="88eeb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88eeb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="88eeb-110">Child elements</span></span>

<span data-ttu-id="88eeb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="88eeb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88eeb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="88eeb-112">Parent elements</span></span>

|<span data-ttu-id="88eeb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="88eeb-113">**Element**</span></span>|<span data-ttu-id="88eeb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="88eeb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88eeb-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="88eeb-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="88eeb-116">毎年特定の日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="88eeb-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="88eeb-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="88eeb-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="88eeb-118">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="88eeb-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88eeb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="88eeb-119">Text value</span></span>

<span data-ttu-id="88eeb-120">テキスト値は、タイム ゾーンの切り替えが発生する月を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="88eeb-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88eeb-121">備考</span><span class="sxs-lookup"><span data-stu-id="88eeb-121">Remarks</span></span>

<span data-ttu-id="88eeb-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="88eeb-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88eeb-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="88eeb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88eeb-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="88eeb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88eeb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="88eeb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="88eeb-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="88eeb-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="88eeb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="88eeb-127">Validation File</span></span>  <br/> |<span data-ttu-id="88eeb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88eeb-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88eeb-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="88eeb-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="88eeb-130">False</span><span class="sxs-lookup"><span data-stu-id="88eeb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88eeb-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="88eeb-131">See also</span></span>



- [<span data-ttu-id="88eeb-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="88eeb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

