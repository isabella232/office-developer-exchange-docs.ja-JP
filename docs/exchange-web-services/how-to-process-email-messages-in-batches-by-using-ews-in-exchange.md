---
title: 電子メール メッセージを Exchange で EWS を使用してバッチ プロセス
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで複数のメール メッセージの作成、取得、更新、削除をバッチ処理する方法について説明します。
ms.openlocfilehash: 30ebbdf4c92111df629c7662987e301d167336e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759063"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="26f69-103">電子メール メッセージを Exchange で EWS を使用してバッチ プロセス</span><span class="sxs-lookup"><span data-stu-id="26f69-103">Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="26f69-104">Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで複数のメール メッセージの作成、取得、更新、削除をバッチ処理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="26f69-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="26f69-105">EWS のマネージ API を使用することができます。 または EWS 呼び出しの数を減らすために電子メール メッセージのバッチがクライアントを使用すると、Exchange サーバーにします。</span><span class="sxs-lookup"><span data-stu-id="26f69-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="26f69-106">EWS のマネージ API を使用してを作成、取得、更新、削除、およびバッチ処理でメッセージを送信すると、 [email メッセージ](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用する 1 つの電子メール メッセージを使用するときに、 [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="26f69-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="26f69-107">EWS を使用する場合は、単一および電子メール メッセージのバッチの両方を使用する同じ操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="26f69-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span> 
  
<span data-ttu-id="26f69-108">**表 1 です。EWS のマネージ API のメソッドおよび電子メール メッセージのバッチを処理するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="26f69-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="26f69-109">**目的…**</span><span class="sxs-lookup"><span data-stu-id="26f69-109">**In order to…**</span></span>|<span data-ttu-id="26f69-110">**この EWS 管理 API メソッドを使用します。**</span><span class="sxs-lookup"><span data-stu-id="26f69-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="26f69-111">**EWS 操作を使用します。**</span><span class="sxs-lookup"><span data-stu-id="26f69-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="26f69-112">バッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="26f69-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="26f69-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="26f69-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="26f69-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="26f69-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="26f69-115">バッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="26f69-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="26f69-116">ExchangeService.BindToItems</span><span class="sxs-lookup"><span data-stu-id="26f69-116">ExchangeService.BindToItems</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="26f69-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="26f69-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="26f69-118">バッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="26f69-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="26f69-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="26f69-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/ja-jp/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="26f69-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="26f69-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="26f69-121">バッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="26f69-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="26f69-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="26f69-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/ja-jp/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="26f69-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="26f69-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="26f69-124">この記事では、EWS のマネージ API または EWS を使用して電子メール メッセージのバッチのための基本的なタスクを完了する方法について学習します。</span><span class="sxs-lookup"><span data-stu-id="26f69-124">In this article, you'll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="26f69-125">EWS マネージ API を使用してバッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="26f69-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="26f69-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-126"></span></span>

<span data-ttu-id="26f69-127">例を次に示すように、マネージ API の EWS **CreateItems**メソッドを使用してバッチ処理でメッセージを作成できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-127">You can create messages in batches by using the EWS Managed API **CreateItems** method, as shown in the following example.</span></span> <span data-ttu-id="26f69-128">次の使用例 3 つの[なか](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトをローカルに作成するには、各メッセージは、コレクションに追加し、メッセージのコレクションで**CreateItems**メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="26f69-128">This example creates three [EmailMessage](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span> 
  
<span data-ttu-id="26f69-129">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="26f69-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="26f69-130">例は、[下書き] フォルダー内のメッセージをのみ保存に注意してください。メッセージは送信されません。</span><span class="sxs-lookup"><span data-stu-id="26f69-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="26f69-131">メッセージを送信する方法の詳細については、 [EWS のマネージ API を使用してバッチ処理での電子メール メッセージの送信](#bk_sendewsma)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>
  
## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="26f69-132">EWS を使用して、バッチ処理でメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="26f69-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="26f69-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-133"></span></span>

<span data-ttu-id="26f69-134">コード例を次に示すように、 [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS 操作を使用してバッチ処理で電子メール メッセージを作成できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-134">You can create email messages in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="26f69-135">EWS のマネージ API が[バッチ内の電子メール メッセージを作成](#bk_createewsma)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="26f69-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span> 
  
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

<span data-ttu-id="26f69-136">サーバー要求に応答し、 **CreateItem** **NoError**の[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値は、それぞれの新しいメッセージ、各電子メールが作成され、正常に保存されたことを示す[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージ.</span><span class="sxs-lookup"><span data-stu-id="26f69-136">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span> 
  
<span data-ttu-id="26f69-137">例は、[下書き] フォルダー内のメッセージをのみ保存に注意してください。メッセージは送信されません。</span><span class="sxs-lookup"><span data-stu-id="26f69-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="26f69-138">メッセージを送信する方法の詳細については、 [EWS を使用してバッチ内の電子メール メッセージの送信](#bk_sendews)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="26f69-139">EWS マネージ API を使用してバッチ処理でメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="26f69-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="26f69-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-140"></span></span>

<span data-ttu-id="26f69-141">[CreateItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx)メソッドのパラメーターのいくつかを変更することを除いて、バッチ、電子メール メッセージを作成するのに使用するバッチ内の電子メール メッセージを送信するのにには、同じコードを使用します。</span><span class="sxs-lookup"><span data-stu-id="26f69-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="26f69-142">EWS のマネージ API を使用して電子メール メッセージを送信する[バッチ内の電子メール メッセージを作成](#bk_createewsma)するに使用するコードを使用し、 **CreateItems**メソッドの呼び出しを次の例では、呼び出しに置き換えます。</span><span class="sxs-lookup"><span data-stu-id="26f69-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="26f69-143">この例では、メッセージが送信済みアイテム フォルダーに作成され、するため、メッセージが送信され、ローカルに保存だけでなく、 [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx)にメッセージの処理方法が変更されます。</span><span class="sxs-lookup"><span data-stu-id="26f69-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="26f69-144">EWS を使用してバッチ処理でメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="26f69-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="26f69-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-145"></span></span>

<span data-ttu-id="26f69-146">**CreateItem**操作のいくつかの属性の値を変更する点を除いては、バッチ、電子メール メッセージを作成するのに使用することに、バッチで電子メール メッセージを送信するのにには、同じコードを使用します。</span><span class="sxs-lookup"><span data-stu-id="26f69-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation.</span></span> <span data-ttu-id="26f69-147">EWS を使用して電子メール メッセージを送信するを使用して[バッチ内の電子メール メッセージを作成](#bk_createews)、および"SendAndSaveCopy"、 **MessageDisposition**の値に変更するコードを使用しに示すように、 [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)を"送信済みアイテム] に変更します次のコード例です。</span><span class="sxs-lookup"><span data-stu-id="26f69-147">So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the **MessageDisposition** value to "SendAndSaveCopy", and change the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to "sentitems", as shown in the following code example.</span></span> 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="26f69-148">サーバーは、 **CreateItem**要求**NoError**の[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値は、それぞれの新しいメッセージ、各電子メールが作成され、正常に送信されたことを示す[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="26f69-148">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span> 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="26f69-149">EWS マネージ API を使用してバッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="26f69-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="26f69-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-150"></span></span>

<span data-ttu-id="26f69-151">次の例のように、EWS のマネージ API の[BindToItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で電子メール メッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-151">You can get email messages in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="26f69-152">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="26f69-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="26f69-153">EWS を使用してバッチ処理でメール メッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="26f69-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="26f69-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-154"></span></span>

<span data-ttu-id="26f69-155">次の例では、 [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作とコードを使用してバッチ処理で電子メール メッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-155">You can get email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="26f69-156">EWS のマネージ API が[バッチ内の電子メール メッセージを取得](#bk_getewsma)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="26f69-156">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span> 
  
<span data-ttu-id="26f69-157">**アイテム Id**と**変更キー**の属性は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="26f69-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="26f69-158">サーバーは、要求されたメッセージの[最初のクラスのプロパティ](email-properties-and-elements-in-ews-in-exchange.md)が含まれています[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx)メッセージの**GetItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="26f69-158">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span> 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="26f69-159">EWS マネージ API を使用してバッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="26f69-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="26f69-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-160"></span></span>

<span data-ttu-id="26f69-161">次の例のように、EWS のマネージ API の[UpdateItems](http://msdn.microsoft.com/ja-jp/library/dd634705%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で電子メール メッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-161">You can get email messages in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/ja-jp/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="26f69-162">書き込み可能な電子メール メッセージのプロパティのリストは、 [Exchange プロパティおよび EWS での要素を電子メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-162">For a list of writable email message properties, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="26f69-163">更新された後、下書きメッセージを送信する方法の詳細については、 [EWS のマネージ API を使用して電子メール メッセージを送信する](#bk_sendewsma)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>
  
<span data-ttu-id="26f69-164">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="26f69-164">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="26f69-165">EWS を使用してバッチ処理でメール メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="26f69-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="26f69-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-166"></span></span>

<span data-ttu-id="26f69-167">[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作を使用してバッチ内の電子メール メッセージを更新するには、次のコード例に示すように。</span><span class="sxs-lookup"><span data-stu-id="26f69-167">You can update email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="26f69-168">EWS のマネージ API が[バッチ内の電子メール メッセージを更新](#bk_updateewsma)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="26f69-168">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>
  
<span data-ttu-id="26f69-169">書き込み可能な電子メール メッセージの要素のリストは、[プロパティおよび EWS での要素を Exchange 電子メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-169">For a list of writable email message elements, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="26f69-170">更新された後、下書きメッセージを送信する方法の詳細については、 [EWS を使用して、下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
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

<span data-ttu-id="26f69-171">サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、更新プログラムのそれぞれのサーバー上でが正常に保存されたことを示す値を含む、 [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx)メッセージの**UpdateItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="26f69-171">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="26f69-172">[ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx)要素内での競合が報告されます。</span><span class="sxs-lookup"><span data-stu-id="26f69-172">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="26f69-173">EWS マネージ API を使用してバッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="26f69-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="26f69-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-174"></span></span>

<span data-ttu-id="26f69-175">、EWS のマネージ API の[DeleteItems](http://msdn.microsoft.com/ja-jp/library/dd635460%28v=exchg.80%29.aspx)メソッドを使用してバッチ内のメッセージを削除するには、次の例のようにします。</span><span class="sxs-lookup"><span data-stu-id="26f69-175">You can delete messages in batches by using the EWS Managed API [DeleteItems](http://msdn.microsoft.com/ja-jp/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="26f69-176">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="26f69-176">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="26f69-177">EWS を使用してバッチ処理でメール メッセージを削除する</span><span class="sxs-lookup"><span data-stu-id="26f69-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="26f69-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-178"></span></span>

<span data-ttu-id="26f69-179">[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS 操作を使用してバッチ内の電子メール メッセージを削除するには、次のコード例に示すように。</span><span class="sxs-lookup"><span data-stu-id="26f69-179">You can delete email messages in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="26f69-180">EWS のマネージ API が[バッチ内の電子メール メッセージを削除](#bk_deleteewsma)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="26f69-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>
  
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

<span data-ttu-id="26f69-181">サーバー要求に応答、 **DeleteItem** **NoError**の削除された項目ごとに[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値を含む[DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx)のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="26f69-181">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="26f69-182">返す成功アイテム ID が見つかりませんだった場合に注意してください。</span><span class="sxs-lookup"><span data-stu-id="26f69-182">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="26f69-183">バッチ処理が正常に完了したことを確認する</span><span class="sxs-lookup"><span data-stu-id="26f69-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="26f69-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="26f69-184"></span></span>

<span data-ttu-id="26f69-p113">バッチ要求された 1 つ以上のメール メッセージを要求どおりに処理できないと、失敗したメール メッセージごとにエラーが返されます。バッチ処理のそれ以外のメールは予期したとおりに処理されます。対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更を行えなかったりすると、バッチ処理でエラーが生じます。このセクションの情報には、メール メッセージのバッチ処理で生じたエラーの詳細を取得する方法が示されています。</span><span class="sxs-lookup"><span data-stu-id="26f69-p113">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected. Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent. The information in this section shows how to get error details about failures in batch processing of email message.</span></span>
  
<span data-ttu-id="26f69-188">EWS のマネージ API を使用して、バッチ処理の成功を確認するには、 [ServiceResponseCollection](http://msdn.microsoft.com/ja-jp/library/dd633715%28v=exchg.80%29.aspx)の[OverallResult](http://msdn.microsoft.com/ja-jp/library/dd634515%28v=exchg.80%29.aspx)プロパティが[ServiceResult.Success](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx)に等しいかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="26f69-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/ja-jp/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/ja-jp/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="26f69-189">その場合は、すべての電子メールが正常に処理されました。</span><span class="sxs-lookup"><span data-stu-id="26f69-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="26f69-190">**OverallResult**が**ServiceResult.Success**、1 つまたは複数の電子メールの場合は、正常に処理されませんでした。</span><span class="sxs-lookup"><span data-stu-id="26f69-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="26f69-191">**ServiceResponseCollection**で返されるオブジェクトの各には、次のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="26f69-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="26f69-192">エラー コード</span><span class="sxs-lookup"><span data-stu-id="26f69-192">ErrorCode</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="26f69-193">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="26f69-193">ErrorDetails</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="26f69-194">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="26f69-194">ErrorMessage</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="26f69-195">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="26f69-195">ErrorProperties</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="26f69-196">結果</span><span class="sxs-lookup"><span data-stu-id="26f69-196">Result</span></span>](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="26f69-197">これらのプロパティには、なぜ電子メール メッセージを処理できませんでした要求に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="26f69-197">These properties contain information about why the email messages could not be processed as requested.</span></span> <span data-ttu-id="26f69-198">この資料の例は、障害が発生したメッセージごとに、**結果**、**エラー コード**、および**エラー メッセージ**を出力します。</span><span class="sxs-lookup"><span data-stu-id="26f69-198">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message.</span></span> <span data-ttu-id="26f69-199">これらの結果を使用すると、問題を調査します。</span><span class="sxs-lookup"><span data-stu-id="26f69-199">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="26f69-200">EWS では、バッチ処理の成功を確認するには、処理中の各項目の[ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx)属性を確認します。</span><span class="sxs-lookup"><span data-stu-id="26f69-200">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="26f69-201">**ResponseMessageType**、するすべての応答メッセージの派生元の基本型の基本構造を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26f69-201">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="26f69-202">**ResponseClass**属性は、電子メールが正常に処理されなかった場合に、電子メールが正常に処理された場合の**成功**または**エラー**に設定されます。</span><span class="sxs-lookup"><span data-stu-id="26f69-202">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully.</span></span> <span data-ttu-id="26f69-203">、電子メール メッセージのバッチ処理中に**警告**は発生しません。</span><span class="sxs-lookup"><span data-stu-id="26f69-203">For email messages, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="26f69-204">**ResponseClass**が**成功**の場合は、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の後も常に**NoError**に設定されています。</span><span class="sxs-lookup"><span data-stu-id="26f69-204">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="26f69-205">**ResponseClass**が**エラー**の場合は、問題の原因を特定するのには、[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、 **ResponseCode**、および[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx)の要素の値を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="26f69-205">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="26f69-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx)は、現在使用されていません。</span><span class="sxs-lookup"><span data-stu-id="26f69-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="26f69-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="26f69-207">See also</span></span>


- [<span data-ttu-id="26f69-208">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="26f69-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="26f69-209">EWS を使用して Exchange が電子メール メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="26f69-209">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="26f69-210">EWS を使用して Exchange が電子メール メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="26f69-210">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="26f69-211">移動し、EWS を使用して Exchange が電子メール メッセージをコピー</span><span class="sxs-lookup"><span data-stu-id="26f69-211">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="26f69-212">EWS のバッチ要求の影響を調整</span><span class="sxs-lookup"><span data-stu-id="26f69-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

