---
title: Exchange EWS を使用して添付ファイルを取得します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 12ce3cc0-a201-42e4-93e1-1f57961ff711
description: EWS Managed API または Exchange の EWS を使用して、EWS アイテムから添付物を取得する方法について説明します。
ms.openlocfilehash: 2e1b3cfb346abd068695f66b01f9e34f1f5ff03f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758955"
---
# <a name="get-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="d9bf9-103">Exchange EWS を使用して添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-103">Get attachments by using EWS in Exchange</span></span>

<span data-ttu-id="d9bf9-104">EWS Managed API または Exchange の EWS を使用して、EWS アイテムから添付物を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-104">Learn how to get attachments from EWS items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d9bf9-p101">EWS マネージ APIまたは EWS を使用して、EWS から添付物を取得する方法について説明します。アイテムを取得するための最初の呼び出しには、アイテムの添付コレクションに関するメタデータだけが含まれるので、添付物の取得は常に 2 段階プロセスになります。最初に、アイテムを取得します。次に、添付物を取得します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-p101">You can get attachments from an item by using the EWS Managed API or EWS. Because the initial call to get an item only includes metadata about the attachment collection on the item, retrieving attachments is always a two-step process. First, retrieve the item. Next, retrieve the attachment.</span></span>
  
<span data-ttu-id="d9bf9-109">**表 1. 添付物を追加するためのEWS マネージ API とEWS の操作**</span><span class="sxs-lookup"><span data-stu-id="d9bf9-109">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="d9bf9-110">**タスク**</span><span class="sxs-lookup"><span data-stu-id="d9bf9-110">**Task**</span></span>|<span data-ttu-id="d9bf9-111">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="d9bf9-111">**EWS Managed API method**</span></span>|<span data-ttu-id="d9bf9-112">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="d9bf9-112">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d9bf9-113">アイテム添付を取得する</span><span class="sxs-lookup"><span data-stu-id="d9bf9-113">Get item attachments</span></span>  <br/> |<span data-ttu-id="d9bf9-114">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) の後に [ItemAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9bf9-114">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [ItemAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="d9bf9-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) の後に [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9bf9-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="d9bf9-116">ファイル添付を取得する</span><span class="sxs-lookup"><span data-stu-id="d9bf9-116">Get file attachments</span></span>  <br/> |<span data-ttu-id="d9bf9-117">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) の後に [FileAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9bf9-117">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [FileAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="d9bf9-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) の後に [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d9bf9-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="get-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="d9bf9-119">EWS マネージ API を使用して電子メールから添付物を取得する</span><span class="sxs-lookup"><span data-stu-id="d9bf9-119">Get attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="d9bf9-120"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9bf9-120"></span></span>

<span data-ttu-id="d9bf9-p102">次のコード例は、 [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) メソッドを使用して **EmailMessage** オブジェクトを取得し、添付コレクションを反復処理して、添付物ごとに **FileAttachment.Load** メソッドまたは **ItemAttachment.Load** メソッドを適宜呼び出す方法を示します。各ファイル添付が C:\temp\ フォルダーに保存され、各アイテム添付がメモリに読み込まれます。アイテム添付を保存する方法の詳細については、「 [EWS マネージ API を使用して、添付のある電子メールを保存する](#bk_saveitemattach)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-p102">The following code example shows how to get an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object by using the **Bind** method, then iterate through the attachment collection and call the **FileAttachment.Load** or **ItemAttachment.Load** method on each attachment as appropriate. Each file attachment is saved to the C:\temp\ folder, and each item attachment is loaded into memory. For information about how to save an item attachment, see [Save an attached email by using the EWS Managed API](#bk_saveitemattach).</span></span>
  
<span data-ttu-id="d9bf9-124">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、 **itemId** が添付物の取得元のメッセージの [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) であり、ユーザーが Exchange Server に認証されたと想定しています。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void GetAttachmentsFromEmail(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and load each attachment.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is FileAttachment)
        {
            FileAttachment fileAttachment = attachment as FileAttachment;
            // Load the attachment into a file.
            // This call results in a GetAttachment call to EWS.
            fileAttachment.Load("C:\\temp\\" + fileAttachment.Name);
           
            Console.WriteLine("File attachment name: " + fileAttachment.Name);
        }
        else // Attachment is an item attachment.
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            // Load attachment into memory and write out the subject.
            // This does not save the file like it does with a file attachment.
            // This call results in a GetAttachment call to EWS.
            itemAttachment.Load();
            Console.WriteLine("Item attachment name: " + itemAttachment.Name);
        }
    }
}
```

## <a name="get-an-attachment-from-an-email-by-using-ews"></a><span data-ttu-id="d9bf9-125">EWS を使用して電子メールから添付物を取得する</span><span class="sxs-lookup"><span data-stu-id="d9bf9-125">Get an attachment from an email by using EWS</span></span>
<span data-ttu-id="d9bf9-126"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9bf9-126"></span></span>

<span data-ttu-id="d9bf9-p103">EWS を使用して添付物を取得するには、最初にメッセージと添付コレクションを取得して、取得する添付物の [AttachmentId (GetAttachment と DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) を取得します。1 つ以上の **AttachmentId** の値を取得したら、 [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) 操作を呼び出して、添付物のすべてのプロパティを読み込みます。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-p103">To get attachments by using EWS, you first need to retrieve the message and the attachment collection to get the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to retrieve. After you have one or more **AttachmentId** values to retrieve, call the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation to load all the properties for the attachment.</span></span> 
  
<span data-ttu-id="d9bf9-p104">次のコード例は、[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して電子メール メッセージとメッセージの添付物のコレクションを取得する方法を示しています。これは、EWS マネージ API を使用して [電子メールからすべての添付物を取得する](#bk_getattachewsma)ときに EWS マネージ API が送信する最初の XML 要求でもあります。読みやすくするため、一部の属性の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-p104">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message. This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](#bk_getattachewsma). The values of some attributes are shortened for readability.</span></span>
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Attachments" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="ERu/AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9bf9-132">サーバーは、 **GetItem** 要求に [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode ** 値 、および既存の添付物の [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-132">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
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
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="ERu/AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAYEMnd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="5zTzlqU=" />
                  <t:Name>FileAttachment.txt</t:Name>
                  <t:Size>212</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>false</t:IsContactPhoto>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="Ktum21o=" />
                  <t:Name>Attached Message Item</t:Name>
                  <t:Size>3063</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="d9bf9-133">[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) の値がわかったので、取得する各添付物の [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-133">Now that you have the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values, call [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) on each attachment you want to retrieve.</span></span> 
  
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
    <m:GetAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="5zTzlqU=" />
      </m:AttachmentIds>
    </m:GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9bf9-134">アイテム添付を取得するときは、添付物が正常に取得されたことを示す **NoError** の [ResponseCode](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) の値を含む [GetAttachmentResponse](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) メッセージ、および添付されたアイテムのすべての要素 (このケースでは電子メール メッセージ) をもって、サーバーは **GetAttachment** の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-134">When retrieving an item attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements for the attached item, which in this case is an email message.</span></span>
  
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
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="Ktum21o=" />
              <t:Name>Attached Message Item</t:Name>
              <t:Message>
                <t:ItemClass>IPM.Note</t:ItemClass>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">&amp;lt;meta http-equiv="Content-Type" 
                    content="text/html; charset=utf-8"&amp;gt;Message Item Body</t:Body>
                <t:Size>2859</t:Size>
                <t:IsSubmitted>false</t:IsSubmitted>
                <t:IsDraft>true</t:IsDraft>
                <t:IsFromMe>false</t:IsFromMe>
                <t:IsResend>false</t:IsResend>
                <t:IsUnmodified>false</t:IsUnmodified>
                <t:DateTimeCreated>2014-05-14T17:59:37Z</t:DateTimeCreated>
                <t:ResponseObjects>
                  <t:ForwardItem />
                </t:ResponseObjects>
                <t:DisplayCc />
                <t:DisplayTo>primary; emaildelegate</t:DisplayTo>
                <t:HasAttachments>false</t:HasAttachments>
                <t:Culture>en</t:Culture>
                <t:EffectiveRights>
                  <t:CreateAssociated>false</t:CreateAssociated>
                  <t:CreateContents>false</t:CreateContents>
                  <t:CreateHierarchy>false</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                </t:EffectiveRights>
                <t:LastModifiedName>primary</t:LastModifiedName>
                <t:LastModifiedTime>2014-05-14T17:59:30Z</t:LastModifiedTime>
                <t:IsAssociated>false</t:IsAssociated>
                <t:WebClientReadFormQueryString>?ItemID=AAMk3D&amp;amp;exvsurl=1&amp;amp;viewmodel=
                    ReadMessageItem</t:WebClientReadFormQueryString>
                <t:ConversationId Id="AAQkADIwM2ZlM2ZlLWMwYjctNDg2N/Rc+d0=" />
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:Name>primary</t:Name>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:Name>emaildelegate</t:Name>
                    <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                </t:ToRecipients>
                <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                <t:ConversationIndex>AQHPb55BxR5Fm0Arx0yY4xbL9Fz53Q==</t:ConversationIndex>
                <t:ConversationTopic>Message Item Subject</t:ConversationTopic>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:ItemAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="d9bf9-135">ファイル添付を取得するときは、添付物が正常に取得されたことを示す **NoError** の [ResponseCode](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) の値を含む [GetAttachmentResponse](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) メッセージ、およびファイル添付のすべての要素をもって、サーバーは **GetAttachment** の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-135">When retrieving a file attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements of the file attachment.</span></span>
  
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
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="5zTzlqU=" />
              <t:Name>FileAttachment.txt</t:Name>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="save-an-attached-email-by-using-the-ews-managed-api"></a><span data-ttu-id="d9bf9-136">EWS マネージ API を使用して、添付のある電子メールを保存する</span><span class="sxs-lookup"><span data-stu-id="d9bf9-136">Save an attached email by using the EWS Managed API</span></span>
<span data-ttu-id="d9bf9-137"><a name="bk_saveitemattach"> </a></span><span class="sxs-lookup"><span data-stu-id="d9bf9-137"></span></span>

<span data-ttu-id="d9bf9-p105">EWS マネージ API を使用して電子メールの添付物の内容を保存するには、[MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) をファイルに保存する必要があります。この場合、フォローアップ フラグやカテゴリなど、アイテムに設定された拡張プロパティはすべて失われます。この例では、電子メールの添付物を C:\temp\ フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-p105">In order to save the contents of an email attachment using the EWS Managed API, you need to save the [MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) to a file. In doing so, you will lose any extended properties set on the item, such as follow-up flags and categories. This example saves the email attachment to the to the C:\temp\ folder.</span></span> 
  
<span data-ttu-id="d9bf9-141">なお、アイテム添付は厳密に型指定されたアイテムではないため、別のフォルダーにアイテム添付を移動またはコピーすることはできません。このため、添付物を別のフォルダーに移動しようとしている場合は、次のコード例を使用して、別のフォルダーに[ファイルをインポート](how-to-import-items-by-using-ews-in-exchange.md)します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-141">Note that you cannot move or copy the item attachment to another folder because the item attachment is not a strongly-typed item, so if you're trying to move an attachment to a different folder, use the following code example and then [import the file](how-to-import-items-by-using-ews-in-exchange.md) into a different folder.</span></span> 
  
```cs
public static void SaveEmailAttachment(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is ItemAttachment)
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            itemAttachment.Load(ItemSchema.MimeContent);
            string fileName = "C:\\Temp\\" + itemAttachment.Item.Subject + ".eml";
            // Write the bytes of the attachment into a file.
            File.WriteAllBytes(fileName, itemAttachment.Item.MimeContent.Content);
            Console.WriteLine("Email attachment name: "+ itemAttachment.Item.Subject + ".eml");
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="d9bf9-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9bf9-142">See also</span></span>


- [<span data-ttu-id="d9bf9-143">Exchange の添付物と EWS</span><span class="sxs-lookup"><span data-stu-id="d9bf9-143">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d9bf9-144">Exchange EWS を使用して添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-144">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d9bf9-145">Exchange EWS を使用して添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="d9bf9-145">Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    

