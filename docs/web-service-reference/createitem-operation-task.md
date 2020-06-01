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
description: CreateItem 操作は、Exchange ストアにタスクアイテムを作成します。
ms.openlocfilehash: 502108843193e7ed8377b0fade9e106ef3d1976c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457103"
---
# <a name="createitem-operation-task"></a><span data-ttu-id="88d58-103">CreateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="88d58-103">CreateItem operation (task)</span></span>

<span data-ttu-id="88d58-104">CreateItem 操作は、Exchange ストアにタスクアイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="88d58-104">The CreateItem operation creates task items in the Exchange store.</span></span>
  
## <a name="task-createitem-request"></a><span data-ttu-id="88d58-105">Task CreateItem 要求</span><span class="sxs-lookup"><span data-stu-id="88d58-105">Task CreateItem Request</span></span>

### <a name="description"></a><span data-ttu-id="88d58-106">説明</span><span class="sxs-lookup"><span data-stu-id="88d58-106">Description</span></span>

<span data-ttu-id="88d58-107">次の CreateItem 要求の例は、メールボックス内のタスクアイテムを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="88d58-107">The following example of a CreateItem request shows how to create a task item in a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="88d58-108">コード</span><span class="sxs-lookup"><span data-stu-id="88d58-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

### <a name="comments"></a><span data-ttu-id="88d58-109">コメント</span><span class="sxs-lookup"><span data-stu-id="88d58-109">Comments</span></span>

<span data-ttu-id="88d58-110">定期的なタスクに対する要求は、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターが受信したときに変更されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-110">Requests for recurring tasks are altered when they are received by the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span> <span data-ttu-id="88d58-111">次の変更が行われます。</span><span class="sxs-lookup"><span data-stu-id="88d58-111">The following changes occur:</span></span>
  
- <span data-ttu-id="88d58-112">タスクの定期的なアイテムの期間の開始日[(定期的なアイテム)](startdate-recurrence.md)のプロパティには、日付のみが保存されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-112">Only the date is saved for the [StartDate (Recurrence)](startdate-recurrence.md) property of the recurrence range of the task.</span></span> <span data-ttu-id="88d58-113">時刻部分は切り捨てられます。</span><span class="sxs-lookup"><span data-stu-id="88d58-113">The time part is truncated.</span></span> 
    
- <span data-ttu-id="88d58-114">[StartDate (定期的なアイテム)](startdate-recurrence.md)プロパティは、定期的なパターンに応じて調整できます。</span><span class="sxs-lookup"><span data-stu-id="88d58-114">The [StartDate (Recurrence)](startdate-recurrence.md) property may be adjusted, depending on the recurrence pattern.</span></span> <span data-ttu-id="88d58-115">たとえば、定期パターンが毎週月曜日として指定されていて、StartDate が2006年10月26日に設定されている場合、StartDate は次の月曜日である2006年10月30日に調整されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-115">For example, if the recurrence pattern is specified as every Monday and the StartDate is set to October 26, 2006, which is a Thursday, StartDate is adjusted to October 30, 2006, which is the next Monday.</span></span> 
    
- <span data-ttu-id="88d58-116">タスクの[startdate](startdate.md)プロパティが設定されている場合は、定期的なアイテムの範囲の[startdate (繰り返し)](startdate-recurrence.md)に合わせて更新されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-116">If the [StartDate](startdate.md) property of the task is set, it is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> <span data-ttu-id="88d58-117">タスクの[DueDate](duedate.md)プロパティも、新しい[StartDate](startdate.md)に基づいて更新されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-117">The [DueDate](duedate.md) property of the task is also updated based on the new [StartDate](startdate.md).</span></span>
    
- <span data-ttu-id="88d58-118">[Startdate](startdate.md)が設定されていない場合は、 [DueDate](duedate.md)プロパティのみが更新され、定期的なアイテムの範囲の[startdate (繰り返し)](startdate-recurrence.md)に一致します。</span><span class="sxs-lookup"><span data-stu-id="88d58-118">If the [StartDate](startdate.md) is not set, only the [DueDate](duedate.md) property is updated to match the [StartDate (Recurrence)](startdate-recurrence.md) of the recurrence range.</span></span> 
    
<span data-ttu-id="88d58-119">次の表に、クライアントアクセスサーバーが、毎週月曜日の定期タスクに対して行う変更を示します。</span><span class="sxs-lookup"><span data-stu-id="88d58-119">The following table shows the changes that the Client Access server makes to a recurring task that has a Task.Recurrence.Pattern of every Monday.</span></span>
  
<span data-ttu-id="88d58-120">**定期的なタスクに対する変更**</span><span class="sxs-lookup"><span data-stu-id="88d58-120">**Changes to a recurring task**</span></span>

|<span data-ttu-id="88d58-121">**Property**</span><span class="sxs-lookup"><span data-stu-id="88d58-121">**Property**</span></span>|<span data-ttu-id="88d58-122">**元の値**</span><span class="sxs-lookup"><span data-stu-id="88d58-122">**Original Value**</span></span>|<span data-ttu-id="88d58-123">**更新された値**</span><span class="sxs-lookup"><span data-stu-id="88d58-123">**Updated Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="88d58-124">タスクの開始日</span><span class="sxs-lookup"><span data-stu-id="88d58-124">Task.StartDate</span></span>  <br/> |<span data-ttu-id="88d58-125">2006年1月1日</span><span class="sxs-lookup"><span data-stu-id="88d58-125">January 1, 2006</span></span>  <br/> |<span data-ttu-id="88d58-126">2006年10月30日</span><span class="sxs-lookup"><span data-stu-id="88d58-126">October 30, 2006</span></span>  <br/> |
|<span data-ttu-id="88d58-127">DueDate</span><span class="sxs-lookup"><span data-stu-id="88d58-127">Task.DueDate</span></span>  <br/> |<span data-ttu-id="88d58-128">2006年1月3日</span><span class="sxs-lookup"><span data-stu-id="88d58-128">January 3, 2006</span></span>  <br/> |<span data-ttu-id="88d58-129">2006年11月1日</span><span class="sxs-lookup"><span data-stu-id="88d58-129">November 1, 2006</span></span>  <br/> |
|<span data-ttu-id="88d58-130">タスクの定期的なアイテムの指定。</span><span class="sxs-lookup"><span data-stu-id="88d58-130">Task.Recurrence.Range.StartDate</span></span>  <br/> |<span data-ttu-id="88d58-131">2006年10月26日</span><span class="sxs-lookup"><span data-stu-id="88d58-131">October 26, 2006</span></span>  <br/> |<span data-ttu-id="88d58-132">2006年10月30日</span><span class="sxs-lookup"><span data-stu-id="88d58-132">October 30, 2006</span></span>  <br/> |
   
<span data-ttu-id="88d58-133">既定では、宛先フォルダーが指定されていない場合、タスクアイテムは [タスク] フォルダーに作成されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-133">By default, if a destination folder is not specified, task items are created in the Tasks folder.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="88d58-134">Request 要素</span><span class="sxs-lookup"><span data-stu-id="88d58-134">Request elements</span></span>

<span data-ttu-id="88d58-135">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="88d58-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="88d58-136">CreateItem</span><span class="sxs-lookup"><span data-stu-id="88d58-136">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="88d58-137">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="88d58-137">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="88d58-138">Task</span><span class="sxs-lookup"><span data-stu-id="88d58-138">Task</span></span>](task.md)
    
- <span data-ttu-id="88d58-139">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="88d58-139">[Subject](subject.md)</span></span>
    
- [<span data-ttu-id="88d58-140">DueDate</span><span class="sxs-lookup"><span data-stu-id="88d58-140">DueDate</span></span>](duedate.md)
    
- [<span data-ttu-id="88d58-141">状態</span><span class="sxs-lookup"><span data-stu-id="88d58-141">Status</span></span>](status.md)
    
## <a name="successful-task-createitem-response"></a><span data-ttu-id="88d58-142">成功したタスクの CreateItem 応答</span><span class="sxs-lookup"><span data-stu-id="88d58-142">Successful Task CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="88d58-143">説明</span><span class="sxs-lookup"><span data-stu-id="88d58-143">Description</span></span>

<span data-ttu-id="88d58-144">次の例は、CreateItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="88d58-144">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="88d58-145">コード</span><span class="sxs-lookup"><span data-stu-id="88d58-145">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="88d58-146">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="88d58-146">Successful response elements</span></span>

<span data-ttu-id="88d58-147">応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="88d58-147">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="88d58-148">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="88d58-148">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="88d58-149">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="88d58-149">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="88d58-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="88d58-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="88d58-151">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88d58-151">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="88d58-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="88d58-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="88d58-153">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="88d58-153">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="88d58-154">Task</span><span class="sxs-lookup"><span data-stu-id="88d58-154">Task</span></span>](task.md)
    
- [<span data-ttu-id="88d58-155">ItemId</span><span class="sxs-lookup"><span data-stu-id="88d58-155">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="88d58-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="88d58-156">See also</span></span>



<span data-ttu-id="88d58-157">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="88d58-157">[CreateItem operation](createitem-operation.md)</span></span>


[<span data-ttu-id="88d58-158">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="88d58-158">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="88d58-159">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="88d58-159">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="88d58-160">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="88d58-160">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

