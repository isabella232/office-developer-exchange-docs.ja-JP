---
title: Status
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
description: 状態の要素は、作業項目の状態を表します。
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833584"
---
# <a name="status"></a><span data-ttu-id="d4bfc-103">Status</span><span class="sxs-lookup"><span data-stu-id="d4bfc-103">Status</span></span>

<span data-ttu-id="d4bfc-104">**状態**の要素は、作業項目の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="d4bfc-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="d4bfc-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4bfc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d4bfc-106">Attributes and elements</span></span>

<span data-ttu-id="d4bfc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4bfc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4bfc-108">Attributes</span></span>

<span data-ttu-id="d4bfc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4bfc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d4bfc-110">Child elements</span></span>

<span data-ttu-id="d4bfc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4bfc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d4bfc-112">Parent elements</span></span>

|<span data-ttu-id="d4bfc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4bfc-113">**Element**</span></span>|<span data-ttu-id="d4bfc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4bfc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4bfc-115">タスク</span><span class="sxs-lookup"><span data-stu-id="d4bfc-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="d4bfc-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4bfc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d4bfc-117">Text value</span></span>

<span data-ttu-id="d4bfc-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-118">A text value is required.</span></span> <span data-ttu-id="d4bfc-119">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="d4bfc-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="d4bfc-120">NotStarted</span></span>
    
- <span data-ttu-id="d4bfc-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="d4bfc-121">InProgress</span></span>
    
- <span data-ttu-id="d4bfc-122">Completed</span><span class="sxs-lookup"><span data-stu-id="d4bfc-122">Completed</span></span>
    
- <span data-ttu-id="d4bfc-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="d4bfc-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="d4bfc-124">Deferred</span><span class="sxs-lookup"><span data-stu-id="d4bfc-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d4bfc-125">備考</span><span class="sxs-lookup"><span data-stu-id="d4bfc-125">Remarks</span></span>

<span data-ttu-id="d4bfc-126">[CompleteDate](completedate.md)を設定すると、[達成率](percentcomplete.md)を 100 または**完了****状態**に設定すると同じ効果になります。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="d4bfc-127">で、これらのプロパティには、少なくとも 2 つ設定、処理された最後のプロパティ値が決まります。 これらの要素に設定されている要求。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="d4bfc-128">たとえば、**達成率**が 100 の場合、 **CompleteDate**は 2007 年 1 月 1 日と**状態**が [未開始、プロパティがこの順序でストリームは、未開始、 **CompleteDate にタスクの**ステータス**を設定するのには影響があります。** は**null**との**達成率**を 0 にします。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="d4bfc-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4bfc-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="d4bfc-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4bfc-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="d4bfc-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4bfc-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4bfc-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d4bfc-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d4bfc-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4bfc-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4bfc-134">Validation File</span></span>  <br/> |<span data-ttu-id="d4bfc-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4bfc-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4bfc-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d4bfc-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4bfc-137">False</span><span class="sxs-lookup"><span data-stu-id="d4bfc-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4bfc-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4bfc-138">See also</span></span>



- [<span data-ttu-id="d4bfc-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4bfc-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d4bfc-140">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-140">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="d4bfc-141">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="d4bfc-141">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

