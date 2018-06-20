---
title: CreateItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: CreateItem 操作は、Exchange ストア内の作業項目を作成します。
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759838"
---
# <a name="createitem-operation-task"></a><span data-ttu-id="719e5-103">CreateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="719e5-103">CreateItem operation (task)</span></span>

<span data-ttu-id="719e5-104">CreateItem 操作は、Exchange ストア内の作業項目を作成します。</span><span class="sxs-lookup"><span data-stu-id="719e5-104">The CreateItem operation creates task items in the Exchange store.</span></span>
  
## <a name="task-createitem-request"></a><span data-ttu-id="719e5-105">CreateItem 要求のタスク</span><span class="sxs-lookup"><span data-stu-id="719e5-105">Task CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="719e5-106">説明</span><span class="sxs-lookup"><span data-stu-id="719e5-106">Description</span></span>

<span data-ttu-id="719e5-107">CreateItem 要求の次の例では、メールボックス内のタスク項目を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="719e5-107">The following example of a CreateItem request shows how to create a task item in a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="719e5-108">コード</span><span class="sxs-lookup"><span data-stu-id="719e5-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="719e5-109">コメント</span><span class="sxs-lookup"><span data-stu-id="719e5-109">Comments</span></span>

<span data-ttu-id="719e5-110">定期タスクの要求は、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターで受信したときに変更されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-110">Requests for recurring tasks are altered when they are received by the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span> <span data-ttu-id="719e5-111">次の変更が発生します。</span><span class="sxs-lookup"><span data-stu-id="719e5-111">The following changes occur:</span></span>
  
- <span data-ttu-id="719e5-112">タスクの期間の[開始日 (反復)](startdate-recurrence.md)プロパティの値は、日付のみが保存されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-112">Only the date is saved for the [StartDate (Recurrence)](startdate-recurrence.md) property of the recurrence range of the task.</span></span> <span data-ttu-id="719e5-113">時刻の部分が切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="719e5-113">The time part is truncated.</span></span> 
    
- <span data-ttu-id="719e5-114">定期的なパターンによって、[開始日 (繰り返し)](startdate-recurrence.md)のプロパティを調整することがあります。</span><span class="sxs-lookup"><span data-stu-id="719e5-114">The [StartDate (Recurrence)](startdate-recurrence.md) property may be adjusted, depending on the recurrence pattern.</span></span> <span data-ttu-id="719e5-115">開始日の調整など、定期的なパターンが、毎週月曜日を指定し、開始日が 2006 年 10 月 26 日に設定されている場合は木曜日で、2006 年 10 月 30 日には次の月曜日です。</span><span class="sxs-lookup"><span data-stu-id="719e5-115">For example, if the recurrence pattern is specified as every Monday and the StartDate is set to October 26, 2006, which is a Thursday, StartDate is adjusted to October 30, 2006, which is the next Monday.</span></span> 
    
- <span data-ttu-id="719e5-116">タスクの[開始日](startdate.md)のプロパティが設定されている場合は、定期的なアイテムの範囲の[開始日 (反復)](startdate-recurrence.md)を一致するように更新されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-116">If the [StartDate](startdate.md) property of the task is set, it is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> <span data-ttu-id="719e5-117">タスクの[DueDate](duedate.md)プロパティに新しい[開始日](startdate.md)に基づいて更新されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-117">The [DueDate](duedate.md) property of the task is also updated based on the new [StartDate](startdate.md).</span></span>
    
- <span data-ttu-id="719e5-118">[開始日](startdate.md)が設定されていない場合は、定期的なアイテムの範囲の[開始日 (反復)](startdate-recurrence.md)を一致するように[DueDate](duedate.md)プロパティのみが更新されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-118">If the [StartDate](startdate.md) is not set, only the [DueDate](duedate.md) property is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> 
    
<span data-ttu-id="719e5-119">次の表は、定期的なタスクを毎週月曜日の Task.Recurrence.Pattern を持つクライアント アクセス サーバーが行った変更を示しています。</span><span class="sxs-lookup"><span data-stu-id="719e5-119">The following table shows the changes that the Client Access server makes to a recurring task that has a Task.Recurrence.Pattern of every Monday.</span></span>
  
<span data-ttu-id="719e5-120">**定期的なタスクへの変更**</span><span class="sxs-lookup"><span data-stu-id="719e5-120">**Changes to a recurring task**</span></span>

|<span data-ttu-id="719e5-121">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="719e5-121">**Property**</span></span>|<span data-ttu-id="719e5-122">**元の値**</span><span class="sxs-lookup"><span data-stu-id="719e5-122">**Original Value**</span></span>|<span data-ttu-id="719e5-123">**更新された値**</span><span class="sxs-lookup"><span data-stu-id="719e5-123">**Updated Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="719e5-124">Task.StartDate</span><span class="sxs-lookup"><span data-stu-id="719e5-124">Task.StartDate</span></span>  <br/> |<span data-ttu-id="719e5-125">2006 年 1 月 1 日</span><span class="sxs-lookup"><span data-stu-id="719e5-125">January 1, 2006</span></span>  <br/> |<span data-ttu-id="719e5-126">2006 年 10 月 30 日</span><span class="sxs-lookup"><span data-stu-id="719e5-126">October 30, 2006</span></span>  <br/> |
|<span data-ttu-id="719e5-127">Task.DueDate</span><span class="sxs-lookup"><span data-stu-id="719e5-127">Task.DueDate</span></span>  <br/> |<span data-ttu-id="719e5-128">2006 年 1 月 3 日</span><span class="sxs-lookup"><span data-stu-id="719e5-128">January 3, 2006</span></span>  <br/> |<span data-ttu-id="719e5-129">2006 年 11 月 1 日</span><span class="sxs-lookup"><span data-stu-id="719e5-129">November 1, 2006</span></span>  <br/> |
|<span data-ttu-id="719e5-130">Task.Recurrence.Range.StartDate</span><span class="sxs-lookup"><span data-stu-id="719e5-130">Task.Recurrence.Range.StartDate</span></span>  <br/> |<span data-ttu-id="719e5-131">2006 年 10 月 26 日</span><span class="sxs-lookup"><span data-stu-id="719e5-131">October 26, 2006</span></span>  <br/> |<span data-ttu-id="719e5-132">2006 年 10 月 30 日</span><span class="sxs-lookup"><span data-stu-id="719e5-132">October 30, 2006</span></span>  <br/> |
   
<span data-ttu-id="719e5-133">既定では、インストール先のフォルダーが指定されていない場合タスク項目は、[タスク] フォルダーに作成されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-133">By default, if a destination folder is not specified, task items are created in the Tasks folder.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="719e5-134">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="719e5-134">Request elements</span></span>

<span data-ttu-id="719e5-135">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="719e5-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="719e5-136">CreateItem</span><span class="sxs-lookup"><span data-stu-id="719e5-136">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="719e5-137">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="719e5-137">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="719e5-138">タスク</span><span class="sxs-lookup"><span data-stu-id="719e5-138">Task</span></span>](task.md)
    
- [<span data-ttu-id="719e5-139">Subject</span><span class="sxs-lookup"><span data-stu-id="719e5-139">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="719e5-140">DueDate</span><span class="sxs-lookup"><span data-stu-id="719e5-140">DueDate</span></span>](duedate.md)
    
- [<span data-ttu-id="719e5-141">Status</span><span class="sxs-lookup"><span data-stu-id="719e5-141">Status</span></span>](status.md)
    
## <a name="successful-task-createitem-response"></a><span data-ttu-id="719e5-142">Createitem メソッドの応答を正常終了したタスク</span><span class="sxs-lookup"><span data-stu-id="719e5-142">Successful Task CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="719e5-143">説明</span><span class="sxs-lookup"><span data-stu-id="719e5-143">Description</span></span>

<span data-ttu-id="719e5-144">次の使用例は、CreateItem 要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="719e5-144">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="719e5-145">コード</span><span class="sxs-lookup"><span data-stu-id="719e5-145">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="719e5-146">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="719e5-146">Successful response elements</span></span>

<span data-ttu-id="719e5-147">応答では、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="719e5-147">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="719e5-148">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="719e5-148">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="719e5-149">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="719e5-149">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="719e5-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="719e5-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="719e5-151">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="719e5-151">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="719e5-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="719e5-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="719e5-153">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="719e5-153">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="719e5-154">タスク</span><span class="sxs-lookup"><span data-stu-id="719e5-154">Task</span></span>](task.md)
    
- [<span data-ttu-id="719e5-155">ItemId</span><span class="sxs-lookup"><span data-stu-id="719e5-155">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="719e5-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="719e5-156">See also</span></span>



<span data-ttu-id="719e5-157">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="719e5-157">[CreateItem operation](createitem-operation.md)</span></span>


[<span data-ttu-id="719e5-158">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="719e5-158">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="719e5-159">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="719e5-159">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="719e5-160">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="719e5-160">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

