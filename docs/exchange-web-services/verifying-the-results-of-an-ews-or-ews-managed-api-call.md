---
title: EWS または EWS マネージ API の呼び出しの結果の確認
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: be8e76898dd111a6dec33d4a57d9d50a2a935390
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457397"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="e8d47-103">EWS または EWS マネージ API の呼び出しの結果の確認</span><span class="sxs-lookup"><span data-stu-id="e8d47-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="e8d47-104">EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="e8d47-p101">プログラムが正しく実行されないとき、アプリケーションがネットワーク経由で送信している SOAP 要求とサーバーが送信している応答を調べることで、何が起こったか理解できます。「[EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)」の記事では、それらの SOAP 要求をキャプチャして表示するためのツールへのリンクを掲載しています。要求および応答を取得した後で、サーバーに送信した要求が正しく処理されたことを検証するには、どうしたらよいでしょうか。続きを読んで確認してください。</span><span class="sxs-lookup"><span data-stu-id="e8d47-p101">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back. The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests. After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly? Read on to find out.</span></span> 
  
<span data-ttu-id="e8d47-109">EWS 要求を送信している場合は、応答の各応答メッセージの **ResponseClass** 属性を確認して、検証を開始します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="e8d47-110">これにより、アイテムごとに操作が正常に完了したかどうかがわかります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="e8d47-p103">メソッドが呼び出しているオブジェクトに応じて、EWS 、マネージ API を使用して要求を送信する場合に、応答オブジェクトを使用していくつかの検証を行うことができます。SOAP 応答には、EWS マネージ API の応答オブジェクトに含まれているもののスーパーセットが含まれているため、SOAP の応答も同様に確認することをお勧めします。SOAP 応答には、EWS マネージ API の応答オブジェクトより多くの情報が含まれているため、SOAP 応答で、検証を開始します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-p103">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects. But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well. Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="e8d47-114">SOAP 応答の結果の確認</span><span class="sxs-lookup"><span data-stu-id="e8d47-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="e8d47-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="e8d47-115"><a name="bk_verifysoap"> </a></span></span>

<span data-ttu-id="e8d47-116">SOAP 応答を受信するとき、最初に **ResponseClass** 属性を確認します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="e8d47-117">この属性は、次の例に示すように、[ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) 要素の各 **ResponseMessageType** インスタンスに含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](https://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="e8d47-118">SOAP 応答には、1 つの SOAP 応答で複数の応答メッセージが含まれている可能性があるため、各応答メッセージを個別に確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="e8d47-119">**ResponseClass** が操作の応答の一部として含まれている操作を使用している場合、次のように、操作の **ResponseClass** のみを確認したくなるかもしれません。 </span><span class="sxs-lookup"><span data-stu-id="e8d47-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="e8d47-120">しかし、操作の状態は最上位レベルの応答の形状のみを反映し、個々のメッセージのすべての応答のステータスを反映しません。</span><span class="sxs-lookup"><span data-stu-id="e8d47-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="e8d47-121">次の例では、[AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) 操作には **Success** の **ResponseClass** がありますが、基になる [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) 要素には **Error** の値の **ResponseClass** があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-121">In the following example, the [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](https://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

<span data-ttu-id="e8d47-122">このため、SOAP EWS の応答では、操作の **ResponseClass** を信頼できず、操作でアイテムの処理中にエラーが発生したかどうかを判断するには、各応答メッセージの **ResponseClass** を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="e8d47-123">成功を確認する</span><span class="sxs-lookup"><span data-stu-id="e8d47-123">Verifying success</span></span>

<span data-ttu-id="e8d47-124">各 **ResponseMessage** 属性の **ResponseClass** 属性が **Success** に設定されている場合、すべてのアイテムで操作が正常に完了し、次のタスクに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="e8d47-125">次の例は、1 つのアイテムを取得するための [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-125">The following example shows a successful response to a [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="e8d47-126">**ResponseClass** が **Success** に設定されている場合、関連付けられた [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) は常に **NoError** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

<span data-ttu-id="e8d47-127">次の例は、複数のアイテムを取得するための **GetItem** 操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="e8d47-128">それぞれの [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) 要素には、**Success** の **ResponseClass** があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-128">Each of the [GetItemResponseMessage](https://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="e8d47-129">エラーおよび警告の処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-129">Handling errors and warnings</span></span>

<span data-ttu-id="e8d47-130">応答を受信して **ResponseClass** 属性が **Error** に設定されている場合、1 つ以上のアイテムで操作が正常に完了していません。</span><span class="sxs-lookup"><span data-stu-id="e8d47-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="e8d47-131">問題を修正し、要求または失敗した要求の部分を再実行してください。</span><span class="sxs-lookup"><span data-stu-id="e8d47-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="e8d47-132">**Warning** の値の **ResponseClass** 属性の値は、[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作によってのみ返され、エンティティを一意の識別子に解決できなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="e8d47-133">これは他のすべての操作では無視できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="e8d47-134">次の応答で、**ResponseClass** 属性の値は **Error**です。</span><span class="sxs-lookup"><span data-stu-id="e8d47-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

<span data-ttu-id="e8d47-135">この例では、EWS が問題をデバッグする手がかりを提供します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="e8d47-136">**ResponseClass** 属性の値が **Error** のとき、該当する場合に次の追加の要素が応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="e8d47-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — エラーを説明します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-137">[MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="e8d47-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — 追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-138">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="e8d47-139">[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — エラーが発生した要素を識別します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-139">[MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="e8d47-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — 使用されていません。</span><span class="sxs-lookup"><span data-stu-id="e8d47-140">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="e8d47-141">これらの要素で提供される情報を使用して、問題を調査できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="e8d47-142">前の例は、**MessageText** はプロパティがオブジェクトの種類に対して有効でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="e8d47-143">要求はメール メッセージを取得することでしたが、予定アイテムに対してのみ有効な **AssociatedCalendarItemId** がプロパティ セットに含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="e8d47-144">次の例は、複数の電子メール アイテムを取得するためのバッチ操作の一部として受信したエラーを示します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="e8d47-145">最初のアイテムが正常に取得され、**ResponseClass** が **Success** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="e8d47-146">2 番目のアイテムが見つからなかったため、**ResponseClass** が **Error** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
```XML
<m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

<span data-ttu-id="e8d47-147">バッチ要求の 1 つ以上のアイテムを要求どおりに処理できないと、失敗したアイテムごとにエラーが返されます。バッチ処理のそれ以外のアイテムは予期したとおりに処理されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="e8d47-148">対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなったりすると、バッチ処理でエラーが生じます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="e8d47-149">操作がいくつかのアイテムでは完了した場合、1 つ以上のアイテムを処理できないときでもエラーが返されないため、次の操作に進む前に、それぞれの **ResponseClass** 属性を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="e8d47-150">応答要素によって提供される情報で、要求の修正またはブロックの解除ができない場合は、[次の手順](#bk_nextsteps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8d47-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="e8d47-151">EWS マネージ API メソッド呼び出しの結果の確認</span><span class="sxs-lookup"><span data-stu-id="e8d47-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="e8d47-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="e8d47-152"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="e8d47-153">EWS マネージ API を使用して [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトにメソッドを呼び出している場合、メソッドは、[ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) オブジェクトのコレクション、または **ServiceResponse** から派生したオブジェクトのコレクションを含む [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) オブジェクトを返すはずです。</span><span class="sxs-lookup"><span data-stu-id="e8d47-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="e8d47-154">**ServiceResponseCollection** および含まれる **ServiceResponse** オブジェクトには、メソッドの呼び出しの結果に関する情報が含まれています。この情報を使って、結果を確認できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="e8d47-155">EWS マネージ API を使用して [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトのメソッド、または派生オブジェクトの 1 つを呼び出している場合、メソッドは正常に完了したことを確認するための応答オブジェクトを返さず、メソッドが正常に完了しなかった場合に [Exception](https://msdn.microsoft.com/library/c18k6c59) をスローします。</span><span class="sxs-lookup"><span data-stu-id="e8d47-155">If you're using the EWS Managed API and calling a method on an [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](https://msdn.microsoft.com/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="e8d47-156">成功を確認する</span><span class="sxs-lookup"><span data-stu-id="e8d47-156">Verifying success</span></span>

<span data-ttu-id="e8d47-157">EWS マネージ API を使用する利点の 1 つは、1 つの応答で複数のアイテムを処理するとき、全体のステータスが提供されることです。</span><span class="sxs-lookup"><span data-stu-id="e8d47-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="e8d47-158">それで、呼び出したメソッドが **ServiceResponseCollection** を返した場合、**ServiceResponseCollection** の [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) のプロパティが [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx) に等しいかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="e8d47-159">等しい場合、バッチ プロセスのすべてのアイテムが正常に終了しています。**ServiceResponse** オブジェクトを個別に確認する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="e8d47-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="e8d47-160">**OverallResult** プロパティが **ServiceResult.Success** に設定されていない場合、[エラーまたは警告を処理する](#bk_ewsmaerrors)必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="e8d47-161">呼び出しているメソッドが **ServiceResponseCollection** を返さず、**ServiceResponse** オブジェクトを返す場合は、**Result** プロパティの値を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="e8d47-162">**Result** 値が **Success** に設定されている場合、メソッドが正常に完了したことがわかります。</span><span class="sxs-lookup"><span data-stu-id="e8d47-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="e8d47-p116">呼び出しているメソッドに戻り値がない場合、EWS マネージ API によって成功を確認する方法は実際にはありません。例外がスローされない限り、メソッドが正常に完了したと想定できます。追加の検証をする場合は、[SOAP 応答を確認して結果を確認](#bk_verifysoap)することもできます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-p116">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API. As long as an exception is not thrown, you can assume the method completed successfully. For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="e8d47-166">エラー、警告、および例外の処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="e8d47-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="e8d47-167"><a name="bk_ewsmaerrors"> </a></span></span>

<span data-ttu-id="e8d47-168">EWS マネージ API のコードが **Exception** をスローした場合、[Exception.Message](https://msdn.microsoft.com/library/9btwf6wk) の値を使用して、エラーの原因を特定できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](https://msdn.microsoft.com/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="e8d47-169">**Message** プロパティには、基になる SOAP 応答内の [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) 要素の内容が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-169">The **Message** property contains the contents of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="e8d47-170">さらに、例外が最も一般的な例外の [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) オブジェクト型である場合、基になる SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素に含まれる [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx)、および関連付けられた [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) オブジェクトを識別する [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) プロパティも取得できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-170">In addition, if the exception is of type [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="e8d47-171">次のコードは、**ServiceResponseException** の内容をキャッチして表示する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

<span data-ttu-id="e8d47-172">呼び出したメソッドが **ServiceResponseCollection** を返し、**OverallResult** プロパティの値が **Warning** または **Error** と等しい場合は、**ServiceResponseCollection** の各オブジェクト内をループして、エラーを検出します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="e8d47-173">少なくとも 1 つの応答で **Result** の値が **Warning** に設定され、他のすべての応答で **Result** の値が **Success** に設定されている場合は、**OverallResult** プロパティは **Warning** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="e8d47-174">少なくとも 1 つの応答で **Result** の値が **Error** に設定されている場合は、**OverallResult** プロパティは **Error** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="e8d47-175">**OverallResult** が **Warning** または **Error** に設定されている場合、以下のプロパティが **ServiceResponse** オブジェクトに適宜設定されます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="e8d47-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — 追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-176">[ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="e8d47-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — いくつかの **ErrorCodes** のエラーに関する詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e8d47-177">[ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="e8d47-178">たとえば、エラー コードが **ErrorRecurrenceHasNoOccurrence** の場合、**ErrorDetails** には **EffectiveStartDate** と **EffectiveEndDate** のキーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="e8d47-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — エラーを説明します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-179">[ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="e8d47-180">[ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — 可能な場合は、エラーの原因となったプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e8d47-180">[ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="e8d47-181">たとえば、エラー コードが **ErrorInvalidPropertyForOperation** の場合、**ErrorProperties** には要求に無効なプロパティの定義が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="e8d47-182">[Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — 問題が発生したときに **Error** または **Warning** が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-182">[Result](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="e8d47-183">**ServiceResponse** プロパティによって提供される情報が、メソッドの呼び出しの修正、またはブロックの解除を行うための十分な情報を提供していない場合は、「[次の手順](#bk_nextsteps)」で **ErrorCode** の値の詳細な情報を確認してください。</span><span class="sxs-lookup"><span data-stu-id="e8d47-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="e8d47-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="e8d47-184"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="e8d47-185">次のトピックで、トラブルシューティングに関する追加の情報を検索できます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="e8d47-186">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素</span><span class="sxs-lookup"><span data-stu-id="e8d47-186">[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="e8d47-187">[ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 列挙体</span><span class="sxs-lookup"><span data-stu-id="e8d47-187">[ServiceError](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="e8d47-188">EWS プロパティ関連のエラー</span><span class="sxs-lookup"><span data-stu-id="e8d47-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="e8d47-189">さらに、要求で実現したい内容によっては、次のトピックでエラー コードに関するその他の有用な情報を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="e8d47-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="e8d47-190">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="e8d47-191">Exchange の EWS での通知に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="e8d47-192">Exchange の EWS での同期に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="e8d47-193">Exchange の EWS での削除に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="e8d47-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="e8d47-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8d47-194">See also</span></span>


- [<span data-ttu-id="e8d47-195">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="e8d47-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="e8d47-196">Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース</span><span class="sxs-lookup"><span data-stu-id="e8d47-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

