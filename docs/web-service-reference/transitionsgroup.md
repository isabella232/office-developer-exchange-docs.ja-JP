---
title: 遷移 Tionsgroup
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
description: 推移 Tionsgroup 要素は、タイムゾーンの遷移の配列を表します。
ms.openlocfilehash: 9f08dec048d410dadab9580e7886b2499d943176
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467418"
---
# <a name="transitionsgroup"></a><span data-ttu-id="d5371-103">遷移 Tionsgroup</span><span class="sxs-lookup"><span data-stu-id="d5371-103">TransitionsGroup</span></span>

<span data-ttu-id="d5371-104">**推移 Tionsgroup**要素は、タイムゾーンの遷移の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="d5371-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="d5371-105">**Arrayofstype Tionstype**</span><span class="sxs-lookup"><span data-stu-id="d5371-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5371-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d5371-106">Attributes and elements</span></span>

<span data-ttu-id="d5371-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5371-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5371-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5371-108">Attributes</span></span>

|<span data-ttu-id="d5371-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d5371-109">**Attribute**</span></span>|<span data-ttu-id="d5371-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5371-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d5371-111">ID</span><span class="sxs-lookup"><span data-stu-id="d5371-111">Id</span></span>  <br/> |<span data-ttu-id="d5371-112">遷移グループの一意の識別子を表す文字列型 (string) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5371-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d5371-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d5371-113">Child elements</span></span>

|<span data-ttu-id="d5371-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="d5371-114">**Element**</span></span>|<span data-ttu-id="d5371-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5371-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5371-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="d5371-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="d5371-117">特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="d5371-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="d5371-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="d5371-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="d5371-119">毎年同じ日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="d5371-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="d5371-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="d5371-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="d5371-121">指定した日に発生するタイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="d5371-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5371-122">親要素</span><span class="sxs-lookup"><span data-stu-id="d5371-122">Parent elements</span></span>

|<span data-ttu-id="d5371-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5371-123">**Element**</span></span>|<span data-ttu-id="d5371-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5371-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5371-125">遷移のグループ</span><span class="sxs-lookup"><span data-stu-id="d5371-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="d5371-126">タイムゾーン遷移グループの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="d5371-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5371-127">注釈</span><span class="sxs-lookup"><span data-stu-id="d5371-127">Remarks</span></span>

<span data-ttu-id="d5371-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5371-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5371-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d5371-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5371-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5371-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5371-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5371-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d5371-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d5371-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5371-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5371-133">Validation File</span></span>  <br/> |<span data-ttu-id="d5371-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d5371-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5371-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5371-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5371-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="d5371-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5371-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5371-137">See also</span></span>



- [<span data-ttu-id="d5371-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d5371-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

