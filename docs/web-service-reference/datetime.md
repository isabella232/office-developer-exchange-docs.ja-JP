---
title: >
  DateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DateTime
api_type:
- schema
ms.assetid: 9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4
description: DateTime 要素は、タイムゾーンの切り替えが行われる日付と時刻を表します。
ms.openlocfilehash: 109fc1107ddf59d3e8aea12b267775503ac462ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44442879"
---
# <a name="datetime"></a><span data-ttu-id="3433c-103">DateTime
</span><span class="sxs-lookup"><span data-stu-id="3433c-103">DateTime</span></span>

<span data-ttu-id="3433c-104">**DateTime**要素は、タイムゾーンの切り替えが行われる日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="3433c-104">The **DateTime** element represents the date and time at which the time zone transition occurs.</span></span> 
  
```xml
<DateTime/>
```

<span data-ttu-id="3433c-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="3433c-105">**DateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3433c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3433c-106">Attributes and elements</span></span>

<span data-ttu-id="3433c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3433c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3433c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3433c-108">Attributes</span></span>

<span data-ttu-id="3433c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3433c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3433c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3433c-110">Child elements</span></span>

<span data-ttu-id="3433c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3433c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3433c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3433c-112">Parent elements</span></span>

|<span data-ttu-id="3433c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3433c-113">**Element**</span></span>|<span data-ttu-id="3433c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3433c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3433c-115">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="3433c-115">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="3433c-116">特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="3433c-116">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3433c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3433c-117">Text value</span></span>

<span data-ttu-id="3433c-118">**DateTime**要素のテキスト値は、タイムゾーンの切り替えが発生する日付と時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="3433c-118">The text value of the **DateTime** element represents the date and time at which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3433c-119">注釈</span><span class="sxs-lookup"><span data-stu-id="3433c-119">Remarks</span></span>

<span data-ttu-id="3433c-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3433c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3433c-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3433c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3433c-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="3433c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3433c-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3433c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3433c-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3433c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3433c-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3433c-125">Validation File</span></span>  <br/> |<span data-ttu-id="3433c-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3433c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3433c-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3433c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3433c-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="3433c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3433c-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3433c-129">See also</span></span>

- [<span data-ttu-id="3433c-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3433c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

