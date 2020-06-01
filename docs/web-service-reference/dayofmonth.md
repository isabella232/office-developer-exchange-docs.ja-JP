---
title: DayOfMonth
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: DayOfMonth 要素は、定期的なアイテムが発生する月の日付を表します。
ms.openlocfilehash: dc333a46283d5e8eba3a79f62f8c22c22f56e190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44442830"
---
# <a name="dayofmonth"></a><span data-ttu-id="ecb64-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="ecb64-103">DayOfMonth</span></span>

<span data-ttu-id="ecb64-104">**DayOfMonth**要素は、定期的なアイテムが発生する月の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="ecb64-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="ecb64-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ecb64-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ecb64-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ecb64-106">Attributes and elements</span></span>

<span data-ttu-id="ecb64-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ecb64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecb64-108">属性</span><span class="sxs-lookup"><span data-stu-id="ecb64-108">Attributes</span></span>

<span data-ttu-id="ecb64-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ecb64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecb64-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ecb64-110">Child elements</span></span>

<span data-ttu-id="ecb64-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ecb64-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecb64-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ecb64-112">Parent elements</span></span>

|<span data-ttu-id="ecb64-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ecb64-113">**Element**</span></span>|<span data-ttu-id="ecb64-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ecb64-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecb64-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ecb64-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="ecb64-116">1 年ごと。</span><span class="sxs-lookup"><span data-stu-id="ecb64-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="ecb64-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ecb64-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="ecb64-118">1 か月ごと。</span><span class="sxs-lookup"><span data-stu-id="ecb64-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ecb64-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ecb64-119">Text value</span></span>

<span data-ttu-id="ecb64-120">1 ~ 31 の範囲の整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecb64-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="ecb64-121">特定の月の場合、この値が月の日数よりも大きい場合は、その月の末日が想定されます。</span><span class="sxs-lookup"><span data-stu-id="ecb64-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ecb64-122">注釈</span><span class="sxs-lookup"><span data-stu-id="ecb64-122">Remarks</span></span>

<span data-ttu-id="ecb64-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ecb64-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecb64-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ecb64-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecb64-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ecb64-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ecb64-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ecb64-126">Schema name</span></span>  <br/> |<span data-ttu-id="ecb64-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ecb64-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ecb64-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ecb64-128">Validation file</span></span>  <br/> |<span data-ttu-id="ecb64-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ecb64-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ecb64-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ecb64-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ecb64-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="ecb64-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecb64-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="ecb64-132">See also</span></span>

- [<span data-ttu-id="ecb64-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ecb64-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

