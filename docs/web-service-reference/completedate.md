---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: CompleteDate 要素は、項目が完了された日付を表します。
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759635"
---
# <a name="completedate"></a><span data-ttu-id="7c87c-103">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="7c87c-103">CompleteDate</span></span>

<span data-ttu-id="7c87c-104">**CompleteDate**要素は、項目が完了された日付を表します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="7c87c-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="7c87c-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c87c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c87c-106">Attributes and elements</span></span>

<span data-ttu-id="7c87c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c87c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c87c-108">Attributes</span></span>

<span data-ttu-id="7c87c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c87c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c87c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c87c-110">Child elements</span></span>

<span data-ttu-id="7c87c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7c87c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c87c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7c87c-112">Parent elements</span></span>

|<span data-ttu-id="7c87c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c87c-113">**Element**</span></span>|<span data-ttu-id="7c87c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c87c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c87c-115">タスク</span><span class="sxs-lookup"><span data-stu-id="7c87c-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="7c87c-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7c87c-117">Flag</span><span class="sxs-lookup"><span data-stu-id="7c87c-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="7c87c-118">メールボックス アイテムにフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c87c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7c87c-119">Text value</span></span>

<span data-ttu-id="7c87c-120">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="7c87c-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c87c-121">備考</span><span class="sxs-lookup"><span data-stu-id="7c87c-121">Remarks</span></span>

<span data-ttu-id="7c87c-122">**CompleteDate**を設定すると、[達成率](percentcomplete.md)を 100 または**完了**[状態](status.md)に設定すると同じ効果になります。</span><span class="sxs-lookup"><span data-stu-id="7c87c-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="7c87c-123">で、これらのプロパティには、少なくとも 2 つ設定、処理された最後のプロパティ値が決まります。 これらの要素に設定されている要求。</span><span class="sxs-lookup"><span data-stu-id="7c87c-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="7c87c-124">たとえば、[達成率](percentcomplete.md)は、100、 **CompleteDate**には、2007 年 1 月 1 日[状態](status.md)が [**未開始**、しプロパティをこの順序でストリームは、影響がある**未開始にタスクの[ステータス](status.md)を設定するのには**、 [CompleteDate](completedate.md) **null**、および[達成率](percentcomplete.md)を 0 にするです。</span><span class="sxs-lookup"><span data-stu-id="7c87c-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="7c87c-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7c87c-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c87c-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c87c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c87c-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c87c-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c87c-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c87c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7c87c-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7c87c-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c87c-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c87c-130">Validation File</span></span>  <br/> |<span data-ttu-id="7c87c-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c87c-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c87c-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c87c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c87c-133">False</span><span class="sxs-lookup"><span data-stu-id="7c87c-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c87c-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c87c-134">See also</span></span>



- [<span data-ttu-id="7c87c-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c87c-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7c87c-136">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-136">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="7c87c-137">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="7c87c-137">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

