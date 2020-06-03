---
title: Is割り当て編集可能
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
description: Is/編集可能な要素は、タスクの種類を表します。
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468055"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="9834d-103">Is割り当て編集可能</span><span class="sxs-lookup"><span data-stu-id="9834d-103">IsAssignmentEditable</span></span>

<span data-ttu-id="9834d-104">**Is/編集可能**な要素は、タスクの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="9834d-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="9834d-105">**以外**</span><span class="sxs-lookup"><span data-stu-id="9834d-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9834d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9834d-106">Attributes and elements</span></span>

<span data-ttu-id="9834d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9834d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9834d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9834d-108">Attributes</span></span>

<span data-ttu-id="9834d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9834d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9834d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9834d-110">Child elements</span></span>

<span data-ttu-id="9834d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9834d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9834d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9834d-112">Parent elements</span></span>

|<span data-ttu-id="9834d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9834d-113">**Element**</span></span>|<span data-ttu-id="9834d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9834d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9834d-115">タスク</span><span class="sxs-lookup"><span data-stu-id="9834d-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="9834d-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="9834d-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9834d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9834d-117">Text value</span></span>

<span data-ttu-id="9834d-118">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9834d-118">This property is read-only.</span></span> <span data-ttu-id="9834d-119">次の表に、使用可能な値を示します。</span><span class="sxs-lookup"><span data-stu-id="9834d-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="9834d-120">**値**</span><span class="sxs-lookup"><span data-stu-id="9834d-120">**Value**</span></span>|<span data-ttu-id="9834d-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="9834d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9834d-122">.0</span><span class="sxs-lookup"><span data-stu-id="9834d-122">0</span></span>  <br/> |<span data-ttu-id="9834d-123">すべてのタスクアイテムの既定値。</span><span class="sxs-lookup"><span data-stu-id="9834d-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="9834d-124">1 </span><span class="sxs-lookup"><span data-stu-id="9834d-124">1</span></span>  <br/> |<span data-ttu-id="9834d-125">仕事の依頼。</span><span class="sxs-lookup"><span data-stu-id="9834d-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="9834d-126">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9834d-126">2</span></span>  <br/> |<span data-ttu-id="9834d-127">タスクの依頼の受信者からのタスクの承諾。</span><span class="sxs-lookup"><span data-stu-id="9834d-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="9834d-128">1/3</span><span class="sxs-lookup"><span data-stu-id="9834d-128">3</span></span>  <br/> |<span data-ttu-id="9834d-129">仕事の依頼の受信者からのタスク declination。</span><span class="sxs-lookup"><span data-stu-id="9834d-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="9834d-130">4 </span><span class="sxs-lookup"><span data-stu-id="9834d-130">4</span></span>  <br/> |<span data-ttu-id="9834d-131">以前のタスクの依頼に対する更新。</span><span class="sxs-lookup"><span data-stu-id="9834d-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="9834d-132">5 </span><span class="sxs-lookup"><span data-stu-id="9834d-132">5</span></span>  <br/> |<span data-ttu-id="9834d-133">不使用。</span><span class="sxs-lookup"><span data-stu-id="9834d-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9834d-134">注釈</span><span class="sxs-lookup"><span data-stu-id="9834d-134">Remarks</span></span>

<span data-ttu-id="9834d-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9834d-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9834d-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9834d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9834d-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="9834d-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9834d-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9834d-138">Schema Name</span></span>  <br/> |<span data-ttu-id="9834d-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9834d-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9834d-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9834d-140">Validation File</span></span>  <br/> |<span data-ttu-id="9834d-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9834d-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9834d-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9834d-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="9834d-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="9834d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9834d-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9834d-144">See also</span></span>



- [<span data-ttu-id="9834d-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9834d-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

