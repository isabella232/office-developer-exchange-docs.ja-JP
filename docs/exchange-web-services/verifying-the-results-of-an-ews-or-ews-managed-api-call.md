---
title: EWS または EWS マネージ API の呼び出しの結果の確認
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759193"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a><span data-ttu-id="988de-103">EWS または EWS マネージ API の呼び出しの結果の確認</span><span class="sxs-lookup"><span data-stu-id="988de-103">Verifying the results of an EWS or EWS Managed API call</span></span>

<span data-ttu-id="988de-104">EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="988de-104">Learn how to verify the results of your EWS or EWS Managed API calls.</span></span>
  
<span data-ttu-id="988de-105">プログラムが正しく実行されないと、役に立ちます、アプリケーションは、ネットワークとサーバーが送信する応答が送信される SOAP 要求を調べることで何が起こって参照してください。</span><span class="sxs-lookup"><span data-stu-id="988de-105">When things aren't working correctly, it helps to see what's going on by examining the SOAP requests that your application is sending over the network and the responses that the server is sending back.</span></span> <span data-ttu-id="988de-106">[ツールとリソースの EWS アプリケーションのトラブルシューティング](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)の資料には、キャプチャし、それらの SOAP 要求を表示するためのツールへのリンクが含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-106">The [tools and resources for troubleshooting EWS applications](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md) article includes links to tools to help capture and view those SOAP requests.</span></span> <span data-ttu-id="988de-107">要求および応答があれば後、検証するにはサーバーに送信する要求が正しく処理されたことでしょうか。</span><span class="sxs-lookup"><span data-stu-id="988de-107">After you've got the requests and the responses, how do you verify that the request you sent to the server was processed correctly?</span></span> <span data-ttu-id="988de-108">読み。</span><span class="sxs-lookup"><span data-stu-id="988de-108">Read on to find out.</span></span> 
  
<span data-ttu-id="988de-109">EWS 要求を送信する場合はしようとしている応答の応答メッセージごとに**ResponseClass**属性を確認することで、検証を開始します。</span><span class="sxs-lookup"><span data-stu-id="988de-109">If you're sending EWS requests, you're going to start your verification by checking the **ResponseClass** attribute for each response message in the response.</span></span> <span data-ttu-id="988de-110">通知する項目ごとに、操作が正常に完了したかどうか。</span><span class="sxs-lookup"><span data-stu-id="988de-110">That will tell you whether the operation completed successfully on each item.</span></span> 
  
<span data-ttu-id="988de-p103">メソッドが呼び出しているオブジェクトに応じて、EWS 、マネージ API を使用して要求を送信する場合に、応答オブジェクトを使用していくつかの検証を行うことができます。SOAP 応答には、EWS マネージ API の応答オブジェクトに含まれているもののスーパーセットが含まれているため、SOAP の応答も同様に確認することをお勧めします。SOAP 応答には、EWS マネージ API の応答オブジェクトより多くの情報が含まれているため、SOAP 応答で、検証を開始します。</span><span class="sxs-lookup"><span data-stu-id="988de-p103">Depending on the object that your method is calling, if you're using the EWS Managed API to send requests, you can do some verification using the response objects. But because the SOAP response contains a superset of what's included in the EWS Managed API response objects, you might want to look at the SOAP response as well. Because the SOAP response can often contain more information than the EWS Managed API response objects, start your verification with the SOAP response.</span></span>
  
## <a name="verifying-the-results-of-a-soap-response"></a><span data-ttu-id="988de-114">SOAP 応答の結果の確認</span><span class="sxs-lookup"><span data-stu-id="988de-114">Verifying the results of a SOAP response</span></span>
<span data-ttu-id="988de-115"><a name="bk_verifysoap"> </a></span><span class="sxs-lookup"><span data-stu-id="988de-115"></span></span>

<span data-ttu-id="988de-116">SOAP 応答を受信するときにまず最初に見て、 **ResponseClass**属性です。</span><span class="sxs-lookup"><span data-stu-id="988de-116">When you receive a SOAP response, the first thing to look at is the **ResponseClass** attribute.</span></span> <span data-ttu-id="988de-117">次の例のように、 [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx)要素では、 **ResponseMessageType**のインスタンスごとにこの属性が含まれます。</span><span class="sxs-lookup"><span data-stu-id="988de-117">This attribute is included in each **ResponseMessageType** instance in the [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) element, as shown in the following example.</span></span> 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

<span data-ttu-id="988de-118">SOAP 応答には、1 つの SOAP 応答で複数の応答メッセージが含まれている可能性があるため、各応答メッセージを個別に確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="988de-118">Because a SOAP response might contain multiple response messages in a single SOAP response, it's important to check each response message individually.</span></span>
  
<span data-ttu-id="988de-119">場合は、次のように、操作の応答の一部として、 **ResponseClass**を含む操作で作業することが考えられますのみ操作の**ResponseClass**を確認します。</span><span class="sxs-lookup"><span data-stu-id="988de-119">If you're working with an operation that includes a **ResponseClass** as part of the operation response, like the following, you might be tempted to only check the **ResponseClass** of the operation.</span></span> 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

<span data-ttu-id="988de-120">ただし、処理の状態はのみ最上位レベルの応答の形状が反映され、個々 のメッセージのすべての応答のステータスを反映しません。</span><span class="sxs-lookup"><span data-stu-id="988de-120">However, the operation status only reflects the shape of the top-level response and does not reflect the status of all the individual message responses.</span></span> <span data-ttu-id="988de-121">次の例では、 [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx)操作が**成功**すると、の**ResponseClass**を持つが、基の[DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx)要素は、**エラー**の**ResponseClass**値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="988de-121">In the following example, the [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) operation has a **ResponseClass** of **Success**, but the underlying [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) element has a **ResponseClass** value of **Error**.</span></span>
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="988de-122">したがって、EWS の SOAP 応答の操作の**ResponseClass**に依存できません -、操作に、項目の処理エラーが発生するかどうかを判断するには、各応答メッセージの**ResponseClass**を参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="988de-122">So for SOAP EWS responses, you can't rely on the **ResponseClass** of the operation - you have to look at the **ResponseClass** of each response message to determine whether the operation encountered any errors processing the items.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="988de-123">成功を確認する</span><span class="sxs-lookup"><span data-stu-id="988de-123">Verifying success</span></span>

<span data-ttu-id="988de-124">各**ResponseClass** **ResponseMessage**の各属性の設定を有効に**成功した場合**、すべての項目を正常に完了した操作と、次のタスク移動することができます。</span><span class="sxs-lookup"><span data-stu-id="988de-124">If each **ResponseClass** attribute for each **ResponseMessage** attribute is set to **Success**, the operation completed successfully on all the items, and you can move on to your next task.</span></span>
  
<span data-ttu-id="988de-125">次の例では、1 つのアイテムを取得するために[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx)操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="988de-125">The following example shows a successful response to a [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation request to retrieve a single item.</span></span> <span data-ttu-id="988de-126">**成功**に**ResponseClass**を設定すると、関連付けられている[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)は必ず設定する**NoError**を注意してください。</span><span class="sxs-lookup"><span data-stu-id="988de-126">Note that when the **ResponseClass** is set to **Success**, the associated [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) is always set to **NoError**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="988de-127">複数のアイテムを取得するために**GetItem**操作の要求に正常な応答を次に示します。</span><span class="sxs-lookup"><span data-stu-id="988de-127">The following is a successful response to a **GetItem** operation request to retrieve multiple items.</span></span> <span data-ttu-id="988de-128">[GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx)要素は、それぞれの**成功**は、 **ResponseClass**です。</span><span class="sxs-lookup"><span data-stu-id="988de-128">Each of the [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) elements has a **ResponseClass** of **Success**.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="handling-errors-and-warnings"></a><span data-ttu-id="988de-129">エラーおよび警告の処理</span><span class="sxs-lookup"><span data-stu-id="988de-129">Handling errors and warnings</span></span>

<span data-ttu-id="988de-130">応答を受信すると、**エラー**を**ResponseClass**属性が設定されて、1 つまたは複数のアイテムに対して操作が正常に完了しませんでした。</span><span class="sxs-lookup"><span data-stu-id="988de-130">When you receive a response and the **ResponseClass** attribute is set to **Error**, the operation did not complete successfully on one or more items.</span></span> <span data-ttu-id="988de-131">問題を修正し、要求、または失敗した要求の一部を再実行してください。</span><span class="sxs-lookup"><span data-stu-id="988de-131">Correct the issue and retry your request, or the part of your request that failed.</span></span> <span data-ttu-id="988de-132">**警告**値の**ResponseClass**属性の値、 [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx)操作のみが返されますを示し、そのエンティティは一意の id を解決できませんでした。</span><span class="sxs-lookup"><span data-stu-id="988de-132">A **ResponseClass** attribute value of **Warning** value is only returned by the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation, and indicates that the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="988de-133">他のすべての操作を無視できます。</span><span class="sxs-lookup"><span data-stu-id="988de-133">You can ignore it for all other operations.</span></span> 
  
<span data-ttu-id="988de-134">次の応答では、 **ResponseClass**属性は、**エラー**の値を持ちます。</span><span class="sxs-lookup"><span data-stu-id="988de-134">In the following response, the **ResponseClass** attribute has a value of **Error**.</span></span>
  
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

<span data-ttu-id="988de-135">この例では、EWS は、問題をデバッグする手がかりを提供します。</span><span class="sxs-lookup"><span data-stu-id="988de-135">In this example, EWS provides clues to debug the issue.</span></span> <span data-ttu-id="988de-136">**ResponseClass**属性は、**エラー**の値を持つと、は、該当する場合の応答で以下の要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="988de-136">When the **ResponseClass** attribute has a value of **Error**, the following additional elements are included in the response when applicable:</span></span>
  
- <span data-ttu-id="988de-137">[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)エラーを説明します。</span><span class="sxs-lookup"><span data-stu-id="988de-137">[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="988de-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) -追加のトラブルシューティング リソースの検索に使用することができます、エラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-138">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="988de-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) -エラーが発生した要素を識別します。</span><span class="sxs-lookup"><span data-stu-id="988de-139">[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — Identifies the elements that caused the error.</span></span> 
    
- <span data-ttu-id="988de-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) -使用されていません。</span><span class="sxs-lookup"><span data-stu-id="988de-140">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — Unused.</span></span> 
    
<span data-ttu-id="988de-141">これらの要素で提供される情報を使用すると、お客様の問題を調査します。</span><span class="sxs-lookup"><span data-stu-id="988de-141">You can use the information provided in these elements to investigate your issue.</span></span> <span data-ttu-id="988de-142">前の例では、**メッセージ テキスト**は、プロパティがオブジェクトの種類に対して有効でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="988de-142">In the previous example, the **MessageText** indicates that the property isn't valid for the object type.</span></span> <span data-ttu-id="988de-143">要求が電子メール メッセージを取得したが、プロパティが含まれて**AssociatedCalendarItemId**では、予定アイテムの有効なをします。</span><span class="sxs-lookup"><span data-stu-id="988de-143">The request was to get an email message, but the property set included the **AssociatedCalendarItemId**, which is only valid for appointment items.</span></span>
  
<span data-ttu-id="988de-144">次の例では、複数の電子メール アイテムを取得するためのバッチ操作の一部として受信したエラーを示します。</span><span class="sxs-lookup"><span data-stu-id="988de-144">The following example shows an error that was received as part of a batched operation to get multiple email items.</span></span> <span data-ttu-id="988de-145">最初の項目が正常に取得され、 **ResponseClass**が**成功した場合**に設定します。</span><span class="sxs-lookup"><span data-stu-id="988de-145">The first item was retrieved successfully and the **ResponseClass** is set to **Success**.</span></span> <span data-ttu-id="988de-146">2 番目の項目が見つかりませんでしたと**ResponseClass**は**エラー**に設定します。</span><span class="sxs-lookup"><span data-stu-id="988de-146">The second item could not be found, and the **ResponseClass** is set to **Error**.</span></span>
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="988de-147">要求されたバッチ要求の 1 つまたは複数の項目を処理できませんと、失敗した各アイテムのエラーが返されるバッチ内の項目の残りの部分が期待どおりに処理されます。</span><span class="sxs-lookup"><span data-stu-id="988de-147">When one or more items in a batched request can't be processed as requested, an error is returned for each item that failed, and the rest of the items in the batch are processed as expected.</span></span> <span data-ttu-id="988de-148">バッチ処理でエラーが発生するアイテムが削除された、したがってことはできません送信、取得、または更新、または場合は、項目別のフォルダーに移動し、新しい項目の id。</span><span class="sxs-lookup"><span data-stu-id="988de-148">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID.</span></span> <span data-ttu-id="988de-149">操作はいくつかのアイテムを完了し、1 つまたは複数のアイテムを処理できないときにエラーが返されない、ためすることが重要、次の操作を移動する前に、 **ResponseClass**の各属性を確認します。</span><span class="sxs-lookup"><span data-stu-id="988de-149">Because the operation will complete for some items and not return an error when one or more items can't be processed, it's important to check each **ResponseClass** attribute before you move on to your next operation.</span></span> 
  
<span data-ttu-id="988de-150">応答の要素によって提供される情報は、要求を修正するか、それ以外の場合、ブロックを解除する場合、は、[次の手順](#bk_nextsteps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="988de-150">If the information provided by the response elements doesn't help you correct your request or otherwise unblock you, see [Next steps](#bk_nextsteps).</span></span>
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a><span data-ttu-id="988de-151">EWS マネージ API メソッド呼び出しの結果の確認</span><span class="sxs-lookup"><span data-stu-id="988de-151">Verifying the results of an EWS Managed API method call</span></span>
<span data-ttu-id="988de-152"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="988de-152"></span></span>

<span data-ttu-id="988de-153">EWS のマネージ API を使用している[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトでメソッドを呼び出す場合、おそらくメソッドは、 [ServiceResponse](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx)オブジェクトのコレクションまたはコレクションを含む[ServiceResponseCollection](http://msdn.microsoft.com/ja-jp/library/dd633715%28v=exchg.80%29.aspx)オブジェクトを取得するには、オブジェクトは、 **ServiceResponse**オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="988de-153">If you're using the EWS Managed API and calling a method on an [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, your method will likely return a [ServiceResponseCollection](http://msdn.microsoft.com/ja-jp/library/dd633715%28v=exchg.80%29.aspx) object, which contains a collection of [ServiceResponse](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) objects, or a collection of objects derived from the **ServiceResponse** objects.</span></span> <span data-ttu-id="988de-154">**ServiceResponseCollection**と**ServiceResponse**オブジェクトが含まれているには、結果を確認に使用できるメソッドの呼び出しの結果に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-154">The **ServiceResponseCollection** and included **ServiceResponse** objects contain information about the result of the method call, which you can use to verify your results.</span></span> 
  
<span data-ttu-id="988de-155">EWS のマネージ API を使用している[アイテム](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)オブジェクト、またはそのいずれかの派生オブジェクトでメソッドを呼び出すと、可能性の高い方法を成功すると、確認の応答オブジェクトを返さないですが、[例外](http://msdn.microsoft.com/ja-jp/library/c18k6c59)をスローするメソッドが完了しない場合は正常にします。</span><span class="sxs-lookup"><span data-stu-id="988de-155">If you're using the EWS Managed API and calling a method on an [Item](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object, or one of the derived objects, the method likely does not return a response object to check for success, but does throw an [Exception](http://msdn.microsoft.com/ja-jp/library/c18k6c59) if the method does not complete successfully.</span></span> 
  
### <a name="verifying-success"></a><span data-ttu-id="988de-156">成功を確認する</span><span class="sxs-lookup"><span data-stu-id="988de-156">Verifying success</span></span>

<span data-ttu-id="988de-157">EWS のマネージ API を使用する利点の 1 つは、1 つの応答で複数のアイテムを処理するとき、全体のステータスが提供されることです。</span><span class="sxs-lookup"><span data-stu-id="988de-157">One benefit of using the EWS Managed API is that it provides an overall status when dealing with multiple items in one response.</span></span> <span data-ttu-id="988de-158">メソッドを返す場合、 **ServiceResponseCollection**、 **ServiceResponseCollection**の[OverallResult](http://msdn.microsoft.com/ja-jp/library/dd634515%28v=exchg.80%29.aspx)プロパティが[ServiceResult.Success](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx)に等しいことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="988de-158">So if the method you called returns a **ServiceResponseCollection**, you can check that the [OverallResult](http://msdn.microsoft.com/ja-jp/library/dd634515%28v=exchg.80%29.aspx) property of the **ServiceResponseCollection** is equal to [ServiceResult.Success](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="988de-159">バッチ プロセスですべての項目が正常に終了した場合は、**ServiceResponse**の各オブジェクトを個別に確認する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="988de-159">If so, all the items in the batched process were completed successfully; you don't have to check each **ServiceResponse** object individually.</span></span> <span data-ttu-id="988de-160">**OverallResult**プロパティが**ServiceResult.Success**に設定されていない場合は、[エラーまたは警告を処理](#bk_ewsmaerrors)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="988de-160">If the **OverallResult** property is not set to **ServiceResult.Success**, you have to [handle the error or warning](#bk_ewsmaerrors).</span></span>
  
<span data-ttu-id="988de-161">呼び出し先のメソッドは**ServiceResponseCollection**を返しませんが、 **ServiceResponse**オブジェクトを返しますが場合、は、 **Result**プロパティの値を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="988de-161">If the method you're calling does not return a **ServiceResponseCollection**, but does return a **ServiceResponse** object, you have to check the value of the **Result** property.</span></span> <span data-ttu-id="988de-162">**結果**の値は、**成功した場合**に設定されている場合、メソッドは正常に終了しましたが知っています。</span><span class="sxs-lookup"><span data-stu-id="988de-162">If the **Result** value is set to **Success**, you know the method completed successfully.</span></span>
  
<span data-ttu-id="988de-163">呼び出し先のメソッドが戻り値を持たない場合、EWS のマネージ API を使用して成功を確認する方法は実際にはありません。</span><span class="sxs-lookup"><span data-stu-id="988de-163">If the method you're calling has no return value, there's really no way to check for success via the EWS Managed API.</span></span> <span data-ttu-id="988de-164">例外がスローされない限りは、メソッドが正常に完了したと想定できます。</span><span class="sxs-lookup"><span data-stu-id="988de-164">As long as an exception is not thrown, you can assume the method completed successfully.</span></span> <span data-ttu-id="988de-165">追加の検証をすることも[結果を確認するのには、SOAP 応答を確認](#bk_verifysoap)します。</span><span class="sxs-lookup"><span data-stu-id="988de-165">For additional validation, you can also [check the SOAP response to verify the results](#bk_verifysoap).</span></span>
  
### <a name="handling-errors-warnings-and-exceptions"></a><span data-ttu-id="988de-166">エラー、警告、および例外の処理</span><span class="sxs-lookup"><span data-stu-id="988de-166">Handling errors, warnings, and exceptions</span></span>
<span data-ttu-id="988de-167"><a name="bk_ewsmaerrors"> </a></span><span class="sxs-lookup"><span data-stu-id="988de-167"></span></span>

<span data-ttu-id="988de-168">EWS のマネージ API コードは、**例外**をスローする場合は、エラーの原因を特定するのには[Exception.Message](http://msdn.microsoft.com/ja-jp/library/9btwf6wk)値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="988de-168">If your EWS Managed API code throws an **Exception**, you can use the [Exception.Message](http://msdn.microsoft.com/ja-jp/library/9btwf6wk) value to determine the source of the error.</span></span> <span data-ttu-id="988de-169">**メッセージ**プロパティには、基になる SOAP 応答の[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)の要素の内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-169">The **Message** property contains the contents of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) element in the underlying SOAP response.</span></span> <span data-ttu-id="988de-170">さらに、例外の場合は、最も一般的な例外の 1 つ、 [ServiceResponseException](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)オブジェクトの種類取得することも、基になる SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素、および[応答](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx)に含まれている[エラー コード](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx)関連する[ServiceResponse](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx)オブジェクトを識別するプロパティです。</span><span class="sxs-lookup"><span data-stu-id="988de-170">In addition, if the exception is of type [ServiceResponseException](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) object, one of the most common exceptions, you can also retrieve the [ErrorCode](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx) contained in the underlying SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element, and the [Response](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) property that identifies the associated [ServiceResponse](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="988de-171">次のコードでは、キャッチし、 **ServiceResponseException**の内容を表示する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="988de-171">The following code shows how to catch and display the contents of a **ServiceResponseException**.</span></span> 
  
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

<span data-ttu-id="988de-172">**ServiceResponseCollection**内の各オブジェクトをループ処理する必要がある場合は、呼び出されたメソッドは**ServiceResponseCollection**を返し、**警告**または**エラー**を**OverallResult**プロパティの値は、エラーを検索します。</span><span class="sxs-lookup"><span data-stu-id="988de-172">If the method you called returns a **ServiceResponseCollection**, and the value of the **OverallResult** property is equal to **Warning** or **Error**, you'll have to loop through each object in the **ServiceResponseCollection** to find the error.</span></span> <span data-ttu-id="988de-173">少なくとも 1 つの応答には、**結果**値が**警告**にセットし、その他のすべての応答に**成功**] に設定の**結果**の値がある場合、 **OverallResult**プロパティは**警告**を設定します。</span><span class="sxs-lookup"><span data-stu-id="988de-173">The **OverallResult** property is set to **Warning** if at least one response has its **Result** value set to **Warning** and all other responses have their **Result** values set to **Success**.</span></span> <span data-ttu-id="988de-174">**OverallResult**プロパティを少なくとも 1 つの応答には、**結果**値が**Error**に設定されている場合、**エラー**に設定されます。</span><span class="sxs-lookup"><span data-stu-id="988de-174">The **OverallResult** property is set to **Error** if at least one response has its **Result** value set to **Error**.</span></span> <span data-ttu-id="988de-175">**OverallResult**設定すると、**警告**または**エラー**を適切な**ServiceResponse**オブジェクトに対して次のプロパティが設定されます。</span><span class="sxs-lookup"><span data-stu-id="988de-175">When the **OverallResult** is set to **Warning** or **Error**, the following properties are set on the **ServiceResponse** objects as appropriate:</span></span> 
  
- <span data-ttu-id="988de-176">[エラー コード](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)など、追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-176">[ErrorCode](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — Contains the error code, which can be used to find additional troubleshooting resources.</span></span> 
    
- <span data-ttu-id="988de-177">[ErrorDetails](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) - **ErrorCodes**をいくつかのエラーの詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="988de-177">[ErrorDetails](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — Contains details about the error for some **ErrorCodes**.</span></span> <span data-ttu-id="988de-178">たとえば、エラー コードが**ErrorRecurrenceHasNoOccurrence**の場合は、 **ErrorDetails**キーが含まれます**EffectiveStartDate**と**EffectiveEndDate**。</span><span class="sxs-lookup"><span data-stu-id="988de-178">For example, when the error code is **ErrorRecurrenceHasNoOccurrence**, the **ErrorDetails** will contain keys for **EffectiveStartDate** and **EffectiveEndDate**.</span></span> 
    
- <span data-ttu-id="988de-179">[エラー メッセージ](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx): エラーを説明します。</span><span class="sxs-lookup"><span data-stu-id="988de-179">[ErrorMessage](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — Describes the error.</span></span> 
    
- <span data-ttu-id="988de-180">[ErrorProperties](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) -可能な場合は、エラーの原因となったプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="988de-180">[ErrorProperties](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — If available, identifies the properties that caused the error.</span></span> <span data-ttu-id="988de-181">などのエラー コードが**ErrorInvalidPropertyForOperation**の場合は、 **ErrorProperties**は、要求の無効なプロパティの定義を含みます。</span><span class="sxs-lookup"><span data-stu-id="988de-181">For example, when the error code is **ErrorInvalidPropertyForOperation**, **ErrorProperties** contains the definition of the property that was invalid for the request.</span></span> 
    
- <span data-ttu-id="988de-182">[結果](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx): 含まれる**エラー**または問題が発生したときに**警告**します。</span><span class="sxs-lookup"><span data-stu-id="988de-182">[Result](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — Contains **Error** or **Warning** when an issue is encountered.</span></span> 
    
<span data-ttu-id="988de-183">**ServiceResponse**プロパティによって提供される情報は、メソッドの呼び出しを修正またはブロックを解除して、**エラー コード**値の詳細情報を確認する[次の手順](#bk_nextsteps)を参照してくださいに十分な情報を提供しません。 場合、</span><span class="sxs-lookup"><span data-stu-id="988de-183">If the information provided by the **ServiceResponse** properties doesn't provide enough information to correct your method call or unblock you, see [Next steps](#bk_nextsteps) to dig up more information on **ErrorCode** values.</span></span> 
  
## 
<span data-ttu-id="988de-184"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="988de-184"></span></span>

<span data-ttu-id="988de-185">次のトピックで、トラブルシューティングに関する追加の情報を検索できます。</span><span class="sxs-lookup"><span data-stu-id="988de-185">You can look up additional troubleshooting information in the following topics:</span></span>
  
- <span data-ttu-id="988de-186">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素</span><span class="sxs-lookup"><span data-stu-id="988de-186">[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element</span></span> 
    
- <span data-ttu-id="988de-187">[サービス エラー](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)の列挙</span><span class="sxs-lookup"><span data-stu-id="988de-187">[ServiceError](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) enumeration</span></span> 
    
- [<span data-ttu-id="988de-188">EWS プロパティに関連するエラー</span><span class="sxs-lookup"><span data-stu-id="988de-188">EWS property-related errors</span></span>](ews-property-related-errors.md)
    
<span data-ttu-id="988de-189">さらに、要求で実現したい内容によっては、次のトピックでエラー コードに関するその他の有用な情報を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="988de-189">In addition, depending on what you're trying to accomplish in your request, you might find additional helpful information about the error code in the following topics:</span></span>
  
- [<span data-ttu-id="988de-190">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="988de-190">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="988de-191">Exchange における EWS での通知関連エラーの処理</span><span class="sxs-lookup"><span data-stu-id="988de-191">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="988de-192">Exchange EWS での同期に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="988de-192">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="988de-193">Exchange EWS での削除に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="988de-193">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="988de-194">関連項目</span><span class="sxs-lookup"><span data-stu-id="988de-194">See also</span></span>


- [<span data-ttu-id="988de-195">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="988de-195">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="988de-196">Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース</span><span class="sxs-lookup"><span data-stu-id="988de-196">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

