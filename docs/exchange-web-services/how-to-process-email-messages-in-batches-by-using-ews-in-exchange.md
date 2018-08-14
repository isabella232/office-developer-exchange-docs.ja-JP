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
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Exchange で EWS を使用してバッチ処理でメール メッセージを処理する

Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで複数のメール メッセージの作成、取得、更新、削除をバッチ処理する方法について説明します。
  
EWS マネージ API または EWS を使用すると、メール メッセージのバッチ操作を行い、クライアントが Exchange サーバーを呼び出す回数を減らせます。 EWS マネージ API を使用してメール メッセージの作成、取得、更新、削除、送信のバッチ操作を行う場合、[ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。1 つのメール メッセージを対象とする場合には [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクト メソッドを使用します。 EWS を使用する場合は、同じ操作を使用して 1 つのメール メッセージの処理とバッチ処理のどちらも行えます。 
  
**表 1. メール メッセージをバッチ処理するための EWS マネージ API メソッドと EWS 操作**

|**目的**|**使用する EWS マネージ API メソッド**|**使用する EWS 操作**|
|:-----|:-----|:-----|
|バッチ処理でメール メッセージを作成する  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|バッチ処理でメール メッセージを取得する  <br/> |[ExchangeService.BindToItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|バッチ処理でメール メッセージを更新する  <br/> |[ExchangeService.UpdateItems](http://msdn.microsoft.com/ja-JP/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|バッチ処理でメール メッセージを削除する  <br/> |[ExchangeService.DeleteItems](http://msdn.microsoft.com/ja-JP/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
この記事では、EWS マネージ API または EWS を使用してメール メッセージのバッチ処理を行うための基本的なタスクの実行方法について説明します。
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理でメール メッセージを作成する
<a name="bk_createewsma"> </a>

次の例に示されているように、EWS マネージ API **CreateItems** メソッドを使用すると、バッチ処理でメッセージを作成できます。 この例では、3 つの [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトをローカルに作成し、それぞれのメッセージをコレクションに追加してから、メッセージのコレクションをパラメーターにして **CreateItems** メソッドを呼び出します。 
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
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

この例では、下書きフォルダーにメッセージを保存しますが、メッセージは送信しません。 メッセージを送信する方法の詳細については、「[EWS マネージ API を使用してバッチ処理でメール メッセージを送信する](#bk_sendewsma)」を参照してください。
  
## <a name="create-email-messages-in-batches-by-using-ews"></a>EWS を使用してバッチ処理でメール メッセージを作成する
<a name="bk_createews"> </a>

次のコード例に示されているように、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS 操作を使用して、バッチ処理でメール メッセージを作成できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを作成](#bk_createewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。  
  
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

サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの新しいメッセージが正常に作成および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。 
  
この例では、下書きフォルダーにメッセージを保存しますが、メッセージは送信しません。 メッセージを送信する方法の詳細については、「[EWS を使用してバッチ処理でメール メッセージを送信する](#bk_sendews)」を参照してください。
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理でメール メッセージを送信する
<a name="bk_sendewsma"> </a>

バッチ処理でメール メッセージを送信するには、バッチ処理でのメール メッセージの作成に使用するコードと同じコードを使用します。ただし、一部の [CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) メソッドのパラメーターは変更します。 そのため、EWS マネージ API を使用してメール メッセージを送信するには、[バッチ処理でのメール メッセージの作成](#bk_createewsma)に使用するコードを使用して、**CreateItems** メソッドへの呼び出しを次の例の呼び出しに置き換えます。 この例では、メッセージは送信済みアイテム フォルダーに作成されます。またメッセージがローカルに保存されるだけでなく送信されるように、メッセージの処理方法を [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx) に変更しています。
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>EWS を使用してバッチ処理でメール メッセージを送信する
<a name="bk_sendews"> </a>

バッチ処理でメール メッセージを送信するには、バッチ処理でのメール メッセージの作成に使用するコードと同じコードを使用します。ただし、**CreateItem** 操作の一部の属性値は変更します。 そのため、EWS を使用してメール メッセージを送信するには、[バッチ処理でのメール メッセージの作成](#bk_createews)に使用するコードを使用して、次のコード例に示すように、**MessageDisposition** 値を "SendAndSaveCopy" に変更し、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) を "sentitems" に変更します。 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの新しいメッセージが正常に作成および送信されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理でメール メッセージを取得する
<a name="bk_getewsma"> </a>

次の例に示されているように、EWS マネージ API [BindToItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメール メッセージを取得できます。 
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
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

## <a name="get-email-messages-in-batches-by-using-ews"></a>EWS を使用してバッチ処理でメール メッセージを取得する
<a name="bk_getews"> </a>

次のコード例に示されている [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作とコードを使用して、バッチ処理でメール メッセージを取得できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを取得](#bk_getewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。  
  
**ItemId** 属性と **ChangeKey** 属性は読みやすいように短縮されています。 
  
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

サーバーは **GetItem** 要求に [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの要求されたメッセージの[ファースト クラス プロパティ](email-properties-and-elements-in-ews-in-exchange.md)が含まれます。 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理でメール メッセージを更新する
<a name="bk_updateewsma"> </a>

次の例に示されているように、EWS マネージ API の [UpdateItems](http://msdn.microsoft.com/ja-JP/library/dd634705%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメール メッセージを取得できます。 
  
書き込み可能なメール メッセージ プロパティの一覧については、「[Exchange における EWS でのメールのプロパティと要素](email-properties-and-elements-in-ews-in-exchange.md)」を参照してください。
  
下書きメッセージを更新してから送信する方法の詳細については、「[EWS マネージ API を使用してメール メッセージを送信する](#bk_sendewsma)」を参照してください。
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
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

## <a name="update-email-messages-in-batches-by-using-ews"></a>EWS を使用してバッチ処理でメール メッセージを更新する
<a name="bk_updateews"> </a>

次のコード例に示されているように、EWS の [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して、バッチ処理でメール メッセージを更新できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを更新](#bk_updateewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。
  
書き込み可能なメール メッセージ要素の一覧については、「[Exchange における EWS でのメールのプロパティと要素](email-properties-and-elements-in-ews-in-exchange.md)」を参照してください。
  
下書きメッセージを更新してから送信する方法の詳細については、「[EWS を使用して下書きメール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)」を参照してください。
  
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

サーバーは、**UpdateItem** 要求に [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの更新がサーバーで正常に行われたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。競合は、[ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) 要素で報告されます。 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理でメール メッセージを削除する
<a name="bk_deleteewsma"> </a>

次の例に示されているように、EWS マネージ API の [DeleteItems](http://msdn.microsoft.com/ja-JP/library/dd635460%28v=exchg.80%29.aspx) メソッドを使用すると、バッチ処理でメッセージを削除できます。 
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
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

## <a name="delete-email-messages-in-batches-by-using-ews"></a>EWS を使用してバッチ処理でメール メッセージを削除する
<a name="bk_deleteews"> </a>

次のコード例に示されているように、EWS の [DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用して、バッチ処理でメール メッセージを削除できます。これは、EWS マネージ API を使用して[バッチ処理でメール メッセージを削除](#bk_deleteewsma)する際に、EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、**DeleteItem** 要求に [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) メッセージで応答します。このメッセージには、削除された各アイテムの **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。この操作によって、アイテム ID が見つからない場合でも成功が返される点に注意してください。 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a>バッチ処理が正常に完了したことを確認する
<a name="bk_successful"> </a>

バッチ要求された 1 つ以上のメール メッセージを要求どおりに処理できないと、失敗したメール メッセージごとにエラーが返されます。バッチ処理のそれ以外のメールは予期したとおりに処理されます。対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更を行えなかったりすると、バッチ処理でエラーが生じます。このセクションの情報には、メール メッセージのバッチ処理で生じたエラーの詳細を取得する方法が示されています。
  
EWS マネージ API を使用してバッチ処理が成功したかどうかは、[ServiceResponseCollection](http://msdn.microsoft.com/ja-JP/library/dd633715%28v=exchg.80%29.aspx) の [OverallResult](http://msdn.microsoft.com/ja-JP/library/dd634515%28v=exchg.80%29.aspx) プロパティが [ServiceResult.Success](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx) と等しいかどうかを調べることで確認できます。 等しい場合は、すべてのメールが正常に処理されています。 **OverallResult** が **ServiceResult.Success** と等しくない場合は、1 つ以上のメールが正常に処理されていません。 **ServiceResponseCollection** で返される各オブジェクトには、次のプロパティが含まれます。 
  
- [ErrorCode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [ErrorDetails](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [ErrorMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [ErrorProperties](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [Result](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
これらのプロパティには、メール メッセージを要求どおりに処理できなかった原因についての情報が含まれます。この記事の例では、エラーが生じた各メッセージの **Result**、**ErrorCode**、**ErrorMessage** が出力されます。これらの結果を使用して問題を調査できます。 
  
EWS でバッチ処理が成功したことを確認するには、各処理対象アイテムの [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) 属性を調べます。すべての応答メッセージの派生元となる基本タイプの **ResponseMessageType** の基本構造を次に示します。  
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

**ResponseClass** 属性は、メールが正常に処理された場合には **Success** に設定され、正常に処理されなかった場合には **Error** に設定されます。メール メッセージの場合には、バッチ処理中に **Warning** が示されることはありません。**ResponseClass** が **Success** の場合、それに続く [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素は必ず **NoError** に設定されます。**ResponseClass** が **Error** の場合、[MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、**ResponseCode**、[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) の各要素の値を確認し、問題の原因を特定する必要があります。[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) は現在使用されていません。 
  
## <a name="see-also"></a>関連項目


- [Exchange のメールと EWS](email-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用してメール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用してメール メッセージに応答する](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用してメール メッセージを移動およびコピーする](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [EWS のバッチ要求の調整の影響](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

