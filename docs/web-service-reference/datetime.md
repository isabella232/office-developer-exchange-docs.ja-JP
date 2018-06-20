---
title: DateTime
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
description: DateTime の要素では、日付とタイム ゾーンの切り替えが発生する時刻を表します。
ms.openlocfilehash: e8212e375a691a00b8d830dbd34c87a8eef91e53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759916"
---
# <a name="datetime"></a><span data-ttu-id="6b411-103">DateTime</span><span class="sxs-lookup"><span data-stu-id="6b411-103">DateTime</span></span>

<span data-ttu-id="6b411-104">**DateTime**の要素では、日付とタイム ゾーンの切り替えが発生する時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6b411-104">The **DateTime** element represents the date and time at which the time zone transition occurs.</span></span> 
  
```xml
<DateTime/>
```

<span data-ttu-id="6b411-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="6b411-105">**DateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6b411-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b411-106">Attributes and elements</span></span>

<span data-ttu-id="6b411-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b411-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b411-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b411-108">Attributes</span></span>

<span data-ttu-id="6b411-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b411-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b411-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b411-110">Child elements</span></span>

<span data-ttu-id="6b411-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6b411-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b411-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6b411-112">Parent elements</span></span>

|<span data-ttu-id="6b411-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b411-113">**Element**</span></span>|<span data-ttu-id="6b411-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b411-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b411-115">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="6b411-115">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="6b411-116">特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="6b411-116">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b411-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b411-117">Text value</span></span>

<span data-ttu-id="6b411-118">**DateTime**の要素のテキスト値は、日付とタイム ゾーンの切り替えが発生する時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="6b411-118">The text value of the **DateTime** element represents the date and time at which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6b411-119">備考</span><span class="sxs-lookup"><span data-stu-id="6b411-119">Remarks</span></span>

<span data-ttu-id="6b411-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b411-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b411-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="6b411-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b411-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="6b411-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b411-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b411-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6b411-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b411-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b411-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b411-125">Validation File</span></span>  <br/> |<span data-ttu-id="6b411-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b411-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b411-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6b411-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b411-128">False</span><span class="sxs-lookup"><span data-stu-id="6b411-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b411-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b411-129">See also</span></span>

- [<span data-ttu-id="6b411-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b411-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

