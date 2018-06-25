---
title: タイム
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
description: タイムの要素では、期間およびタイム ゾーンを定義するための遷移を指定します。
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839712"
---
# <a name="timezonedefinition"></a><span data-ttu-id="1dca9-103">タイム</span><span class="sxs-lookup"><span data-stu-id="1dca9-103">TimeZoneDefinition</span></span>

<span data-ttu-id="1dca9-104">**タイム**の要素では、期間およびタイム ゾーンを定義するための遷移を指定します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="1dca9-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="1dca9-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dca9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1dca9-106">Attributes and elements</span></span>

<span data-ttu-id="1dca9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dca9-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dca9-108">Attributes</span></span>

|<span data-ttu-id="1dca9-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1dca9-109">**Attribute**</span></span>|<span data-ttu-id="1dca9-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dca9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1dca9-111">ID</span><span class="sxs-lookup"><span data-stu-id="1dca9-111">Id</span></span>  <br/> |<span data-ttu-id="1dca9-112">タイム ゾーンの一意の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="1dca9-113">名前</span><span class="sxs-lookup"><span data-stu-id="1dca9-113">Name</span></span>  <br/> |<span data-ttu-id="1dca9-114">タイム ゾーンのわかりやすい名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1dca9-115">子要素</span><span class="sxs-lookup"><span data-stu-id="1dca9-115">Child elements</span></span>

|<span data-ttu-id="1dca9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1dca9-116">**Element**</span></span>|<span data-ttu-id="1dca9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dca9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dca9-118">Periods</span><span class="sxs-lookup"><span data-stu-id="1dca9-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="1dca9-119">タイム ゾーンのさまざまな段階での時刻のオフセットを定義する[期間](period.md)の要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="1dca9-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="1dca9-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="1dca9-121">タイムゾーンの遷移を指定する[TransitionsGroup](transitionsgroup.md)要素の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="1dca9-122">遷移</span><span class="sxs-lookup"><span data-stu-id="1dca9-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="1dca9-123">タイム ゾーンの移行の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dca9-124">親要素</span><span class="sxs-lookup"><span data-stu-id="1dca9-124">Parent elements</span></span>

|<span data-ttu-id="1dca9-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="1dca9-125">**Element**</span></span>|<span data-ttu-id="1dca9-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="1dca9-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dca9-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="1dca9-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="1dca9-128">タイム ゾーン定義の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="1dca9-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="1dca9-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="1dca9-130">スコープの作成、更新、および Exchange Web サービス (EWS) を使用して取得するオブジェクトの DateTime プロパティを使用する既定のタイム ゾーンの定義を表します。</span><span class="sxs-lookup"><span data-stu-id="1dca9-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1dca9-131">備考</span><span class="sxs-lookup"><span data-stu-id="1dca9-131">Remarks</span></span>

<span data-ttu-id="1dca9-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1dca9-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dca9-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="1dca9-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dca9-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="1dca9-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dca9-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1dca9-135">Schema Name</span></span>  <br/> |<span data-ttu-id="1dca9-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1dca9-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dca9-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1dca9-137">Validation File</span></span>  <br/> |<span data-ttu-id="1dca9-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1dca9-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dca9-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1dca9-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dca9-140">False</span><span class="sxs-lookup"><span data-stu-id="1dca9-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dca9-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dca9-141">See also</span></span>



- [<span data-ttu-id="1dca9-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1dca9-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

