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
description: 達成率の要素は、タスクの完了状態を説明します。
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832717"
---
# <a name="percentcomplete"></a><span data-ttu-id="19f7b-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="19f7b-103">PercentComplete</span></span>

<span data-ttu-id="19f7b-104">**達成率**の要素は、タスクの完了状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="19f7b-105">**二重**</span><span class="sxs-lookup"><span data-stu-id="19f7b-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19f7b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="19f7b-106">Attributes and elements</span></span>

<span data-ttu-id="19f7b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19f7b-108">属性</span><span class="sxs-lookup"><span data-stu-id="19f7b-108">Attributes</span></span>

<span data-ttu-id="19f7b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19f7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19f7b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19f7b-110">Child elements</span></span>

<span data-ttu-id="19f7b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="19f7b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19f7b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="19f7b-112">Parent elements</span></span>

|<span data-ttu-id="19f7b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="19f7b-113">**Element**</span></span>|<span data-ttu-id="19f7b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="19f7b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19f7b-115">タスク</span><span class="sxs-lookup"><span data-stu-id="19f7b-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="19f7b-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19f7b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="19f7b-117">Text value</span></span>

<span data-ttu-id="19f7b-118">0 から 100 までの整数を表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="19f7b-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19f7b-119">備考</span><span class="sxs-lookup"><span data-stu-id="19f7b-119">Remarks</span></span>

<span data-ttu-id="19f7b-120">[CompleteDate](completedate.md)要素を設定または**完了**の[状態](status.md)の要素の設定と同じ効果を**達成率**を 100 に設定します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="19f7b-121">で、これらのプロパティには、少なくとも 2 つ設定、処理された最後のプロパティ値が決まります。 これらの要素に設定されている要求。</span><span class="sxs-lookup"><span data-stu-id="19f7b-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="19f7b-122">たとえば、**達成率**は、100、 [CompleteDate](completedate.md)には、2007 年 1 月 1 日[状態](status.md)が [未開始、し、プロパティがこの順序でストリーム配信、影響がある未開始、[に、タスクの[ステータス](status.md)を設定するのにはCompleteDate](completedate.md)は**null**との**達成率**を 0 にします。</span><span class="sxs-lookup"><span data-stu-id="19f7b-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="19f7b-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="19f7b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19f7b-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="19f7b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19f7b-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="19f7b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19f7b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19f7b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="19f7b-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="19f7b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="19f7b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19f7b-128">Validation File</span></span>  <br/> |<span data-ttu-id="19f7b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19f7b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19f7b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="19f7b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="19f7b-131">False</span><span class="sxs-lookup"><span data-stu-id="19f7b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19f7b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="19f7b-132">See also</span></span>



- [<span data-ttu-id="19f7b-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="19f7b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="19f7b-134">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-134">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="19f7b-135">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="19f7b-135">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

