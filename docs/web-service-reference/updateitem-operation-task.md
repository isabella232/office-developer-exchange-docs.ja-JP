---
title: UpdateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: b0a7f114-d040-40eb-a8f3-05ea6489e472
description: UpdateItem 操作は、Exchange ストア内のタスクアイテムのプロパティを更新するために使用されます。
ms.openlocfilehash: 0041af114d11fd9577037dd154e40b84e8483c35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459806"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="feb39-103">UpdateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="feb39-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="feb39-104">UpdateItem 操作は、Exchange ストア内のタスクアイテムのプロパティを更新するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="feb39-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="feb39-105">注釈</span><span class="sxs-lookup"><span data-stu-id="feb39-105">Remarks</span></span>

<span data-ttu-id="feb39-106">Exchange Web サービスを使用してタスクの要求を送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="feb39-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="feb39-107">Exchange Web サービスは、Microsoft office outlook によって作成されたタスク要求を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="feb39-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="feb39-108">タスクの依頼が既に送信されている場合、タスクを更新する要求はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="feb39-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="feb39-109">定期的なタスクの現在の発生を更新する</span><span class="sxs-lookup"><span data-stu-id="feb39-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="feb39-110">定期的なタスクに対する UpdateItem 操作の結果は、単一の非定期的なタスクに対する UpdateItem 操作の結果とは異なります。</span><span class="sxs-lookup"><span data-stu-id="feb39-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="feb39-111">定期的なタスクの発生に変更を加えると、次の更新が行われたときに1回限りのタスクが生成されます。</span><span class="sxs-lookup"><span data-stu-id="feb39-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="feb39-112">[再生成] または [再生成なし] のタスクの [状態] プロパティは、[**完了**] に設定されています。</span><span class="sxs-lookup"><span data-stu-id="feb39-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="feb39-113">再生成以外のタスクの開始日または終了日が変更されています。</span><span class="sxs-lookup"><span data-stu-id="feb39-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="feb39-114">たとえば、 **Updateitem**要求で定期的なタスクの完了値を**true**に設定すると、 **updateitemresponse**には、新しく作成された1回限りのタスクを表す新しい Id と changekey が含まれます。</span><span class="sxs-lookup"><span data-stu-id="feb39-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="feb39-115">要求に含まれていた Id は依然として有効であり、その Id で表される定期タスクは、次の出現を表すように更新されています。</span><span class="sxs-lookup"><span data-stu-id="feb39-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="feb39-116">要求に含まれていた ChangeKey は、定期タスクが更新されているため無効になりました。</span><span class="sxs-lookup"><span data-stu-id="feb39-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="feb39-117">[GetItem 操作](getitem-operation.md)を使用して、定期的なタスクの最新の**changekey**を取得できます。</span><span class="sxs-lookup"><span data-stu-id="feb39-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="feb39-118">非定期的なタスクまたは定期的なタスクの最後の発生の場合、UpdateItem 応答は渡されたものと同じ**Id**を返し、関連付けられた更新された**changekey**を返します。</span><span class="sxs-lookup"><span data-stu-id="feb39-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="feb39-119">関連項目</span><span class="sxs-lookup"><span data-stu-id="feb39-119">See also</span></span>



<span data-ttu-id="feb39-120">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="feb39-120">[UpdateItem operation](updateitem-operation.md)</span></span>

