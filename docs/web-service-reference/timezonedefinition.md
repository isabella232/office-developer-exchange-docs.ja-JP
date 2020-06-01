---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: TimeZoneDefinition 要素は、タイムゾーンを定義する期間と遷移を指定します。
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466067"
---
# <a name="timezonedefinition"></a><span data-ttu-id="c5c14-103">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="c5c14-103">TimeZoneDefinition</span></span>

<span data-ttu-id="c5c14-104">**TimeZoneDefinition**要素は、タイムゾーンを定義する期間と遷移を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="c5c14-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="c5c14-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5c14-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5c14-106">Attributes and elements</span></span>

<span data-ttu-id="c5c14-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5c14-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5c14-108">Attributes</span></span>

|<span data-ttu-id="c5c14-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c5c14-109">**Attribute**</span></span>|<span data-ttu-id="c5c14-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5c14-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5c14-111">ID</span><span class="sxs-lookup"><span data-stu-id="c5c14-111">Id</span></span>  <br/> |<span data-ttu-id="c5c14-112">タイムゾーンの一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="c5c14-113">名前</span><span class="sxs-lookup"><span data-stu-id="c5c14-113">Name</span></span>  <br/> |<span data-ttu-id="c5c14-114">タイムゾーンのわかりやすい名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c5c14-115">子要素</span><span class="sxs-lookup"><span data-stu-id="c5c14-115">Child elements</span></span>

|<span data-ttu-id="c5c14-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="c5c14-116">**Element**</span></span>|<span data-ttu-id="c5c14-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5c14-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c14-118">Periods</span><span class="sxs-lookup"><span data-stu-id="c5c14-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="c5c14-119">タイムゾーンのさまざまな段階での時間のオフセットを定義する[Period](period.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="c5c14-120">遷移のグループ</span><span class="sxs-lookup"><span data-stu-id="c5c14-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="c5c14-121">タイムゾーンの遷移を指定する、[推移 Tionsgroup](transitionsgroup.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="c5c14-122">切り替わる</span><span class="sxs-lookup"><span data-stu-id="c5c14-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="c5c14-123">タイムゾーンの切り替えの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5c14-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c5c14-124">Parent elements</span></span>

|<span data-ttu-id="c5c14-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5c14-125">**Element**</span></span>|<span data-ttu-id="c5c14-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5c14-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5c14-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="c5c14-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="c5c14-128">タイムゾーン定義の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="c5c14-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="c5c14-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="c5c14-130">Exchange Web サービス (EWS) を使用して作成、更新、および取得されるオブジェクトの DateTime プロパティのスコープ設定に使用される既定のタイムゾーン定義を表します。</span><span class="sxs-lookup"><span data-stu-id="c5c14-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5c14-131">注釈</span><span class="sxs-lookup"><span data-stu-id="c5c14-131">Remarks</span></span>

<span data-ttu-id="c5c14-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c5c14-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5c14-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5c14-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5c14-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5c14-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5c14-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5c14-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c5c14-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5c14-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5c14-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5c14-137">Validation File</span></span>  <br/> |<span data-ttu-id="c5c14-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5c14-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5c14-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c5c14-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5c14-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="c5c14-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5c14-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5c14-141">See also</span></span>



- [<span data-ttu-id="c5c14-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5c14-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

