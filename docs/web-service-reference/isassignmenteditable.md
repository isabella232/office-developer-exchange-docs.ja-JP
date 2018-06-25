---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: IsAssignmentEditable 要素は、タスクの種類を表します。
ms.openlocfilehash: 91922c4d6abd4d88ac9e36dd3d4c0224fc1ee716
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831992"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="03c14-103">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="03c14-103">IsAssignmentEditable</span></span>

<span data-ttu-id="03c14-104">**IsAssignmentEditable**要素は、タスクの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="03c14-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="03c14-105">**整数**</span><span class="sxs-lookup"><span data-stu-id="03c14-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03c14-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="03c14-106">Attributes and elements</span></span>

<span data-ttu-id="03c14-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03c14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03c14-108">属性</span><span class="sxs-lookup"><span data-stu-id="03c14-108">Attributes</span></span>

<span data-ttu-id="03c14-109">なし。</span><span class="sxs-lookup"><span data-stu-id="03c14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03c14-110">子要素</span><span class="sxs-lookup"><span data-stu-id="03c14-110">Child elements</span></span>

<span data-ttu-id="03c14-111">なし。</span><span class="sxs-lookup"><span data-stu-id="03c14-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03c14-112">親要素</span><span class="sxs-lookup"><span data-stu-id="03c14-112">Parent elements</span></span>

|<span data-ttu-id="03c14-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="03c14-113">**Element**</span></span>|<span data-ttu-id="03c14-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="03c14-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03c14-115">タスク</span><span class="sxs-lookup"><span data-stu-id="03c14-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="03c14-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="03c14-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03c14-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03c14-117">Text value</span></span>

<span data-ttu-id="03c14-118">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="03c14-118">This property is read-only.</span></span> <span data-ttu-id="03c14-119">次の表は、可能な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="03c14-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="03c14-120">**値**</span><span class="sxs-lookup"><span data-stu-id="03c14-120">**Value**</span></span>|<span data-ttu-id="03c14-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="03c14-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="03c14-122">0</span><span class="sxs-lookup"><span data-stu-id="03c14-122">0</span></span>  <br/> |<span data-ttu-id="03c14-123">すべての作業項目の既定値です。</span><span class="sxs-lookup"><span data-stu-id="03c14-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="03c14-124">1</span><span class="sxs-lookup"><span data-stu-id="03c14-124">1</span></span>  <br/> |<span data-ttu-id="03c14-125">仕事の依頼です。</span><span class="sxs-lookup"><span data-stu-id="03c14-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="03c14-126">2</span><span class="sxs-lookup"><span data-stu-id="03c14-126">2</span></span>  <br/> |<span data-ttu-id="03c14-127">仕事の依頼の受信者からの仕事の承諾します。</span><span class="sxs-lookup"><span data-stu-id="03c14-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="03c14-128">3</span><span class="sxs-lookup"><span data-stu-id="03c14-128">3</span></span>  <br/> |<span data-ttu-id="03c14-129">仕事の依頼の受信者からのタスクの拒否します。</span><span class="sxs-lookup"><span data-stu-id="03c14-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="03c14-130">4</span><span class="sxs-lookup"><span data-stu-id="03c14-130">4</span></span>  <br/> |<span data-ttu-id="03c14-131">前の仕事の依頼を更新します。</span><span class="sxs-lookup"><span data-stu-id="03c14-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="03c14-132">5</span><span class="sxs-lookup"><span data-stu-id="03c14-132">5</span></span>  <br/> |<span data-ttu-id="03c14-133">使用されません。</span><span class="sxs-lookup"><span data-stu-id="03c14-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="03c14-134">備考</span><span class="sxs-lookup"><span data-stu-id="03c14-134">Remarks</span></span>

<span data-ttu-id="03c14-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="03c14-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03c14-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="03c14-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03c14-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="03c14-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="03c14-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03c14-138">Schema Name</span></span>  <br/> |<span data-ttu-id="03c14-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="03c14-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="03c14-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03c14-140">Validation File</span></span>  <br/> |<span data-ttu-id="03c14-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="03c14-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="03c14-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="03c14-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="03c14-143">False</span><span class="sxs-lookup"><span data-stu-id="03c14-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03c14-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="03c14-144">See also</span></span>



- [<span data-ttu-id="03c14-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="03c14-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

