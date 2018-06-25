---
title: TransitionsGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: TransitionsGroup 要素は、タイム ゾーンの移行の配列を表します。
ms.openlocfilehash: e5991ad7f73a1694e0d4abadd8d252acc04970e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839750"
---
# <a name="transitionsgroup"></a><span data-ttu-id="9454e-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="9454e-103">TransitionsGroup</span></span>

<span data-ttu-id="9454e-104">**TransitionsGroup**要素は、タイム ゾーンの移行の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="9454e-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="9454e-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="9454e-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9454e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9454e-106">Attributes and elements</span></span>

<span data-ttu-id="9454e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9454e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9454e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9454e-108">Attributes</span></span>

|<span data-ttu-id="9454e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9454e-109">**Attribute**</span></span>|<span data-ttu-id="9454e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9454e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9454e-111">ID</span><span class="sxs-lookup"><span data-stu-id="9454e-111">Id</span></span>  <br/> |<span data-ttu-id="9454e-112">トランジション グループの一意の識別子を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="9454e-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9454e-113">子要素</span><span class="sxs-lookup"><span data-stu-id="9454e-113">Child elements</span></span>

|<span data-ttu-id="9454e-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="9454e-114">**Element**</span></span>|<span data-ttu-id="9454e-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="9454e-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9454e-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="9454e-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="9454e-117">特定の日付と、特定の時刻に表示されるタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9454e-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="9454e-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="9454e-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="9454e-119">毎年同じ日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9454e-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="9454e-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="9454e-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="9454e-121">年の指定された日に発生するタイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="9454e-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9454e-122">親要素</span><span class="sxs-lookup"><span data-stu-id="9454e-122">Parent elements</span></span>

|<span data-ttu-id="9454e-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="9454e-123">**Element**</span></span>|<span data-ttu-id="9454e-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="9454e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9454e-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="9454e-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="9454e-126">タイム ゾーンの移行グループの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="9454e-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9454e-127">備考</span><span class="sxs-lookup"><span data-stu-id="9454e-127">Remarks</span></span>

<span data-ttu-id="9454e-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9454e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9454e-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="9454e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9454e-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="9454e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9454e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9454e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9454e-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9454e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9454e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9454e-133">Validation File</span></span>  <br/> |<span data-ttu-id="9454e-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9454e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9454e-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9454e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9454e-136">False</span><span class="sxs-lookup"><span data-stu-id="9454e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9454e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="9454e-137">See also</span></span>



- [<span data-ttu-id="9454e-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9454e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

