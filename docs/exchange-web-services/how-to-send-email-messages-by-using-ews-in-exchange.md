---
title: EWS を使用して Exchange が電子メール メッセージを送信します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 5290fafe-8b51-4275-a27e-baf497fc969c
description: Exchange で EWS マネージ API または EWS を使用して、新規または下書きのメール メッセージを送信する方法、または遅延していたメール メッセージを送信する方法を説明します。
ms.openlocfilehash: f09babfcc420d4cbc563ed6605ba555fd9f8c7e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759050"
---
# <a name="send-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="7a311-103">EWS を使用して Exchange が電子メール メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="7a311-103">Send email messages by using EWS in Exchange</span></span>

<span data-ttu-id="7a311-104">Exchange で EWS マネージ API または EWS を使用して、新規または下書きのメール メッセージを送信する方法、または遅延していたメール メッセージを送信する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="7a311-104">Learn how to send new or draft email messages, or to send a delayed email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7a311-p101">EWS マネージ API と EWS のどちらを使用していても、メール メッセージは 2 つの方法で送信することができます。[下書き] フォルダーに保存されているメッセージなどの既存のメッセージを送信するか、または 1 つの手順でメールを作成して送信するかのいずれかが行えます。メッセージの送信に使用するメソッドと操作は、すぐにメッセージを送信する場合でも、遅延していたメッセージを送信する場合でも同じです。</span><span class="sxs-lookup"><span data-stu-id="7a311-p101">Whether you are using the EWS Managed API or EWS, you can send email messages in two ways. You can either send an existing message, such as a message stored in your Drafts folder, or you can create and send an email in one step. The methods and operations that you use to send the message are the same whether you're sending a message immediately, or sending a delayed message.</span></span>
  
<span data-ttu-id="7a311-108">**表 1 です。EWS のマネージ API のメソッドおよび電子メール メッセージを送信するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="7a311-108">**Table 1. EWS Managed API methods and EWS operations for sending email messages**</span></span>

|<span data-ttu-id="7a311-109">**タスク**</span><span class="sxs-lookup"><span data-stu-id="7a311-109">**Task**</span></span>|<span data-ttu-id="7a311-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="7a311-110">**EWS Managed API method**</span></span>|<span data-ttu-id="7a311-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="7a311-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7a311-112">新しいメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-112">Send a new email message</span></span>  <br/> |[<span data-ttu-id="7a311-113">EmailMessage.SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="7a311-113">EmailMessage.SendAndSaveCopy</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a311-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="7a311-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7a311-115">既存のメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-115">Send an existing email message</span></span>  <br/> |[<span data-ttu-id="7a311-116">EmailMessage.Send</span><span class="sxs-lookup"><span data-stu-id="7a311-116">EmailMessage.Send</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7a311-117">SendItem</span><span class="sxs-lookup"><span data-stu-id="7a311-117">SendItem</span></span>](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> |
   
## <a name="send-a-new-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="7a311-118">EWS マネージ API を使用して新しいメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-118">Send a new email message by using the EWS Managed API</span></span>
<span data-ttu-id="7a311-119"><a name="bk_sendnewewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-119"></span></span>

<span data-ttu-id="7a311-120">[なか](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトを使用して電子メール メッセージの受信者にメッセージを送信し、メッセージを送信済みアイテム フォルダーに保存するには、 [SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)メソッドを作成する方法を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="7a311-120">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message and the [SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="7a311-121">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="7a311-121">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "' and saved in the SendItems folder.");
```

## <a name="send-a-new-email-message-by-using-ews"></a><span data-ttu-id="7a311-122">EWS を使用して新しいメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-122">Send a new email message by using EWS</span></span>
<span data-ttu-id="7a311-123"><a name="bk_sendnewews"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-123"></span></span>

<span data-ttu-id="7a311-124">次のコード例では、 **SendAndSaveCopy**の**MessageDisposition**値を持つ[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用して、電子メール メッセージを作成する、受信者にメッセージを送信し、メッセージを送信済みアイテム フォルダーに保存する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="7a311-124">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, send the message to the recipient, and save the message in the Sent Items folder.</span></span> <span data-ttu-id="7a311-125">EWS のマネージ API を送信する場合、XML の要求はまた[、新しい電子メール メッセージを送信](#bk_sendnewewsma)します。</span><span class="sxs-lookup"><span data-stu-id="7a311-125">This is also the XML request that the EWS Managed API sends when you [send a new email message](#bk_sendnewewsma).</span></span>
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7a311-126">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/ja-jp/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7a311-126">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-jp/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="send-a-draft-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="7a311-127">EWS マネージ API を使用して下書きのメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-127">Send a draft email message by using the EWS Managed API</span></span>
<span data-ttu-id="7a311-128"><a name="bk_senddraftewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-128"></span></span>

<span data-ttu-id="7a311-129">次のコード例では、 [EWS のマネージ API を使用して電子メール メッセージを作成](email-and-ews-in-exchange.md#bk_createewsma)する」で示すように、[下書き] フォルダーに格納されているメッセージを送信する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="7a311-129">The following code example shows how to send a message that was stored in the Drafts folder, as shown in [Create an email message by using the EWS Managed API](email-and-ews-in-exchange.md#bk_createewsma).</span></span> <span data-ttu-id="7a311-130">最初に、メッセージを取得するために、 [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを使用し、メソッドを使用して[送信](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx)電子メール メッセージを送信するコード例を次に示すようにします。</span><span class="sxs-lookup"><span data-stu-id="7a311-130">First, use the [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to retrieve the message, and then use the [Send](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to send the email message, as shown in the following code example.</span></span> <span data-ttu-id="7a311-131">送信済みアイテム フォルダーに送信されるメッセージはこのメソッドによって保存されないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="7a311-131">Note that this method does not save the sent message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="7a311-132">この例では、 [EmailMessageSchema.Subject](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx)および[EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx)プロパティは、コンソール出力の値を含めることができるように、[プロパティ設定](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx)に追加されます。</span><span class="sxs-lookup"><span data-stu-id="7a311-132">In this case, the [EmailMessageSchema.Subject](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) and [EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) properties are added to the [PropertySet](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) so that the values can be included in the console output.</span></span> 
  
<span data-ttu-id="7a311-133">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="7a311-133">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
// Send the email message.
// This method call results in a SendItem call to EWS.
message.Send();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "'.");
```

## <a name="send-a-draft-email-message-by-using-ews"></a><span data-ttu-id="7a311-134">EWS を使用して下書きのメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-134">Send a draft email message by using EWS</span></span>
<span data-ttu-id="7a311-135"><a name="bk_senddraftews"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-135"></span></span>

<span data-ttu-id="7a311-136">次のコード例では、 [EWS を使用して電子メール メッセージを作成](email-and-ews-in-exchange.md#bk_createews)する」で示すように、[下書き] フォルダーに保存されていたメッセージを送信する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="7a311-136">The following code examples show how to send a message that was previously stored in the Drafts folder, as shown in [Create an email message by using EWS](email-and-ews-in-exchange.md#bk_createews).</span></span> <span data-ttu-id="7a311-137">最初に送信するのに電子メール メッセージを取得するために[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx)操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a311-137">First use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to retrieve the email message to send.</span></span> <span data-ttu-id="7a311-138">[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx)操作を使用して、受信者に電子メール メッセージを送信し、送信済みアイテム フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="7a311-138">Then use the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the email message to recipients and save it in the Sent Items folder.</span></span> 
  
<span data-ttu-id="7a311-139">**GetItem**要求メッセージでは、最初のメッセージが、バインドする下書き電子メール メッセージの[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を指定し、 [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx)要素内の要素は、 **GetItem**応答に含める結果を制限します。</span><span class="sxs-lookup"><span data-stu-id="7a311-139">The first message, the **GetItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the draft email message to bind to, and elements in the [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) element limit the results to include in the **GetItem** response.</span></span> <span data-ttu-id="7a311-140">**ItemShape**要素には、 [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の**IdOnly**、および[AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx)要素には、**件名**のプロパティ項目のスキーマと**ToRecipients**から[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx)値が含まれます。**アイテム Id**、[件名](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)、および[ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx)要素だけであるは、メッセージ スキーマのプロパティは、応答でクライアントに返されます。</span><span class="sxs-lookup"><span data-stu-id="7a311-140">The **ItemShape** element has a [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) of **IdOnly**, and the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element includes the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) values for the **Subject** property from the Item schema and the **ToRecipients** property from the Message schema, which means that only the **ItemId**, [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx), and [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) elements will be returned to the client in the response.</span></span> <span data-ttu-id="7a311-141">呼び出しと**BaseShape**の要素の意味で返される値を制限することに関する詳細については、[プロパティ セットと応答内の図形 EWS Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a311-141">For more information about limiting the values returned in calls and the meaning of the **BaseShape** element, see [Property sets and response shapes in EWS in Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="7a311-142">[Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを呼び出すときに、EWS のマネージ API によって送信される XML の要求にもです。</span><span class="sxs-lookup"><span data-stu-id="7a311-142">This is also the XML request that is sent by the EWS Managed API when calling the [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="7a311-143">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="7a311-143">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
        <t:ItemId Id="AAMkADE4=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

次の例は、 **GetItem** 操作の処理後にサーバーから返される XML 応答を示しています。 応答は、電子メール メッセージが正常に取得された要求された**件名**と**ToRecipient**の要素が含まれて ことを示します。 <span data-ttu-id="7a311-146">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="7a311-146">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="842"
                         MinorBuildNumber="10"
                         Version="V2_8"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAMkADE4="
                        ChangeKey="CQAAABYA" />
              <t:Subject>Project priorities</t:Subject>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>sadie@contoso.com</t:Name>
                  <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                  <t:MailboxType>OneOff</t:MailboxType>
                </t:Mailbox>
              </t:ToRecipients>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="7a311-147">**SendItem**要求メッセージを 2 番目のメッセージは、 [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx)、送信済みアイテムを保存するフォルダーを指定するだけでなく、送信する電子メール メッセージの[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a311-147">The second message, the **SendItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to send, as well as the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), which specifies the folder in which to save the sent item.</span></span>
  
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
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADE4="
                  ChangeKey="CQAAABYA" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7a311-148">サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**メールが正常に送信されたことを示す値を含む[SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx)メッセージが**SendItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="7a311-148">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="send-a-delayed-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="7a311-149">EWS マネージ API を使用して遅延していたメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-149">Send a delayed email message by using the EWS Managed API</span></span>
<span data-ttu-id="7a311-150"><a name="bk_senddelayedewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-150"></span></span>

<span data-ttu-id="7a311-151">コード例を次に示します[なか](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトを使用して電子メール メッセージ、 [PidTagDeferredSendTime](http://msdn.microsoft.com/ja-jp/library/cc840017.aspx) (0x3FEF0040) プロパティでは、プロパティ定義を作成する[ExtendedPropertyDefinition](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx)クラスを作成する方法と、遅延メッセージを送信し、メッセージを送信済みアイテム フォルダーに保存する方法を[SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) 。</span><span class="sxs-lookup"><span data-stu-id="7a311-151">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message, the [ExtendedPropertyDefinition](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) class to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/ja-jp/library/cc840017.aspx) (0x3FEF0040) property, and the [SendAndSaveCopy](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send a delayed message and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="7a311-152">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="7a311-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a new email message. 
EmailMessage message = new EmailMessage(service);
// Specify the email recipient and subject. 
message.ToRecipients.Add("sadie@contoso.com");
message.Subject = "Delayed email";
// Identify the extended property that can be used to specify when to send the email. 
ExtendedPropertyDefinition PidTagDeferredSendTime = new ExtendedPropertyDefinition(16367, MapiPropertyType.SystemTime);
// Set the time that will be used to specify when the email is sent. 
// In this example, the email will be sent one minute after the next line executes, 
// provided that the message.SendAndSaveCopy request is processed by the server within one minute. 
string sendTime = DateTime.Now.AddMinutes(1).ToUniversalTime().ToString();
// Specify when to send the email by setting the value of the extended property. 
message.SetExtendedProperty(PidTagDeferredSendTime, sendTime);
// Specify the email body. 
StringBuilder str = new StringBuilder();
str.AppendLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
str.AppendLine("The email message will be sent at: " + sendTime + ".");
message.Body = str.ToString();
Console.WriteLine("");
Console.WriteLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
Console.WriteLine("The email message will be sent at: " + sendTime + ".");
// Submit the request to send the email message. 
message.SendAndSaveCopy();
```

## <a name="send-a-delayed-email-message-by-using-ews"></a><span data-ttu-id="7a311-153">EWS を使用して遅延していたメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7a311-153">Send a delayed email message by using EWS</span></span>
<span data-ttu-id="7a311-154"><a name="bk_senddelayedews"> </a></span><span class="sxs-lookup"><span data-stu-id="7a311-154"></span></span>

<span data-ttu-id="7a311-155">次のコード例は、 [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx)要素、[のプロパティ定義を作成するのには、電子メール メッセージを作成する**SendAndSaveCopy**の**MessageDisposition**値を持つ[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用する方法を示しています。PidTagDeferredSendTime](http://msdn.microsoft.com/ja-jp/library/cc840017.aspx) (0x3FEF0040) プロパティを [送信済みアイテム フォルダーに送信されるメッセージを保存するには、メッセージ、および[SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx)の要素を送信する時間を設定します。</span><span class="sxs-lookup"><span data-stu-id="7a311-155">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, the [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) element to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/ja-jp/library/cc840017.aspx) (0x3FEF0040) property to set a time to send the message, and the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) element to save the sent message in the Sent Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Delayed email</t:Subject>
          <t:Body BodyType="HTML">
            The client submitted the SendAndSaveCopy request at: 1/2/2014 9:08:52 PM.
            The email message will be sent at: 1/2/2014 9:09:52 PM.
          </t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI PropertyTag="16367"
                                PropertyType="SystemTime" />
            <t:Value>2014-01-02T21:09:52.000</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7a311-156">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7a311-156">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7a311-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a311-157">See also</span></span>


- [<span data-ttu-id="7a311-158">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="7a311-158">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7a311-159">EWS を使用して Exchange が電子メール メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="7a311-159">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    

