---
title: Exchange で EWS を使用して添付物を追加する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0cbce436-2ae6-4fcc-bd8b-f517a0724e55
description: EWS マネージ API または Exchange の EWS を使用して、添付物を伴う新しくアイテムを作成するか、既存のアイテムに添付物を追加する方法について説明します。
ms.openlocfilehash: dbfff879c92dafeec588d79cddd92e294b763c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758947"
---
# <a name="add-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="14062-103">Exchange で EWS を使用して添付物を追加する</span><span class="sxs-lookup"><span data-stu-id="14062-103">How to: Add attachments by using EWS in Exchange</span></span>

<span data-ttu-id="14062-104">EWS マネージ API または Exchange の EWS を使用して、添付物を伴う新しくアイテムを作成するか、既存のアイテムに添付物を追加する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="14062-104">Learn how to create new items with attachments, or add attachments to existing items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="14062-p101">EWS マネージ API または EWS を使用して、新規アイテムまたは既存のアイテムに、ファイル添付またはアイテム添付を追加できます。EWS マネージ API を使用している場合は、同じメソッドで新規アイテムまたは既存のアイテムに添付物を追加できますが、ファイル添付またはアイテム添付を使用している場合はメソッドが変わります。一方、EWS を使用している場合は、同じ操作でファイル添付またはアイテム添付をアイテムに追加できますが、新規または既存のアイテムに添付物を追加する場合は操作が変わります。</span><span class="sxs-lookup"><span data-stu-id="14062-p101">You can add file attachments or item attachments to new or existing items by using the EWS Managed API or EWS. If you are using the EWS Managed API, you use the same method to add attachments to new or existing items; however, the method changes if you're using a file or item attachment. Conversely, if you are using EWS, you use the same operation to add either a file or item attachment to an item, but the operation changes if you're adding the attachment to a new or existing item.</span></span>
  
<span data-ttu-id="14062-108">**表 1. 添付物を追加するための EWS マネージ API と EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="14062-108">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="14062-109">**タスク**</span><span class="sxs-lookup"><span data-stu-id="14062-109">**Task**</span></span>|<span data-ttu-id="14062-110">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="14062-110">**EWS Managed API method**</span></span>|<span data-ttu-id="14062-111">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="14062-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="14062-112">新規または既存の電子メールにファイル添付を追加する</span><span class="sxs-lookup"><span data-stu-id="14062-112">Add a file attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="14062-113">AttachmentCollection.AddFileAttachment</span><span class="sxs-lookup"><span data-stu-id="14062-113">AttachmentCollection.AddFileAttachment</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="14062-114">新しい電子メールの場合、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="14062-114">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="14062-115">既存の電子メールに追加する場合、[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="14062-115">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
|<span data-ttu-id="14062-116">新規または既存の電子メールにアイテム添付を追加する</span><span class="sxs-lookup"><span data-stu-id="14062-116">Add an item attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="14062-117">AttachmentCollection.AddItemAttachment</span><span class="sxs-lookup"><span data-stu-id="14062-117">AttachmentCollection.AddItemAttachment</span></span>](http://msdn.microsoft.com/ja-JP/library/dd634986%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="14062-118">新しい電子メールの場合、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="14062-118">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="14062-119">既存の電子メールに追加する場合、[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="14062-119">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
   
## <a name="create-an-email-with-file-and-item-attachments-by-using-the-ews-managed-api"></a><span data-ttu-id="14062-120">EWS マネージ API を使用して、ファイル添付およびアイテム添付のある電子メールを作成する</span><span class="sxs-lookup"><span data-stu-id="14062-120">Create an email with file and item attachments by using the EWS Managed API</span></span>
<span data-ttu-id="14062-121"><a name="bk_createattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-121"></span></span>

<span data-ttu-id="14062-122">次のコード例は、複数のファイル添付とアイテム添付のある電子メールを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-122">The following code example shows how to create an email with multiple file attachments and an item attachment by:</span></span> 
  
1. <span data-ttu-id="14062-123">[EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトを使用して、電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-123">Using the [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="14062-124">[AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) と [AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/ja-JP/library/dd634986%28v=exchg.80%29.aspx) メソッドを使用して、添付物をメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="14062-124">Using the [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) and [AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/ja-JP/library/dd634986%28v=exchg.80%29.aspx) methods to add attachments to the message.</span></span> 
    
3. <span data-ttu-id="14062-125">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを使用して、受信者にメッセージを送信し、[送信済みアイテム] フォルダーにメッセージを保存します。</span><span class="sxs-lookup"><span data-stu-id="14062-125">Using the [EmailMessage.SendAndSaveCopyhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipients and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="14062-126">このコード例は、EWS マネージ API を使用してファイル添付をアイテムに追加できる 4 つの方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-126">This code example shows the four ways in which a file attachment can be added to an item by using the EWS Managed API:</span></span>
  
- <span data-ttu-id="14062-127">完全修飾ファイルの場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="14062-127">By using a fully qualified file location.</span></span>
    
- <span data-ttu-id="14062-128">完全修飾ファイルの場所と新しい添付名を使用します。</span><span class="sxs-lookup"><span data-stu-id="14062-128">By using a fully qualified file location and a new attachment name.</span></span>
    
- <span data-ttu-id="14062-129">バイト配列を使用します。</span><span class="sxs-lookup"><span data-stu-id="14062-129">By using a byte array.</span></span>
    
- <span data-ttu-id="14062-130">ストリームを使用します。</span><span class="sxs-lookup"><span data-stu-id="14062-130">By using a stream.</span></span>
    
<span data-ttu-id="14062-131">この例では、アイテム添付が電子メール メッセージと同時に作成されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="14062-131">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="14062-132">アイテム添付として既存の電子メール メッセージを追加する場合には、「[MimeContent および EWS マネージ API を使用して、既存アイテムを新しい電子メールに追加する](#bk_addexistingemailewsma)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14062-132">Note that the item attachment in this example is created at the same time as the email message. To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
<span data-ttu-id="14062-133">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="14062-133">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithAttachments(ExchangeService service)
{
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Message with Attachments";
    message.Body = "This message contains four file attachments 
        and one message item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    message.ToRecipients.Add("ronnie@contoso.com");
    // Add a file attachment by using the fully qualified location of the file. 
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // Add a file attachment by using the fully qualified string name, 
    // and specify the name of the attachment as it will appear in the email.
    // The new name of the file attachment is SecondAttachment.txt.
    message.Attachments.AddFileAttachment("SecondAttachment.txt", "C:\\temp\\FileAttachment2.txt");
    // Add a file attachment by using a byte array.
    // In this example, theBytes is the byte array that represents the content of the image file to attach.
    byte[] theBytes = File.ReadAllBytes("C:\\Temp\\Tulips.jpg");
    // The byte array file attachment is named ThirdAttachment.jpg.
    message.Attachments.AddFileAttachment("ThirdAttachment.jpg", theBytes);
    // Add a file attachment by using a stream.
    FileStream theStream = new FileStream("C:\\temp\\FileAttachment4.txt", FileMode.OpenOrCreate);
    // The streamed file attachment is named FourthAttachment.txt.
    message.Attachments.AddFileAttachment("FourthAttachment.txt", theStream);
    // Add an email message as an item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Name = "Attached Message Item";
    itemAttachment.Item.Subject = "Message Item Subject";
    itemAttachment.Item.Body = "Message Item Body";
    itemAttachment.Item.ToRecipients.Add("sadie@contoso.com");
    itemAttachment.Item.ToRecipients.Add("ronnie@contoso.com");
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-file-and-item-attachments-by-using-ews"></a><span data-ttu-id="14062-134">EWS を使用して、ファイル添付およびアイテム添付のある電子メールを作成する</span><span class="sxs-lookup"><span data-stu-id="14062-134">Create an email with file and item attachments by using EWS</span></span>
<span data-ttu-id="14062-135"><a name="bk_createattachews"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-135"></span></span>

<span data-ttu-id="14062-136">次のコード例は、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して、4 つのファイル添付と 1 つのアイテム添付のある電子メール メッセージを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-136">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with four file attachments and one item attachment. This is also one of the XML requests that the EWS Managed API sends when you create an email with file and item attachments.</span></span> <span data-ttu-id="14062-137">また、これは、[ファイル添付とアイテム添付のある電子メール メッセージを作成する](#bk_createattachewsma)ときに EWS マネージ API が送信する XML 要求の 1 つでもあります。</span><span class="sxs-lookup"><span data-stu-id="14062-137">The following code example shows how to use the CreateItem operation to create an email message with four file attachments and one item attachment. This is also one of the XML requests that the EWS Managed API sends when you [create an email with file and item attachments](#bk_createattachewsma).</span></span>
  
<span data-ttu-id="14062-138">この例では、アイテム添付が電子メール メッセージと同時に作成されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="14062-138">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="14062-139">アイテム添付として既存の電子メール メッセージを追加する場合には、「[MimeContent および EWS マネージ API を使用して、既存アイテムを新しい電子メールに追加する](#bk_addexistingemailewsma)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14062-139">Note that the item attachment in this example is created at the same time as the email message. To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
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
      <m:Items>
        <t:Message>
          <t:Subject>Message with Attachments</t:Subject>
          <t:Body BodyType="HTML">This message contains four file attachments 
              and one message item attachment.</t:Body>
          <t:Attachments>
            <t:FileAttachment>
              <t:Name>FileAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>SecondAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyB0aGUgc2Vjb25kIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>ThirdAttachment.jpg</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>nAoAXNIZMVEZs5GKhdzRcLH/9k=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>FourthAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>obWVudC4=…</t:Content>
            </t:FileAttachment>
            <t:ItemAttachment>
              <t:Name>Attached Message Item</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:Message>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">Message Item Body</t:Body>
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:EmailAddress>mack@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                </t:ToRecipients>
              </t:Message>
            </t:ItemAttachment>
          </t:Attachments>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
            <t:Mailbox>
              <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-140">サーバーは、[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで **CreateItem** 要求に応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の値として **NoError** が含まれており、それは、電子メールと添付物が正常に作成されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-140">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the ItemId of the newly created message.</span></span> <span data-ttu-id="14062-141">新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) と、それぞれの添付物の [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) の値も、この応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-141">The [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values for each of the attachments is also included in the response.</span></span> <span data-ttu-id="14062-142">読みやすくするため、一部の属性の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="14062-142">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="upV4AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXuktU" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="6ts3NuI=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="gOIZx1I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="esRan5I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="t7sU6s=" />
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="XgDCggM=" />
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="14062-143">[新しく作成されたメッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md)には、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="14062-143">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-the-ews-managed-api"></a><span data-ttu-id="14062-144">MimeContent および EWS マネージ API を使用して、既存アイテムを新しい電子メールに追加する</span><span class="sxs-lookup"><span data-stu-id="14062-144">Add an existing item to a new email by using the MimeContent and the EWS Managed API</span></span>
<span data-ttu-id="14062-145"><a name="bk_addexistingemailewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-145"></span></span>

<span data-ttu-id="14062-p106">既存のアイテムをアイテム添付として別のアイテムに追加するには、新しいアイテム添付を作成し、既存のアイテムの内容をその新しいアイテムにコピーする必要があります。これを実行するには、次の 2 つの方法があります。 </span><span class="sxs-lookup"><span data-stu-id="14062-p106">To add an existing item as an item attachment to another item, you need to create a new item attachment and copy the content of the existing item to the new item. There are two ways to do this:</span></span> 
  
1. <span data-ttu-id="14062-148">特に電子メール メッセージを使用している場合は、その電子メールから、新しく作成されたアイテム添付に、[MimeContent](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) プロパティの値をコピーできます。</span><span class="sxs-lookup"><span data-stu-id="14062-148">If you're working with email messages specifically, you can copy the value of the [MimeContent](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) element from the email into the newly created item attachment. You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> <span data-ttu-id="14062-149">この過程で、フォローアップ フラグやカテゴリなどの一部のプロパティが失われますが、標準的な電子メール メッセージには十分機能します。</span><span class="sxs-lookup"><span data-stu-id="14062-149">If you're working with email messages specifically, you can copy the value of the MimeContent element from the email into the newly created item attachment. You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="14062-150">すべての種類のアイテムに完全な再現性が必要な場合は、既存のアイテムにバインドし、すべてのプロパティと拡張プロパティを新しい添付物にコピーできます。</span><span class="sxs-lookup"><span data-stu-id="14062-150">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="14062-151">次のコード例では、**MimeContent** を新しいアイテム添付にコピーする最初の方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-151">The following code example shows the first approach, copying the **MimeContent** into the new item attachment. Following this example is a procedure that shows how you can modify the code to use the second approach.</span></span> <span data-ttu-id="14062-152">例に続いて、2 番目の方法を使用するためにコードを変更する手順を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-152">The following code example shows the first approach, copying the MimeContent into the new item attachment. Following this example is a procedure that shows how you can modify the code to use the second approach.</span></span> 
  
<span data-ttu-id="14062-153">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーから認証されており、**itemId** が、添付するアイテムの [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) であることを想定しています。</span><span class="sxs-lookup"><span data-stu-id="14062-153">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server. The local variable  **itemId**  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
public static void CreateEmailExistingItem(ExchangeService service, ItemId itemId)
{        
    // This method results in a GetItem call to EWS.
    EmailMessage msgToAttach = EmailMessage.Bind(service,itemId, 
        new PropertySet(ItemSchema.MimeContent, ItemSchema.Subject));
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Message with Item Attachment (MimeContent)";
    message.Body = "The attachment to this message was created by copying
        the MimeContent from the original message and adding it to a new item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    // Add an email message item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
    itemAttachment.Name = msgToAttach.Subject;
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

<span data-ttu-id="14062-154">この例を変更して、既存アイテムの各プロパティを新しいアイテム添付にコピーするには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="14062-154">To modify this example to copy each of the properties on the existing item into the new item attachment, do the following:</span></span> 
  
1. <span data-ttu-id="14062-155">**PropertySet.FirstClassProperties** および追加のプロパティ、または必要な拡張プロパティを含むようにプロパティ セットを変更します。</span><span class="sxs-lookup"><span data-stu-id="14062-155">Change the property set to include **PropertySet.FirstClassProperties** and any additional properties or extended properties you need.</span></span> 
    
  ```cs
  // Add additional properties to the PropertySet.
  EmailMessage msgToAttach = EmailMessage.Bind(service, itemId, new PropertySet(PropertySet.FirstClassProperties));
  ```

2. <span data-ttu-id="14062-156">**MimeContent** プロパティは必要ないため、次の行を削除します。</span><span class="sxs-lookup"><span data-stu-id="14062-156">Remove the following line, because you do not need the **MimeContent** property.</span></span> 
    
  ```cs
  itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
  ```

3. <span data-ttu-id="14062-157">既存のアイテムから新しい添付物にコピーする各プロパティについて、この行を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="14062-157">Repeat this line for each property to copy from the existing item to the new attachment. Do not copy the ItemId into the new item attachment because that's a read-only property.</span></span> <span data-ttu-id="14062-158">**ItemId** は読み取り専用プロパティであるため、新しいアイテム添付にはコピーしないでください。</span><span class="sxs-lookup"><span data-stu-id="14062-158">Repeat this line for each property to copy from the existing item to the new attachment. Do not copy the **ItemId** into the new item attachment because that's a read-only property.</span></span> 
    
  ```cs
  itemAttachment.Item.Subject = msgToAttach.Subject;
  ```

4. <span data-ttu-id="14062-159">[PidTagMessageFlags](http://msdn.microsoft.com/ja-JP/library/cc839733.aspx) (0x0E070003) プロパティを、**Sent** への添付物に設定します。</span><span class="sxs-lookup"><span data-stu-id="14062-159">Set the [PidTagMessageFlagshttp://msdn.microsoft.com/ja-JP/library/cc839733.aspx](http://msdn.microsoft.com/ja-JP/library/cc839733.aspx) (0x0E070003) property on the attachment to **Sent**.</span></span>
    
  ```cs
  ExtendedPropertyDefinition sent = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
  msgToAttach.Item.SetExtendedProperty(sent, "1");
  ```

## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-ews"></a><span data-ttu-id="14062-160">MimeContent および EWS を使用して、既存アイテムを新しい電子メールに追加する</span><span class="sxs-lookup"><span data-stu-id="14062-160">Add an existing item to a new email by using the MimeContent and EWS</span></span>
<span data-ttu-id="14062-161"><a name="bk_addexistingemailews"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-161"></span></span>

<span data-ttu-id="14062-162">既存のアイテムを新しいアイテムに追加するには、2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="14062-162">There are two ways to add an existing item to a new item:</span></span> 
  
1. <span data-ttu-id="14062-163">特に電子メール メッセージを使用している場合は、新しく作成したアイテム添付に、電子メールの [MimeContent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) 要素の値をコピーできます。</span><span class="sxs-lookup"><span data-stu-id="14062-163">If you're working with email messages specifically, you can copy the value of the [MimeContent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) element from the email into the newly created item attachment. You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> <span data-ttu-id="14062-164">この過程で、フォローアップ フラグやカテゴリなどの一部のプロパティが失われますが、標準的な電子メール メッセージには十分機能します。</span><span class="sxs-lookup"><span data-stu-id="14062-164">If you're working with email messages specifically, you can copy the value of the MimeContent element from the email into the newly created item attachment. You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="14062-165">すべての種類のアイテムに完全な再現性が必要な場合は、既存のアイテムにバインドし、すべてのプロパティと拡張プロパティを新しい添付物にコピーできます。</span><span class="sxs-lookup"><span data-stu-id="14062-165">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="14062-166">次のコード例は、**MimeContent** 要素を使用して、新しいアイテム添付の **MimeContent** 値に元のアイテムの内容をコピーする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-166">The following code example shows how to use the **MimeContent** element to copy the content of the original item into the **MimeContent** value of the new item attachment. The example uses the following operations:</span></span> <span data-ttu-id="14062-167">この例では、次の操作を使用しています。</span><span class="sxs-lookup"><span data-stu-id="14062-167">The following example uses the</span></span> 
  
1. <span data-ttu-id="14062-168">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — 新しいメッセージでアイテム添付になるメッセージの **MimeContent** および [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) を取得します。</span><span class="sxs-lookup"><span data-stu-id="14062-168">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — To get the **MimeContent** and [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of the message that will become the item attachment on the new message.</span></span> 
    
2. <span data-ttu-id="14062-169">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — 新しい電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-169">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — To create the new email message.</span></span> 
    
3. <span data-ttu-id="14062-170">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) — **GetItem** 操作で取得した **MimeContent** および **Subject** を使用して、新しい添付物を作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-170">[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— To create the new attachment, using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> 
    
4. <span data-ttu-id="14062-171">[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — メッセージを送信し、保存します。</span><span class="sxs-lookup"><span data-stu-id="14062-171">[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — To send and save the message.</span></span> 
    
<span data-ttu-id="14062-172">この例では、まず既存のアイテムの **MimeContent** と **Subject** を取得します。</span><span class="sxs-lookup"><span data-stu-id="14062-172">The example starts by retrieving the **MimeContent** and the **Subject** of the existing item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:MimeContent" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="jCrTAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-173">サーバーは、**GetItem** 要求に対して [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の値として電子メールが正常に作成されたことを示す **NoError**、および電子メールの **MimeContent** と **Subject** が含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-173">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the **AttachmentId** values of the existing attachments.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="944"
                         MinorBuildNumber="11"
                         Version="V2_12"
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
              <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
              <t:ItemId Id="jCrTAAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi+7u" />
              <t:Subject>Play tennis?</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="14062-174">次に、**CreateItem** 操作を呼び出して新しい電子メールを作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-174">Next, call the **CreateItem** operation to create the new email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Message with Item Attachment (MimeContent)</t:Subject>
          <t:Body BodyType="HTML">The attachment to this message was created by copying the MimeContent from the original message and adding it to a new item attachment.</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>primary@contoso1000.onmicrosoft.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-175">サーバーは、[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで **CreateItem** 要求に応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の値として **NoError** が含まれており、それは、電子メールが正常に作成されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-175">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the ItemId of the newly created message.</span></span>
  
<span data-ttu-id="14062-176">次に、**GetItem** 操作で取得した **MimeContent** および **Subject** を使用して、新しいアイテム添付を作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-176">CreateAttachment— To create the new attachment, using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> <span data-ttu-id="14062-177">[ParentItemId](http://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) 要素の値には、**CreateItem** 応答で返された **ItemId** の値を使用して入力します。</span><span class="sxs-lookup"><span data-stu-id="14062-177">Next, create the new item attachment by using the **MimeContent** and **Subject** retrieved by the GetItem operation. The value of the [ParentItemId](http://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) element is populated by using the ItemId value returned in the CreateItem response.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateAttachment>
      <m:ParentItemId Id="jDKsAAA=" />
      <m:Attachments>
        <t:ItemAttachment>
          <t:Name>Play tennis?</t:Name>
          <t:IsInline>false</t:IsInline>
          <t:Message>
            <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
          </t:Message>
        </t:ItemAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-178">サーバーは、**CreateAttachment** 要求に対して、[CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の値として添付物が正常に作成されたことを示す **NoError**、および新しく作成された添付物の [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-178">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
<span data-ttu-id="14062-179">これで新しいメッセージが作成され、アイテムが添付されたため、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作を呼び出して、[新しく作成されたメッセージを送信](how-to-send-email-messages-by-using-ews-in-exchange.md)できます。</span><span class="sxs-lookup"><span data-stu-id="14062-179">Now that the new message has been created, and the item was attached, you can [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md) by calling the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="jDKsAAA="
                  ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi/q/" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-180">サーバーは、[SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) メッセージで **SendItem** 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-180">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="create-an-email-with-an-inline-attachment-by-using-the-ews-managed-api"></a><span data-ttu-id="14062-181">EWS マネージ API を使用して、インライン添付のある電子メールを作成する</span><span class="sxs-lookup"><span data-stu-id="14062-181">Create an email with an inline attachment by using the EWS Managed API</span></span>
<span data-ttu-id="14062-182"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-182"></span></span>

<span data-ttu-id="14062-183">次のコード例は、インライン添付のある電子メールを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-183">The following code example shows how to create an email with an inline attachment by:</span></span>
  
1. <span data-ttu-id="14062-184">[EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトを使用して、電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="14062-184">Using the [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="14062-185">[EmailMessage.Body](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) プロパティを、インライン添付を含む HTML 本文に設定します。</span><span class="sxs-lookup"><span data-stu-id="14062-185">Setting the [EmailMessage.Bodyhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) property to an HTML body that includes an inline attachment.</span></span> 
    
3. <span data-ttu-id="14062-186">[AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) メソッドを使用して、添付物をメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="14062-186">Using the [AttachmentCollection.AddFileAttachmenthttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) method to add the attachment to the message.</span></span> 
    
4. <span data-ttu-id="14062-187">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを使用して、受信者にメッセージを送信し、[送信済みアイテム] フォルダーにメッセージを保存します。</span><span class="sxs-lookup"><span data-stu-id="14062-187">Using the [EmailMessage.SendAndSaveCopyhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="14062-188">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="14062-188">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithInlineAttachment(ExchangeService service)
{
    // Create the HTML body with the content identifier of the attachment.
    string html = @"<html>
                        <head>
                        </head>
                        <body>
                        <img width=100 height=100 id=""1"" src=""cid:Party.jpg"">
                        </body>
                        </html>";
         
    // Create the email message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Inline Attachment";
    message.Body = new MessageBody(BodyType.HTML, html);
    message.ToRecipients.Add("sadie@contoso.com");
    // Add the attachment to the local copy of the email message.
    string file = @"C:\Temp\Party.jpg";
    message.Attachments.AddFileAttachment("Party.jpg", file);
    message.Attachments[0].IsInline = true;
    message.Attachments[0].ContentId = "Party.jpg";
         
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-an-inline-attachment-by-using-ews"></a><span data-ttu-id="14062-189">EWS を使用して、インライン添付のある電子メールを作成する</span><span class="sxs-lookup"><span data-stu-id="14062-189">Create an email with an inline attachment by using EWS</span></span>
<span data-ttu-id="14062-190"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-190"></span></span>

<span data-ttu-id="14062-191">次のコード例は、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して、インライン ファイル添付のある電子メール メッセージを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-191">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with an inline file attachment.</span></span> <span data-ttu-id="14062-192">[Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) 要素の **BodyType** 属性は、コンテンツが HTML 形式であり、イメージ ソースが含まれることを示します。</span><span class="sxs-lookup"><span data-stu-id="14062-192">The **BodyType** attribute of the [Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) element indicates that the content is in HTML format and includes the image source.</span></span> <span data-ttu-id="14062-193">また、これは、EWS マネージ API を使用して[インライン添付のある電子メール メッセージを作成する](#bk_createinlineattachewsma)ときに送信される XML 要求の 1 つでもあります。</span><span class="sxs-lookup"><span data-stu-id="14062-193">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [create an email with an inline attachment](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Inline Attachment</t:Subject>
          <t:Body BodyType="HTML">
            &amp;lt;html&amp;gt;
            &amp;lt;head&amp;gt;
            &amp;lt;/head&amp;gt;
            &amp;lt;body&amp;gt;
            &amp;lt;img width=100 height=100 id="1" src="cid:Party.jpg"&amp;gt;
            &amp;lt;/body&amp;gt;
            &amp;lt;/html&amp;gt;
          </t:Body>
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

<span data-ttu-id="14062-194">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-194">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="14062-195">[新しく作成されたメッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md)には、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="14062-195">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-attachment-to-an-existing-email-by-using-the-ews-managed-api"></a><span data-ttu-id="14062-196">EWS マネージ API を使用して、添付物を既存の電子メールに追加する</span><span class="sxs-lookup"><span data-stu-id="14062-196">Add an attachment to an existing email by using the EWS Managed API</span></span>
<span data-ttu-id="14062-197"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-197"></span></span>

<span data-ttu-id="14062-198">次のコード例は、既存の電子メールに添付物を追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-198">The following code example shows how to add an attachment to an existing email by:</span></span> 
  
1. <span data-ttu-id="14062-199">[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) メソッドを使用して、既存の電子メール メッセージにバインドします。</span><span class="sxs-lookup"><span data-stu-id="14062-199">Using the [EmailMessage.Bindhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message.</span></span> 
    
2. <span data-ttu-id="14062-200">**AddFileAttachment** メソッドを使用して、ファイル添付をメッセージに追加します。</span><span class="sxs-lookup"><span data-stu-id="14062-200">Adding a file attachment to the message by using the **AddFileAttachment** method.</span></span> 
    
3. <span data-ttu-id="14062-201">[EmailMessage.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) メソッドを呼び出すことによって、更新内容を保存します。</span><span class="sxs-lookup"><span data-stu-id="14062-201">Saving the updates by calling the [EmailMessage.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="14062-202">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="14062-202">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
public static void AddAttachmentToExisting(ExchangeService service, ItemId itemId)
{
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId);
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // This method results in a CreateAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="add-an-attachment-to-an-existing-email-by-using-ews"></a><span data-ttu-id="14062-203">EWS を使用して、添付物を既存の電子メールに追加する</span><span class="sxs-lookup"><span data-stu-id="14062-203">Add an attachment to an existing email by using EWS</span></span>
<span data-ttu-id="14062-204"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="14062-204"></span></span>

<span data-ttu-id="14062-205">次のコード例は、[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) 操作を使用して、ファイル添付を既存の電子メール メッセージに追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="14062-205">The following code example shows how to use the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation to add a file attachment to an existing email message. This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to add an attachment to an existing email.</span></span> <span data-ttu-id="14062-206">また、これは EWS マネージ API を使用して[添付物を既存の電子メールに追加する](#bk_createinlineattachewsma)ときに送信される XML 要求の 1 つでもあります。</span><span class="sxs-lookup"><span data-stu-id="14062-206">The following code example shows how to use the CreateAttachment operation to add a file attachment to an existing email message. This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [add an attachment to an existing email](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateAttachment>
      <m:ParentItemId Id="uqE2AAA=" />
      <m:Attachments>
        <t:FileAttachment>
          <t:Name>FileAttachment.txt</t:Name>
          <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
        </t:FileAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="14062-207">サーバーは、**CreateAttachment** 要求に対して、[CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の値として添付物が正常に作成されたことを示す **NoError**、および新しく作成された添付物の [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="14062-207">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="yRLhCh8="
                              RootItemId="uqE2AAA="
                              RootItemChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcf" />
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:CreateAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="14062-208">関連項目</span><span class="sxs-lookup"><span data-stu-id="14062-208">See also</span></span>


- [<span data-ttu-id="14062-209">Exchange における添付物と EWS</span><span class="sxs-lookup"><span data-stu-id="14062-209">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="14062-210">Exchange で EWS を使用して添付物を追加する</span><span class="sxs-lookup"><span data-stu-id="14062-210">How to: Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="14062-211">Exchange で EWS を使用して添付物を削除する</span><span class="sxs-lookup"><span data-stu-id="14062-211">How to: Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="14062-212">Exchange で EWS を使用して添付物を取得する</span><span class="sxs-lookup"><span data-stu-id="14062-212">How to: Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="14062-213">Exchange で EWS を使用してメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="14062-213">How to: Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

