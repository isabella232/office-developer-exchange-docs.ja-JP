---
title: Exchange で EWS を使用してバッチ処理でメール メッセージを処理する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで複数のメール メッセージの作成、取得、更新、削除をバッチ処理する方法について説明します。
ms.openlocfilehash: b7dcc8f0961a34061b0476e2136193bf21731d99
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354044"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="070d5-103">Exchange で EWS を使用してバッチ処理でメール メッセージを処理する</span><span class="sxs-lookup"><span data-stu-id="070d5-103">How to: Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="070d5-104">Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで複数のメール メッセージの作成、取得、更新、削除をバッチ処理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="070d5-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="070d5-105">EWS マネージ API または EWS を使用すると、メール メッセージのバッチ操作を行い、クライアントが Exchange サーバーを呼び出す回数を減らせます。</span><span class="sxs-lookup"><span data-stu-id="070d5-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="070d5-106">EWS マネージ API を使用してメール メッセージの作成、取得、更新、削除、送信のバッチ操作を行う場合、[ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。1 つのメール メッセージを対象とする場合には [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="070d5-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="070d5-107">EWS を使用する場合は、同じ操作を使用して 1 つのメール メッセージの処理とバッチ処理のどちらも行えます。</span><span class="sxs-lookup"><span data-stu-id="070d5-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span> 
  
<span data-ttu-id="070d5-108">**表 1. メール メッセージをバッチ処理するための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="070d5-108">**Table 1.  EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="070d5-109">**目的**</span><span class="sxs-lookup"><span data-stu-id="070d5-109">**In order to…**</span></span>|<span data-ttu-id="070d5-110">**使用する EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="070d5-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="070d5-111">**使用する EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="070d5-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="070d5-112">バッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="070d5-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="070d5-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="070d5-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="070d5-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="070d5-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="070d5-115">バッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="070d5-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="070d5-116">ExchangeService.BindToItems</span><span class="sxs-lookup"><span data-stu-id="070d5-116">ExchangeService.BindToItems</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="070d5-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="070d5-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="070d5-118">バッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="070d5-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="070d5-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="070d5-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/ja-JP/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="070d5-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="070d5-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="070d5-121">バッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="070d5-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="070d5-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="070d5-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/ja-JP/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="070d5-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="070d5-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="070d5-124">この記事では、EWS マネージ API または EWS を使用してメール メッセージのバッチ処理を行うための基本的なタスクの実行方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="070d5-124">In this article, you’ll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="070d5-125">EWS マネージ API を使用してバッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="070d5-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="070d5-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-126"></span></span>

<span data-ttu-id="070d5-127">次の例に示されているように、EWS マネージ API **CreateItems** メソッドを使用すると、バッチ処理でメッセージを作成できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-127">You can get email messages in batches by using the EWS Managed API  UpdateItems http://msdn.microsoft.com/en-us/library/dd634705(v=exchg.80).aspx  method, as shown in the following example.</span></span> <span data-ttu-id="070d5-128">この例では、3 つの [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトをローカルに作成し、それぞれのメッセージをコレクションに追加してから、メッセージのコレクションをパラメーターにして **CreateItems** メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="070d5-128">This example creates three [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span> 
  
<span data-ttu-id="070d5-129">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="070d5-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<ItemId> CreateDraftEmailInBatch(ExchangeService service)
{
    // These are unsaved local instances of an EmailMessage object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    EmailMessage message1 = new EmailMessage(service);
    EmailMessage message2 = new EmailMessage(service);
    EmailMessage message3 = new EmailMessage(service);
    // Set the properties on the first message.
    message1.Subject = "Project priorities";
    message1.Body = "(1) Buy pizza, (2) Eat pizza";
    message1.ToRecipients.Add("sadie@contoso.com");
    // Set the properties on the second message.
    message2.Subject = "Company Soccer Team";
    message2.Body = "Are you interested in joining?";
    message2.ToRecipients.Add("magdalena@contoso.com");
    // Set the properties on the third message.
    message3.Subject = "Code Blast";
    message3.Body = "Are you interested in getting together to finish the methods for the ContosoLive project?";
    message3.ToRecipients.Add("mack@contoso.com");
    // Add the EmailMessage objects to a collection.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>() { message1, message2, message3 };
    // Create the batch of email messages on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.Drafts, MessageDisposition.SaveOnly, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created email messages.
    foreach (EmailMessage message in messageItems)
    {
        try
        {
            itemIds.Add(message.Id);
            Console.WriteLine("Email message '{0}' created successfully.", message.Subject);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating message {0}: {1}", message.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Check for success of the CreateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created messages were successfully saved to the Drafts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each email.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

<span data-ttu-id="070d5-130">この例では、下書きフォルダーにメッセージを保存しますが、メッセージは送信しません。</span><span class="sxs-lookup"><span data-stu-id="070d5-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages. For more about how to send the messages, see Send email messages in batches.</span></span> <span data-ttu-id="070d5-131">メッセージを送信する方法の詳細については、「[EWS マネージ API を使用してバッチ処理でメール メッセージを送信する](#bk_sendewsma)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>
  
## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="070d5-132">EWS を使用してバッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="070d5-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="070d5-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-133"></span></span>

<span data-ttu-id="070d5-p104">次のコード例に示されているように、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS 操作を使用して、バッチ処理でメール メッセージを作成できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを作成](#bk_createewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。 </span><span class="sxs-lookup"><span data-stu-id="070d5-p104">You can create email messages in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example. This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>magdalena@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Are you interested in getting together to finish the methods for the ContosoLive project?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="070d5-136">サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの新しいメッセージが正常に作成および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="070d5-136">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span> 
  
<span data-ttu-id="070d5-137">この例では、下書きフォルダーにメッセージを保存しますが、メッセージは送信しません。</span><span class="sxs-lookup"><span data-stu-id="070d5-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages. For more about how to send the messages, see Send email messages in batches.</span></span> <span data-ttu-id="070d5-138">メッセージを送信する方法の詳細については、「[EWS を使用してバッチ処理でメール メッセージを送信する](#bk_sendews)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="070d5-139">EWS マネージ API を使用してバッチ処理でメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="070d5-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="070d5-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-140"></span></span>

<span data-ttu-id="070d5-141">バッチ処理でメール メッセージを送信するには、バッチ処理でのメール メッセージの作成に使用するコードと同じコードを使用します。ただし、一部の [CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) メソッドのパラメーターは変更します。</span><span class="sxs-lookup"><span data-stu-id="070d5-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="070d5-142">そのため、EWS マネージ API を使用してメール メッセージを送信するには、[バッチ処理でのメール メッセージの作成](#bk_createewsma)に使用するコードを使用して、**CreateItems** メソッドへの呼び出しを次の例の呼び出しに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="070d5-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="070d5-143">この例では、メッセージは送信済みアイテム フォルダーに作成されます。またメッセージがローカルに保存されるだけでなく送信されるように、メッセージの処理方法を [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx) に変更しています。</span><span class="sxs-lookup"><span data-stu-id="070d5-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="070d5-144">EWS を使用してバッチ処理でメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="070d5-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="070d5-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-145"></span></span>

<span data-ttu-id="070d5-146">バッチ処理でメール メッセージを送信するには、バッチ処理でのメール メッセージの作成に使用するコードと同じコードを使用します。ただし、**CreateItem** 操作の一部の属性値は変更します。</span><span class="sxs-lookup"><span data-stu-id="070d5-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation. So, to send email messages by using EWS, use the code you use to create email message in batches, and change the MessageDisposition value to “SendAndSaveCopy”, and change the DistinguishedFolderId to “sentitems”, as shown in the following code example.</span></span> <span data-ttu-id="070d5-147">そのため、EWS を使用してメール メッセージを送信するには、[バッチ処理でのメール メッセージの作成](#bk_createews)に使用するコードを使用して、次のコード例に示すように、**MessageDisposition** 値を "SendAndSaveCopy" に変更し、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) を "sentitems" に変更します。</span><span class="sxs-lookup"><span data-stu-id="070d5-147">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation. So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the MessageDisposition value to “SendAndSaveCopy”, and change the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to “sentitems”, as shown in the following code example.</span></span> 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="070d5-148">サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの新しいメッセージが正常に作成および送信されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="070d5-148">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span> 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="070d5-149">EWS マネージ API を使用してバッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="070d5-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="070d5-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-150"></span></span>

<span data-ttu-id="070d5-151">次の例に示されているように、EWS マネージ API [BindToItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメール メッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-151">You can get email messages in batches by using the EWS Managed API  UpdateItems http://msdn.microsoft.com/en-us/library/dd634705(v=exchg.80).aspx  method, as shown in the following example.</span></span> 
  
<span data-ttu-id="070d5-152">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="070d5-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<EmailMessage> BatchGetEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
    // Get the items from the server.
    // This method call results in a GetItem call to EWS.
    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
           
    // Instantiate a collection of EmailMessage objects to populate from the values that are returned by the Exchange server.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>();
    foreach (GetItemResponse getItemResponse in response)
    {
        try
        {
            Item item = getItemResponse.Item;
            EmailMessage message = (EmailMessage)item;
            messageItems.Add(message);
            // Print out confirmation and the last eight characters of the item ID.
            Console.WriteLine("Found item {0}.", message.Id.ToString().Substring(144));
        }
        catch (Exception ex)
        {
           Console.WriteLine("Exception while getting a message: {0}", ex.Message);
        }
    }
    // Check for success of the BindToItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages retrieved successfully.");
        Console.WriteLine("\r\n");
    }
        return messageItems;
}
```

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="070d5-153">EWS を使用してバッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="070d5-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="070d5-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-154"></span></span>

<span data-ttu-id="070d5-p108">次のコード例に示されている [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作とコードを使用して、バッチ処理でメール メッセージを取得できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを取得](#bk_getewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。 </span><span class="sxs-lookup"><span data-stu-id="070d5-p108">You can get email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example. This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span> 
  
<span data-ttu-id="070d5-157">**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="070d5-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="message:ToRecipients" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="m4NxAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB0" />
        <t:ItemId Id="m4NyAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB1" />
        <t:ItemId Id="m4NzAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB2" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="070d5-158">サーバーは **GetItem** 要求に [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの要求されたメッセージの[ファースト クラス プロパティ](email-properties-and-elements-in-ews-in-exchange.md)が含まれます。</span><span class="sxs-lookup"><span data-stu-id="070d5-158">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span> 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="070d5-159">EWS マネージ API を使用してバッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="070d5-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="070d5-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-160"></span></span>

<span data-ttu-id="070d5-161">次の例に示されているように、EWS マネージ API の [UpdateItems](http://msdn.microsoft.com/ja-JP/library/dd634705%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメール メッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-161">You can get email messages in batches by using the EWS Managed API [UpdateItemshttp://msdn.microsoft.com/en-us/library/dd634705(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="070d5-162">書き込み可能なメール メッセージ プロパティの一覧については、「[Exchange における EWS でのメールのプロパティと要素](email-properties-and-elements-in-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-162">For a list of writable email message properties, see Email properties and elements.</span></span>
  
<span data-ttu-id="070d5-163">下書きメッセージを更新してから送信する方法の詳細については、「[EWS マネージ API を使用してメール メッセージを送信する](#bk_sendewsma)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>
  
<span data-ttu-id="070d5-164">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="070d5-164">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<EmailMessage> BatchUpdateEmailItems(ExchangeService service, Collection<EmailMessage> messageItems)
{
    // Update the subject of each message locally.
    foreach (EmailMessage message in messageItems)
    {
        // Update the Subject of the email.
        message.Subject = "Updated subject at " + DateTime.Now;
        // Print out confirmation with the last eight characters of the item ID and the email subject.
        Console.WriteLine("Updated local email message {0} with the subject '{1}'.", message.Id.ToString().Substring(144), message.Subject);
    }
    // Send the item updates to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(messageItems, WellKnownFolderName.Drafts, ConflictResolutionMode.AutoResolve, MessageDisposition.SaveOnly, null);
    // Check for success of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages updated successfully.\r\n");
    }
    // If the method did not return success, print the result message for each email.
    else
    {
        Console.WriteLine("All emails were not successfully saved on the server.\r\n");
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            Console.WriteLine("Result for (message {0}): {1}", counter, resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            counter++;
        }
    }
    return messageItems;
}    
```

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="070d5-165">EWS を使用してバッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="070d5-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="070d5-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-166"></span></span>

<span data-ttu-id="070d5-p109">次のコード例に示されているように、EWS の [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して、バッチ処理でメール メッセージを更新できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを更新](#bk_updateewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="070d5-p109">You can update email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example. This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>
  
<span data-ttu-id="070d5-169">書き込み可能なメール メッセージ要素の一覧については、「[Exchange における EWS でのメールのプロパティと要素](email-properties-and-elements-in-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-169">For a list of writable email message elements, see Email properties and elements.</span></span>
  
<span data-ttu-id="070d5-170">下書きメッセージを更新してから送信する方法の詳細については、「[EWS を使用して下書きメール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly"
                  ConflictResolution="AutoResolve">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="m4OVAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCy" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OWAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCz" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OXAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKC0" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="070d5-p110">サーバーは、**UpdateItem** 要求に [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの更新がサーバーで正常に行われたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。競合は、[ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) 要素で報告されます。</span><span class="sxs-lookup"><span data-stu-id="070d5-p110">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server. Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="070d5-173">EWS マネージ API を使用してバッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="070d5-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="070d5-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-174"></span></span>

<span data-ttu-id="070d5-175">次の例に示されているように、EWS マネージ API の [DeleteItems](http://msdn.microsoft.com/ja-JP/library/dd635460%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-175">You can delete messages in batches by using the EWS Managed API [DeleteItemshttp://msdn.microsoft.com/en-us/library/dd635460(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="070d5-176">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="070d5-176">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void BatchDeleteEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of email message objects.
    // This method call results in an DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
    
    // Check for success of the DeleteItems method call.
    // DeleteItems returns success even if it does not find all the item IDs.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Email messages deleted successfully.\r\n");
    }
    // If the method did not return success, print a message.
    else
    {
        Console.WriteLine("Not all email messages deleted successfully.\r\n");
    }
}
```

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="070d5-177">EWS を使用してバッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="070d5-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="070d5-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-178"></span></span>

<span data-ttu-id="070d5-p111">次のコード例に示されているように、EWS の [DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用して、バッチ処理でメール メッセージを削除できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを削除](#bk_deleteewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="070d5-p111">You can delete email messages in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example. This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="SoftDelete"
                  AffectedTaskOccurrences="AllOccurrences">
      <m:ItemIds>
        <t:ItemId Id="m4OkAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDE" />
        <t:ItemId Id="m4OlAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDF" />
        <t:ItemId Id="m4OmAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDG" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="070d5-p112">サーバーは、**DeleteItem** 要求に [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) メッセージで応答します。このメッセージには、削除された各アイテムの **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。この操作によって、アイテム ID が見つからない場合でも成功が返される点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="070d5-p112">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed. Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="070d5-183">バッチ処理が正常に完了したことを確認する</span><span class="sxs-lookup"><span data-stu-id="070d5-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="070d5-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="070d5-184"></span></span>

<span data-ttu-id="070d5-p113">バッチ要求された 1 つ以上のメール メッセージを要求どおりに処理できないと、失敗したメール メッセージごとにエラーが返されます。バッチ処理のそれ以外のメールは予期したとおりに処理されます。対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更を行えなかったりすると、バッチ処理でエラーが生じます。このセクションの情報には、メール メッセージのバッチ処理で生じたエラーの詳細を取得する方法が示されています。</span><span class="sxs-lookup"><span data-stu-id="070d5-p113">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected. Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent. The information in this section shows how to get error details about failures in batch processing of email message.</span></span>
  
<span data-ttu-id="070d5-188">EWS マネージ API を使用してバッチ処理が成功したかどうかは、[ServiceResponseCollection](http://msdn.microsoft.com/ja-JP/library/dd633715%28v=exchg.80%29.aspx) の [OverallResult](http://msdn.microsoft.com/ja-JP/library/dd634515%28v=exchg.80%29.aspx) プロパティが [ServiceResult.Success](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx) と等しいかどうかを調べることで確認できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/ja-JP/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/ja-JP/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="070d5-189">等しい場合は、すべてのメールが正常に処理されています。</span><span class="sxs-lookup"><span data-stu-id="070d5-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="070d5-190">**OverallResult** が **ServiceResult.Success** と等しくない場合は、1 つ以上のメールが正常に処理されていません。</span><span class="sxs-lookup"><span data-stu-id="070d5-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="070d5-191">**ServiceResponseCollection** で返される各オブジェクトには、次のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="070d5-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="070d5-192">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="070d5-192">ErrorCode</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="070d5-193">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="070d5-193">ErrorDetails</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="070d5-194">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="070d5-194">ErrorMessage</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="070d5-195">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="070d5-195">ErrorProperties</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="070d5-196">Result</span><span class="sxs-lookup"><span data-stu-id="070d5-196">Result</span></span>](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="070d5-p115">これらのプロパティには、メール メッセージを要求どおりに処理できなかった原因についての情報が含まれます。この記事の例では、エラーが生じた各メッセージの **Result**、**ErrorCode**、**ErrorMessage** が出力されます。これらの結果を使用して問題を調査できます。</span><span class="sxs-lookup"><span data-stu-id="070d5-p115">These properties contain information about why the email messages could not be processed as requested. The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message. You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="070d5-p116">EWS でバッチ処理が成功したことを確認するには、各処理対象アイテムの [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) 属性を調べます。すべての応答メッセージの派生元となる基本タイプの **ResponseMessageType** の基本構造を次に示します。 </span><span class="sxs-lookup"><span data-stu-id="070d5-p116">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed. The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="070d5-p117">**ResponseClass** 属性は、メールが正常に処理された場合には **Success** に設定され、正常に処理されなかった場合には **Error** に設定されます。メール メッセージの場合には、バッチ処理中に **Warning** が示されることはありません。**ResponseClass** が **Success** の場合、それに続く [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素は必ず **NoError** に設定されます。**ResponseClass** が **Error** の場合、[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、**ResponseCode**、[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) の各要素の値を確認し、問題の原因を特定する必要があります。[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) は現在使用されていません。</span><span class="sxs-lookup"><span data-stu-id="070d5-p117">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully. For email messages, you will not encounter a **Warning** during batch processing. If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**. If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem. [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="070d5-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="070d5-207">See also</span></span>


- [<span data-ttu-id="070d5-208">Exchange のメールと EWS</span><span class="sxs-lookup"><span data-stu-id="070d5-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="070d5-209">Exchange で EWS を使用してメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="070d5-209">How to: Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="070d5-210">Exchange において EWS を使用してメール メッセージに応答する</span><span class="sxs-lookup"><span data-stu-id="070d5-210">How to: Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="070d5-211">Exchange において EWS を使用してメール メッセージを移動およびコピーする</span><span class="sxs-lookup"><span data-stu-id="070d5-211">How to: Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="070d5-212">EWS のバッチ要求の調整の影響</span><span class="sxs-lookup"><span data-stu-id="070d5-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

