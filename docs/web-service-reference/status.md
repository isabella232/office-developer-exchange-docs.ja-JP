---
title: 状態
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: Status 要素は、タスクアイテムの状態を表します。
ms.openlocfilehash: 5d022827990b96fd8790ae9566ef49028ebe404c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459960"
---
# <a name="status"></a><span data-ttu-id="c5425-103">状態</span><span class="sxs-lookup"><span data-stu-id="c5425-103">Status</span></span>

<span data-ttu-id="c5425-104">**Status**要素は、タスクアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c5425-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="c5425-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="c5425-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5425-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c5425-106">Attributes and elements</span></span>

<span data-ttu-id="c5425-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c5425-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5425-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5425-108">Attributes</span></span>

<span data-ttu-id="c5425-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c5425-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5425-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c5425-110">Child elements</span></span>

<span data-ttu-id="c5425-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c5425-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5425-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c5425-112">Parent elements</span></span>

|<span data-ttu-id="c5425-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c5425-113">**Element**</span></span>|<span data-ttu-id="c5425-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c5425-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5425-115">タスク</span><span class="sxs-lookup"><span data-stu-id="c5425-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="c5425-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="c5425-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5425-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c5425-117">Text value</span></span>

<span data-ttu-id="c5425-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="c5425-118">A text value is required.</span></span> <span data-ttu-id="c5425-119">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c5425-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="c5425-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="c5425-120">NotStarted</span></span>
    
- <span data-ttu-id="c5425-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="c5425-121">InProgress</span></span>
    
- <span data-ttu-id="c5425-122">Completed</span><span class="sxs-lookup"><span data-stu-id="c5425-122">Completed</span></span>
    
- <span data-ttu-id="c5425-123">WaitingOnOthers 他</span><span class="sxs-lookup"><span data-stu-id="c5425-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="c5425-124">Deferred</span><span class="sxs-lookup"><span data-stu-id="c5425-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c5425-125">注釈</span><span class="sxs-lookup"><span data-stu-id="c5425-125">Remarks</span></span>

<span data-ttu-id="c5425-126">[Completedate](completedate.md)の設定は、[達成](percentcomplete.md)率を100または**状態**から**完了**に設定した場合と同じ効果があります。</span><span class="sxs-lookup"><span data-stu-id="c5425-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="c5425-127">これらのプロパティの少なくとも2つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定されている値が決まります。</span><span class="sxs-lookup"><span data-stu-id="c5425-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="c5425-128">たとえば、**達成**率が100、 **completedate**が1/1/2007、**状態**が NotStarted で、プロパティがこの順序でストリーミングされている場合は、タスクの**状態**を NotStarted に、 **completedate**を**null**に、**達成**率を0に設定することになります。</span><span class="sxs-lookup"><span data-stu-id="c5425-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="c5425-129">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c5425-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5425-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c5425-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5425-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5425-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5425-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c5425-132">Schema Name</span></span>  <br/> |<span data-ttu-id="c5425-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c5425-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5425-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c5425-134">Validation File</span></span>  <br/> |<span data-ttu-id="c5425-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c5425-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5425-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c5425-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5425-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="c5425-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5425-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c5425-138">See also</span></span>



- [<span data-ttu-id="c5425-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c5425-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="c5425-140">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="c5425-140">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="c5425-141">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="c5425-141">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

