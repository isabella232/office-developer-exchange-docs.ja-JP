---
title: UpdateItem 処理 (タスク)
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
description: UpdateItem 操作を使用して、Exchange ストア内の作業項目のプロパティを更新します。
ms.openlocfilehash: d6f966fa663300b476383a136d30cf611d6bfb9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839864"
---
# <a name="updateitem-operation-task"></a><span data-ttu-id="e3020-103">UpdateItem 処理 (タスク)</span><span class="sxs-lookup"><span data-stu-id="e3020-103">UpdateItem operation (task)</span></span>

<span data-ttu-id="e3020-104">UpdateItem 操作を使用して、Exchange ストア内の作業項目のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3020-104">The UpdateItem operation is used to update task item properties in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3020-105">備考</span><span class="sxs-lookup"><span data-stu-id="e3020-105">Remarks</span></span>

<span data-ttu-id="e3020-106">仕事の依頼を送信するのに Exchange Web サービスを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="e3020-106">You cannot use Exchange Web Services to send task requests.</span></span> <span data-ttu-id="e3020-107">Exchange Web サービスでは、MicrosoftOfficeOutlook によって作成された仕事の依頼を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="e3020-107">Exchange Web Services can return task requests that are created by MicrosoftOfficeOutlook.</span></span> <span data-ttu-id="e3020-108">仕事の依頼は既に送信された場合、タスクの更新要求はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="e3020-108">If a task request has already been sent, a request to update the task will return an error.</span></span>
  
## <a name="updating-the-current-occurrence-of-a-recurring-task"></a><span data-ttu-id="e3020-109">定期的な仕事の現在の回を更新</span><span class="sxs-lookup"><span data-stu-id="e3020-109">Updating the Current Occurrence of a Recurring Task</span></span>

<span data-ttu-id="e3020-110">定期的なタスクに対して UpdateItem 操作の結果は、1 つの非定期的なタスクで UpdateItem 演算の結果によって異なります。</span><span class="sxs-lookup"><span data-stu-id="e3020-110">The result of an UpdateItem operation on recurring tasks differs from the result of the UpdateItem operation on a single, nonrecurring task.</span></span> <span data-ttu-id="e3020-111">定期的な仕事の発生への変更には、次の更新が行われたときに生成される一時的な仕事が発生します。</span><span class="sxs-lookup"><span data-stu-id="e3020-111">Changes to an occurrence of a recurring task cause one-off tasks to be generated when the following updates are made:</span></span>
  
1. <span data-ttu-id="e3020-112">再生成するか、nonregenerating の定期的なタスクの status プロパティは、**完了**に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e3020-112">The status property of a regenerating or nonregenerating recurrent task is set to **Completed**.</span></span>
    
2. <span data-ttu-id="e3020-113">開始日または nonregenerating の定期的なタスクの終了日が変更されます。</span><span class="sxs-lookup"><span data-stu-id="e3020-113">The start date or end date of a nonregenerating recurrent task is changed.</span></span>
    
<span data-ttu-id="e3020-114">たとえば、 **UpdateItem**要求は、定期的なタスクの完了] の値を**true**にしている場合は、 **UpdateItemResponse**は、新しい Id と変更キーを新しく作成された 1 回限りのタスクを表す含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3020-114">For example, if an **UpdateItem** request sets the Completed value of a recurring task to **true**, the **UpdateItemResponse** will include a new Id and ChangeKey that represent a newly created one-off task.</span></span> <span data-ttu-id="e3020-115">要求に含まれていた Id がまだ有効であると、次の出現箇所を表示するのにはその Id で表される定期的なタスクが更新されました。</span><span class="sxs-lookup"><span data-stu-id="e3020-115">The Id that was included in the request is still valid and the recurring task that is represented by that Id has been updated to represent the next occurrence.</span></span> <span data-ttu-id="e3020-116">定期タスクが更新されたために、要求に含まれていた変更キーは有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="e3020-116">The ChangeKey that was included in the request is no longer valid because the recurring task has been updated.</span></span> 
  
<span data-ttu-id="e3020-117">[GetItem 操作](getitem-operation.md)を使用すると、定期タスクの最新の**変更キー**を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3020-117">You can use the [GetItem operation](getitem-operation.md) to get the latest **ChangeKey** for the recurring task.</span></span> 
  
<span data-ttu-id="e3020-118">非定期的なタスクまたは定期タスクの最後に出現 UpdateItem 応答は、渡されたものとそれに関連付けられた**変更キー**の更新を取得する同じ**Id**を返します。</span><span class="sxs-lookup"><span data-stu-id="e3020-118">For nonrecurring tasks or for the last occurrence of a recurring task, the UpdateItem response returns the same **Id** that was passed to it and returns the associated updated **ChangeKey**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e3020-119">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3020-119">See also</span></span>



<span data-ttu-id="e3020-120">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e3020-120">[UpdateItem operation](updateitem-operation.md)</span></span>

