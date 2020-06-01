---
title: GetItem 操作 (タスク)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 8265dd06-1752-4470-8074-5f0e3e970f52
description: GetItem 操作は、Exchange ストアからタスクを取得するために使用されます。
ms.openlocfilehash: 17a23d4c2a35761e831610f3514c980a5a67e12b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463336"
---
# <a name="getitem-operation-task"></a><span data-ttu-id="d2ce1-103">GetItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="d2ce1-103">GetItem operation (task)</span></span>

<span data-ttu-id="d2ce1-104">GetItem 操作は、Exchange ストアからタスクを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-104">The GetItem operation is used to get tasks from the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2ce1-105">注釈</span><span class="sxs-lookup"><span data-stu-id="d2ce1-105">Remarks</span></span>

<span data-ttu-id="d2ce1-106">タスクの GetItem 要求の形式は、その他のアイテムの種類に対する GetItem と同じです。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-106">The format of the GetItem request for tasks is the same as GetItem for any other item type.</span></span> <span data-ttu-id="d2ce1-107">唯一の違いは、応答図形内で追加のプロパティを要求できる点です。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-107">The only difference is in which additional properties can be requested within the response shape.</span></span> <span data-ttu-id="d2ce1-108">その他のプロパティは、タスク関連のプロパティまたは拡張プロパティである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-108">Such additional properties must either be task-related properties or extended properties.</span></span>
  
## <a name="task-getitem-request-example"></a><span data-ttu-id="d2ce1-109">タスク GetItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="d2ce1-109">Task GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="d2ce1-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2ce1-110">Description</span></span>

<span data-ttu-id="d2ce1-111">GetItem 要求の次の例は、タスクアイテムを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-111">The following example of a GetItem request shows how to get a task item.</span></span>
  
### <a name="code"></a><span data-ttu-id="d2ce1-112">コード</span><span class="sxs-lookup"><span data-stu-id="d2ce1-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEFkb..."/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d2ce1-113">コメント</span><span class="sxs-lookup"><span data-stu-id="d2ce1-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="d2ce1-114">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-114">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="d2ce1-115">Request 要素</span><span class="sxs-lookup"><span data-stu-id="d2ce1-115">Request elements</span></span>

<span data-ttu-id="d2ce1-116">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d2ce1-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="d2ce1-117">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="d2ce1-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d2ce1-118">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="d2ce1-119">BaseShape</span><span class="sxs-lookup"><span data-stu-id="d2ce1-119">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="d2ce1-120">ItemIds</span><span class="sxs-lookup"><span data-stu-id="d2ce1-120">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="d2ce1-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="d2ce1-121">ItemId</span></span>](itemid.md)
    
## <a name="task-getitem-response-example"></a><span data-ttu-id="d2ce1-122">タスクの GetItem 応答の例</span><span class="sxs-lookup"><span data-stu-id="d2ce1-122">Task GetItem response example</span></span>

### <a name="description"></a><span data-ttu-id="d2ce1-123">説明</span><span class="sxs-lookup"><span data-stu-id="d2ce1-123">Description</span></span>

<span data-ttu-id="d2ce1-124">次の例は、GetItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-124">The following example shows a successful response to a GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d2ce1-125">コード</span><span class="sxs-lookup"><span data-stu-id="d2ce1-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EwAAAB"/>
              <t:ParentFolderId Id="AAAtAEFkbWl=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Task</t:ItemClass>
              <t:Subject>Buy new shoes</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-09-15T15:23:08Z</t:DateTimeReceived>
              <t:Size>153</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-09-15T15:23:08Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-09-15T15:23:08Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:ChangeCount>1</t:ChangeCount>
              <t:IsComplete>false</t:IsComplete>
              <t:IsRecurring>false</t:IsRecurring>
              <t:PercentComplete>0</t:PercentComplete>
              <t:Status>NotStarted</t:Status>
              <t:StatusDescription>Not Started</t:StatusDescription>
            </t:Task>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d2ce1-126">コメント</span><span class="sxs-lookup"><span data-stu-id="d2ce1-126">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="d2ce1-127">読みやすくするために、アイテムとフォルダーの識別子および変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-127">The item and folder identifiers and change keys have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="d2ce1-128">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="d2ce1-128">Successful response elements</span></span>

<span data-ttu-id="d2ce1-129">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d2ce1-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d2ce1-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d2ce1-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d2ce1-131">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="d2ce1-131">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="d2ce1-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2ce1-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d2ce1-133">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2ce1-133">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="d2ce1-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d2ce1-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d2ce1-135">Items</span><span class="sxs-lookup"><span data-stu-id="d2ce1-135">Items</span></span>](items.md)
    
- [<span data-ttu-id="d2ce1-136">Task</span><span class="sxs-lookup"><span data-stu-id="d2ce1-136">Task</span></span>](task.md)
    
- [<span data-ttu-id="d2ce1-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="d2ce1-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d2ce1-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d2ce1-138">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="d2ce1-139">ItemClass</span><span class="sxs-lookup"><span data-stu-id="d2ce1-139">ItemClass</span></span>](itemclass.md)
    
- <span data-ttu-id="d2ce1-140">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="d2ce1-140">[Subject](subject.md)</span></span>
    
- [<span data-ttu-id="d2ce1-141">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="d2ce1-141">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="d2ce1-142">Body</span><span class="sxs-lookup"><span data-stu-id="d2ce1-142">Body</span></span>](body.md)
    
- [<span data-ttu-id="d2ce1-143">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="d2ce1-143">DateTimeReceived</span></span>](datetimereceived.md)
    
- <span data-ttu-id="d2ce1-144">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="d2ce1-144">[Size](size.md)</span></span>
    
- [<span data-ttu-id="d2ce1-145">Importance</span><span class="sxs-lookup"><span data-stu-id="d2ce1-145">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="d2ce1-146">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="d2ce1-146">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="d2ce1-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="d2ce1-147">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="d2ce1-148">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="d2ce1-148">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="d2ce1-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="d2ce1-149">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="d2ce1-150">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="d2ce1-150">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="d2ce1-151">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="d2ce1-151">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="d2ce1-152">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="d2ce1-152">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="d2ce1-153">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="d2ce1-153">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="d2ce1-154">Culture</span><span class="sxs-lookup"><span data-stu-id="d2ce1-154">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="d2ce1-155">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="d2ce1-155">ChangeCount</span></span>](changecount.md)
    
- [<span data-ttu-id="d2ce1-156">IsComplete</span><span class="sxs-lookup"><span data-stu-id="d2ce1-156">IsComplete</span></span>](iscomplete.md)
    
- [<span data-ttu-id="d2ce1-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="d2ce1-157">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="d2ce1-158">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="d2ce1-158">PercentComplete</span></span>](percentcomplete.md)
    
- [<span data-ttu-id="d2ce1-159">状態</span><span class="sxs-lookup"><span data-stu-id="d2ce1-159">Status</span></span>](status.md)
    
- [<span data-ttu-id="d2ce1-160">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="d2ce1-160">StatusDescription</span></span>](statusdescription.md)
    
## <a name="see-also"></a><span data-ttu-id="d2ce1-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2ce1-161">See also</span></span>



<span data-ttu-id="d2ce1-162">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="d2ce1-162">[GetItem operation](getitem-operation.md)</span></span>


[<span data-ttu-id="d2ce1-163">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="d2ce1-163">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="d2ce1-164">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="d2ce1-164">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="d2ce1-165">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="d2ce1-165">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

