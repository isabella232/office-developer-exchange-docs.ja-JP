---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: 達成率の要素は、タスクの完了状態を表します。
ms.openlocfilehash: b7dd2f18bd3ef6addeb6d3a7b004510f35b9cb3d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456886"
---
# <a name="percentcomplete"></a><span data-ttu-id="dd7d6-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="dd7d6-103">PercentComplete</span></span>

<span data-ttu-id="dd7d6-104">**達成**率の要素は、タスクの完了状態を表します。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="dd7d6-105">**再度**</span><span class="sxs-lookup"><span data-stu-id="dd7d6-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd7d6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dd7d6-106">Attributes and elements</span></span>

<span data-ttu-id="dd7d6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd7d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd7d6-108">Attributes</span></span>

<span data-ttu-id="dd7d6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd7d6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd7d6-110">Child elements</span></span>

<span data-ttu-id="dd7d6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd7d6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd7d6-112">Parent elements</span></span>

|<span data-ttu-id="dd7d6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd7d6-113">**Element**</span></span>|<span data-ttu-id="dd7d6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd7d6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd7d6-115">タスク</span><span class="sxs-lookup"><span data-stu-id="dd7d6-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="dd7d6-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd7d6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dd7d6-117">Text value</span></span>

<span data-ttu-id="dd7d6-118">0 ~ 100 の整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd7d6-119">注釈</span><span class="sxs-lookup"><span data-stu-id="dd7d6-119">Remarks</span></span>

<span data-ttu-id="dd7d6-120">**達成**率を100に設定すると、 [completedate](completedate.md)要素を設定するか、 [Status](status.md)要素を**Completed**に設定した場合と同じ結果になります。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="dd7d6-121">これらのプロパティの少なくとも2つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定されている値が決まります。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="dd7d6-122">たとえば、**達成**率が100、 [completedate](completedate.md)が2007、[状態](status.md)が NotStarted で、プロパティがこの順序でストリーミングされている場合は、タスクの[状態](status.md)を NotStarted に、 [completedate](completedate.md)は**null**、**達成**率を0に設定することになります。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="dd7d6-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="dd7d6-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd7d6-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dd7d6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd7d6-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd7d6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd7d6-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd7d6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="dd7d6-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dd7d6-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd7d6-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd7d6-128">Validation File</span></span>  <br/> |<span data-ttu-id="dd7d6-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dd7d6-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd7d6-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dd7d6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd7d6-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="dd7d6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd7d6-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd7d6-132">See also</span></span>



- [<span data-ttu-id="dd7d6-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd7d6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="dd7d6-134">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="dd7d6-134">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="dd7d6-135">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="dd7d6-135">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

