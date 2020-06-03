---
title: Exchange の EWS を使用してアイテムをインポートする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをインポートする方法について説明します。
ms.openlocfilehash: bc874c667c31beb4e59a305626247488cb1a1781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527986"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="d5835-103">Exchange の EWS を使用してアイテムをインポートする</span><span class="sxs-lookup"><span data-stu-id="d5835-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="d5835-104">Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをインポートする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5835-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d5835-p101">多数のシステムに予定、電子メール、連絡先およびタスクが格納されているときに、それらのアイテムをいくつかの方法で Exchange にインポートできます。Exchange へのアイテムのインポートは、それらのアイテムに対するメールボックスのリレーションシップを維持しない場合は簡単です。EWS マネージ API の [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) メソッドを使用するか、EWS の [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用して、Exchange メールボックスにアイテムを作成します。ただし、この単純なアプローチでは、サポートされないシナリオがあります。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="d5835-p101">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways. Importing items into Exchange is simple when mailbox relationships aren't maintained on those items. You can use the [Item.Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox. The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="d5835-p102">出席者 (会議) によって予定をインポートするときに、開催者と出席者のリレーションシップを維持できません。つまり、開催者と出席者のリレーションシップを確立するには、会議の開催者が会議出席依頼を出席者に再送信する必要があるということです。出席者の予定表にインポートされた予定は、会議の開催者の予定に関連付けられることはありません。出席者は、開催者と出席者のリレーションシップを確立するために、開催者からの会議出席依頼の再送信を受け入れる必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5835-p102">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings). This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees. If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment. The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="d5835-113">割り当て済みのタスクがインポートされるときに、割り当て先に関する情報が保持されません。</span><span class="sxs-lookup"><span data-stu-id="d5835-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="d5835-114">どのインポート オプションを使用しても、Exchange にアイテムをバッチ インポートできます。</span><span class="sxs-lookup"><span data-stu-id="d5835-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="d5835-115">アイテムのインポートに EWS マネージ API または EWS のアイテムの種類を使用する</span><span class="sxs-lookup"><span data-stu-id="d5835-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="d5835-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="d5835-116"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="d5835-p103">EWS マネージ API または EWS を使用して、別のシステムから電子メール、連絡先、予定、またはタスクをインポートできます。インポートする内容に応じて、次のいずれかのオブジェクトにインポート元形式からの[プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を設定するだけです。</span><span class="sxs-lookup"><span data-stu-id="d5835-p103">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems. Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="d5835-119">**表 1. EWS マネージ API のオブジェクトと EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="d5835-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="d5835-120">**EWS マネージ API のオブジェクト**</span><span class="sxs-lookup"><span data-stu-id="d5835-120">**EWS Managed API object**</span></span>|<span data-ttu-id="d5835-121">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="d5835-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5835-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="d5835-122">EmailMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d5835-123">Message</span><span class="sxs-lookup"><span data-stu-id="d5835-123">Message</span></span>](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="d5835-124">Contact</span><span class="sxs-lookup"><span data-stu-id="d5835-124">Contact</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d5835-125">Contact</span><span class="sxs-lookup"><span data-stu-id="d5835-125">Contact</span></span>](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="d5835-126">Appointment</span><span class="sxs-lookup"><span data-stu-id="d5835-126">Appointment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d5835-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d5835-127">CalendarItem</span></span>](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="d5835-128">Task</span><span class="sxs-lookup"><span data-stu-id="d5835-128">Task</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d5835-129">Task</span><span class="sxs-lookup"><span data-stu-id="d5835-129">Task</span></span>](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="d5835-p104">EWS マネージ API の [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) メソッドまたは EWS の [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用して、アイテムのインポートを実行します。このアプローチでは、どのプロパティをインポートするかを制御できるため、別のシステムからアイテムをインポートする場合にお勧めします。アイテムにプロパティを設定して、アイテムを保存する方法の詳細については、「 [EWS マネージ API を使用してアイテムを作成する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma)」または「[EWS を使用してアイテムを作成する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5835-p104">Use the [Item.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items. We recommend this approach when you're importing items from other systems because you have control over which properties get imported. For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="d5835-133">完全な再現性のあるアイテムをインポートする</span><span class="sxs-lookup"><span data-stu-id="d5835-133">Import items with full fidelity</span></span>
<span data-ttu-id="d5835-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="d5835-134"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="d5835-p105">EWS の [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) 操作を使用すると、アイテムをデータ ストリームとしてアップロードできます。このアイテムのデータ ストリーム表現は、 [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) 操作の呼び出しの結果から得る必要があります。EWS マネージ API は **UploadItems** 操作を実装していないため、EWS マネージ API を使用する場合は、Web 要求を送信するルーチンを記述することが必要になります。</span><span class="sxs-lookup"><span data-stu-id="d5835-p105">You can use the [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream. This data stream representation of an item has to come from the results of an [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call. Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="d5835-138">これは、別の Exchange サーバーからエクスポートされたアイテムを最も簡単にインポートする方法です。</span><span class="sxs-lookup"><span data-stu-id="d5835-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="d5835-139">次に示す例では、読みやすくなるように識別子と **Data** 要素の内容が簡略化されています。</span><span class="sxs-lookup"><span data-stu-id="d5835-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId  Id="AAMkADEzOTE7kV0AAA=" ChangeKey="AQAAAA=="/>
          <t:Data>AQAAAAgAAAAAAQAAAAADABZADQASDkANABMO</t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d5835-p106">サーバーは **UploadItems** 要求に [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) 要素で応答します。この要素には、アイテムが正常にアップロードされたことを示す [NoError](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 要素の値が含まれていてます。この応答には、アップロードしたアイテムのアイテム ID も含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5835-p106">The server responds to the **UploadItems** request with an [UploadItemsResponse](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) element that that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the item was successfully uploaded. The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="d5835-142">一般的なファイル形式からのインポートに MIME ストリームを使用する</span><span class="sxs-lookup"><span data-stu-id="d5835-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="d5835-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="d5835-143"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="d5835-p107">EWS では、EML (.eml) ファイルと iCal (.ics) ファイルをインポートできます。独自の MIME コンテンツをテストして、Exchange の MIME パーサーが MIME ストリームのコンテンツを処理する方法を確認してください。MIME ストリームは便利に使用できますが、一般に、[アイテムのインポートに EWS マネージ API または EWS のアイテムの種類を使用する](#bk_importproperties)ほうが優れています。ここには、[vCard をインポートする](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50)方法の例があります。</span><span class="sxs-lookup"><span data-stu-id="d5835-p107">EWS can import EML (.eml) and iCal (.ics) files. You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream. Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties). Here's an example of how to [import a vCard](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="d5835-148">MIME ストリームを使用して EML ファイルから電子メールをインポートするために EWS マネージ API を使用する</span><span class="sxs-lookup"><span data-stu-id="d5835-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="d5835-p108">次の例は、EML ファイルのコンテンツで [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) プロパティを設定して、電子メールをメールボックスにインポートする方法を示しています。さらに、インポートした電子メールの [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) 拡張プロパティを設定して、メールボックス内で下書きアイテムとして表示されないようにする方法も示しています。この例では、 **service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="d5835-p108">The following example shows how to set the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox. This example also shows how to set the [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item. This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void UploadMIMEEmail(ExchangeService service)
{
    EmailMessage email = new EmailMessage(service);
    
    string emlFileName = @"C:\import\email.eml";
    using (FileStream fs = new FileStream(emlFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .eml file to the MimeContent property.
        email.MimeContent = new MimeContent("UTF-8", bytes);
    }
    
    // Indicate that this email is not a draft. Otherwise, the email will appear as a 
    // draft to clients.
    ExtendedPropertyDefinition PR_MESSAGE_FLAGS_msgflag_read = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
    email.SetExtendedProperty(PR_MESSAGE_FLAGS_msgflag_read, 1);
    // This results in a CreateItem call to EWS. The email will be saved in the Inbox folder.
    email.Save(WellKnownFolderName.Inbox);
}
```

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="d5835-152">MIME ストリームを使用して iCal ファイルから予定をインポートするために EWS マネージ API を使用する</span><span class="sxs-lookup"><span data-stu-id="d5835-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="d5835-p109">MIME ストリームを使用することで、単純な予定を iCalendar ファイルの形式でインポートできます。会議 (出席者を伴う予定) はインポートできません。これは、開催者と出席者のリレーションシップは、[Exchange 予定表作成](calendars-and-ews-in-exchange.md)ワークフローの一環として設定される必要があるためです。MIME ストリームでは、出席者をキャプチャできません。</span><span class="sxs-lookup"><span data-stu-id="d5835-p109">You can import simple appointments in the form of iCalendar files by using the MIME stream. You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow. Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="d5835-156">次のコード例は、単純な .ics ファイルをユーザーのメールボックスにインポートする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d5835-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
```cs
private static void UploadMIMEAppointment(ExchangeService service)
{
    Appointment appointment = new Appointment(service);
    string iCalFileName = @"C:\import\appointment.ics";
    using (FileStream fs = new FileStream(iCalFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .ics file to the MimeContent property.
        appointment.MimeContent = new MimeContent("UTF-8", bytes);
    }
    // This results in a CreateItem call to EWS. 
    appointment.Save(WellKnownFolderName.Calendar);
}
```

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="d5835-157">MIME ストリームを使用してアイテムをインポートするために EWS を使用する</span><span class="sxs-lookup"><span data-stu-id="d5835-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="d5835-158">EWS の [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用すると、EML アイテムと iCal アイテムは、それぞれの MIME ストリームを使用することでインポートできます。</span><span class="sxs-lookup"><span data-stu-id="d5835-158">You can use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body >
    <m:CreateItem>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </m:SavedItemFolderId> 
        <m:Items>
        <t:Message>
          <t:MimeContent CharacterSet="UTF-8">
            <!-- Insert MIME content here-->
          </t:MimeContent>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="d5835-159">次の手順</span><span class="sxs-lookup"><span data-stu-id="d5835-159">Next steps</span></span>
<span data-ttu-id="d5835-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="d5835-160"><a name="bk_importproperties"> </a></span></span>

<span data-ttu-id="d5835-161">メールボックスにアイテムをインポートしたら、[インポートしたアイテムを保存するためのカスタム フォルダーを作成する](how-to-work-with-folders-by-using-ews-in-exchange.md)ことや、[クライアントとメールボックスのアイテムを同期する](mailbox-synchronization-and-ews-in-exchange.md)ことが必要になります。</span><span class="sxs-lookup"><span data-stu-id="d5835-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d5835-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5835-162">See also</span></span>


- [<span data-ttu-id="d5835-163">Exchange で EWS を使用してアイテムをエクスポートおよびインポートする</span><span class="sxs-lookup"><span data-stu-id="d5835-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d5835-164">Exchange の EWS を使用してアイテムをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="d5835-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d5835-165">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="d5835-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="d5835-166">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="d5835-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

