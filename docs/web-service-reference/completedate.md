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
description: CompleteDate 要素は、アイテムが完了した日付を表します。
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461423"
---
# <a name="completedate"></a><span data-ttu-id="7a071-103">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="7a071-103">CompleteDate</span></span>

<span data-ttu-id="7a071-104">**Completedate**要素は、アイテムが完了した日付を表します。</span><span class="sxs-lookup"><span data-stu-id="7a071-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="7a071-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="7a071-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a071-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7a071-106">Attributes and elements</span></span>

<span data-ttu-id="7a071-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a071-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a071-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a071-108">Attributes</span></span>

<span data-ttu-id="7a071-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7a071-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a071-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7a071-110">Child elements</span></span>

<span data-ttu-id="7a071-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7a071-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a071-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7a071-112">Parent elements</span></span>

|<span data-ttu-id="7a071-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a071-113">**Element**</span></span>|<span data-ttu-id="7a071-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a071-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a071-115">タスク</span><span class="sxs-lookup"><span data-stu-id="7a071-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="7a071-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7a071-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7a071-117">Flag</span><span class="sxs-lookup"><span data-stu-id="7a071-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="7a071-118">メールボックスアイテムのフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="7a071-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a071-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7a071-119">Text value</span></span>

<span data-ttu-id="7a071-120">この要素を使用する場合は、日付と時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a071-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a071-121">注釈</span><span class="sxs-lookup"><span data-stu-id="7a071-121">Remarks</span></span>

<span data-ttu-id="7a071-122">**Completedate**の設定は、[達成](percentcomplete.md)率を100または[状態](status.md)から**完了**に設定した場合と同じ効果があります。</span><span class="sxs-lookup"><span data-stu-id="7a071-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="7a071-123">これらのプロパティの少なくとも2つを設定する要求では、最後に処理されたプロパティによって、これらの要素に設定されている値が決まります。</span><span class="sxs-lookup"><span data-stu-id="7a071-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="7a071-124">たとえば、[達成](percentcomplete.md)率が100、 **completedate**が2007、[状態](status.md)が**NotStarted**で、プロパティがその順序でストリーミングされている場合は、タスクの[状態](status.md)を**NotStarted**に設定し、 [completedate](completedate.md)を**null**に設定し、[達成](percentcomplete.md)率を0に設定することになります。</span><span class="sxs-lookup"><span data-stu-id="7a071-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="7a071-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7a071-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a071-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7a071-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a071-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a071-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a071-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a071-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7a071-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7a071-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a071-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a071-130">Validation File</span></span>  <br/> |<span data-ttu-id="7a071-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7a071-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a071-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7a071-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a071-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="7a071-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a071-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a071-134">See also</span></span>



- [<span data-ttu-id="7a071-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a071-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7a071-136">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="7a071-136">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="7a071-137">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="7a071-137">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

