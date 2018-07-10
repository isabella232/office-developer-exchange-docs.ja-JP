---
title: Exchange EWS を使用して項目をエクスポートします。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをエクスポートする方法について説明します。
ms.openlocfilehash: 65b5b2ef1eba66877d5b6f6c3d4237a26a254196
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758952"
---
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="062b8-103">Exchange EWS を使用して項目をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="062b8-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="062b8-104">Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをエクスポートする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="062b8-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="062b8-p101">EWS マネージ API または EWS を使用すると、さまざまな方法で Exchange からアイテムをエクスポートできます。次の事項によって、使用するオプションが決まります。</span><span class="sxs-lookup"><span data-stu-id="062b8-p101">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways. The option you use depends on:</span></span>
  
- <span data-ttu-id="062b8-107">エクスポートするアイテムの種類。</span><span class="sxs-lookup"><span data-stu-id="062b8-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="062b8-108">Exchange 内のアイテム状態とエクスポートしたアイテムの間で維持する必要のある再現性の程度。</span><span class="sxs-lookup"><span data-stu-id="062b8-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="062b8-109">エクスポートしたアイテムの形式。</span><span class="sxs-lookup"><span data-stu-id="062b8-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="062b8-110">後処理の要件。</span><span class="sxs-lookup"><span data-stu-id="062b8-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="062b8-111">Exchange にアイテムをインポートして戻す必要があるかどうか。</span><span class="sxs-lookup"><span data-stu-id="062b8-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="062b8-p102">この記事では、さまざまなオプションを使用してアイテムをエクスポートする方法について説明します。どのオプションを使用しても Exchange のアイテムのバッチ エクスポートができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-p102">This article shows you how to use each of the different options to export items. You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="062b8-114">カスタム形式でアイテムをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="062b8-114">Export an item into a custom format</span></span>
<span data-ttu-id="062b8-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-115"></span></span>

<span data-ttu-id="062b8-116">[Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS のマネージ API のメソッド呼び出しの結果を使用したり、アプリケーションの要件に合った形式に、EWS の[GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews)操作の結果を解析します。</span><span class="sxs-lookup"><span data-stu-id="062b8-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="062b8-117">データベース、.csv ファイル、または別の形式またはシステムにインポートするためにアイテムをエクスポートするときは、このオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="062b8-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="062b8-118">できますもアイテムを保存する項目、EWS の XML の形式でできる便利な多くのシステムは、XML の解析機能を持つためです。</span><span class="sxs-lookup"><span data-stu-id="062b8-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="062b8-119">プロパティを制御するこのオプションは、エクスポートされるため、 **Item.Bind**メソッドまたは、 **GetItem**操作 (せずに、 [Item.MimeContent](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx)プロパティ) を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="062b8-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="062b8-120">完全な再現性のあるアイテムをエクスポートする</span><span class="sxs-lookup"><span data-stu-id="062b8-120">Export items with full fidelity</span></span>
<span data-ttu-id="062b8-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-121"></span></span>

<span data-ttu-id="062b8-122">忠実にアイテムをエクスポートする場合は、 [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx)の EWS の操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="062b8-122">If you want to export items with full fidelity, you can use the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="062b8-123">**ExportItems**操作は、データ ストリームとして、各項目をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="062b8-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="062b8-124">このデータ ストリームは、解析するためではありませんが、Exchange メールボックスにインポートできるアイテム レベルのバックアップとして使用することができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="062b8-125">呼び出しごとに 100 個を超えるアイテムを含めることを推奨しますが、 **ExportItems**要求のたびに多くの項目を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="062b8-126">EWS 管理 API、実装していない**ExportItems**操作では、EWS のマネージ API を使用する場合のための web 要求を送信するルーチンを記述する必要があります。</span><span class="sxs-lookup"><span data-stu-id="062b8-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="062b8-127">オプションでインデックスを作成して、データ ストリームに関する情報を格納できるように、項目に関するメタデータを取得するのに[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="062b8-127">You can optionally use the [Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="062b8-128">Exchange メールボックスにインポートするアイテムをエクスポートするのには、 **ExportItems**操作を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="062b8-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="062b8-129">次の例では、 **ExportItems**操作を使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="062b8-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="062b8-130">この例では、読みやすさの項目の識別子が短くなります。</span><span class="sxs-lookup"><span data-stu-id="062b8-130">In this example, the item identifier is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

サーバーは、 **NoError**アイテムが正常にエクスポートされることを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx)要素を使用して**ExportItems**の要求に応答します。 応答には、エクスポートされたアイテムと、書き出されたコンテンツが含まれているデータ ストリームの品目 ID も含まれています。 <span data-ttu-id="062b8-133">エクスポートされたアイテムが含まれる SOAP 本文の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="062b8-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:ExportItemsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
        <m:Data>
          AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
          cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
          bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
        </m:Data>
      </m:ExportItemsResponseMessage>
     </m:ResponseMessages>
  </m:ExportItemsResponse>
</s:Body>
```

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="062b8-134">一般的なファイル形式へのエクスポートに MIME ストリームを使用する</span><span class="sxs-lookup"><span data-stu-id="062b8-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="062b8-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-135"></span></span>

<span data-ttu-id="062b8-136">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS の操作を使用するには、項目の MIME の表現を取得します。</span><span class="sxs-lookup"><span data-stu-id="062b8-136">You can use the [Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="062b8-137">Exchange では、各項目の MIME コンテンツを格納するため、MIME ストリームの各項目のデータベース形式に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="062b8-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="062b8-138">この変換は、お勧めしませんがコストがかかるために、規模が大きい項目の MIME ストリームを要求します。</span><span class="sxs-lookup"><span data-stu-id="062b8-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="062b8-139">MIME ストリームにプロパティのセットが含まれているにも注意してください。プロパティ セットに必要なプロパティが含まれていない場合は、他のオプションを検討する必要があります。</span><span class="sxs-lookup"><span data-stu-id="062b8-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="062b8-140">MIME ストリームを使用して電子メールを .eml ファイルと .mht ファイルにエクスポートするために EWS マネージ API を使用する </span><span class="sxs-lookup"><span data-stu-id="062b8-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="062b8-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-141"></span></span>

<span data-ttu-id="062b8-142">Outlook およびその他の一般的なメール ・ アプリケーションは、EML (.eml) ファイル形式を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="062b8-143">次の使用例は、MIME ストリームを使用して電子メールをエクスポートし、EML および MIME HTML (.mht) ファイルを作成するのには、MIME ストリームを使用する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="062b8-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="062b8-144">多くの web ブラウザーでは、MIME HTML ファイル形式をサポートします。</span><span class="sxs-lookup"><span data-stu-id="062b8-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="062b8-145">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="062b8-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEEmail(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    { 
        PropertySet props = new PropertySet(EmailMessageSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = EmailMessage.Bind(service, item.Id, props);
                
        string emlFileName = @"C:\export\email.eml";
        string mhtFileName = @"C:\export\email.mht";
        // Save as .eml.
        using (FileStream fs = new FileStream(emlFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
        // Save as .mht.
        using (FileStream fs = new FileStream(mhtFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="062b8-146">MIME ストリームを使用して iCal ファイルに予定をエクスポートするために EWS マネージ API を使用する</span><span class="sxs-lookup"><span data-stu-id="062b8-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="062b8-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-147"></span></span>

<span data-ttu-id="062b8-148">Outlook およびその他の共通のカレンダー アプリケーションには、iCal (.ics) ファイル形式を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="062b8-149">次の例では、MIME ストリームを使用して予定をエクスポートし、MIME ストリームを使用して、iCal ファイルを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="062b8-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="062b8-150">出席者と添付ファイルに関連するプロパティを含む、MIME ストリームを持つ多くのプロパティはエクスポートされないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="062b8-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="062b8-151">EWS からその他のプロパティをキャプチャするにはそれらを要求し、プライベートの拡張機能としての iCal ファイルに保存します。</span><span class="sxs-lookup"><span data-stu-id="062b8-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="062b8-152">"X-"では、これらのプライベート拡張機能が付けられます。</span><span class="sxs-lookup"><span data-stu-id="062b8-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="062b8-153">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="062b8-153">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="062b8-154">この例では、予定表フォルダーに件名が「財務予測 2015」予定があることも想定しています。</span><span class="sxs-lookup"><span data-stu-id="062b8-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
```cs
private static void ExportMIMEAppointment(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Calendar);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly); 
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems("subject:'2015 Financial Projections'", view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(AppointmentSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Appointment.Bind(service, item.Id, props);
        string iCalFileName = @"C:\export\appointment.ics";
        // Save as .ics.
        using (FileStream fs = new FileStream(iCalFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="062b8-155">MIME ストリームを使用して vCard ファイルに連絡先をエクスポートするために EWS マネージ API を使用する</span><span class="sxs-lookup"><span data-stu-id="062b8-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="062b8-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-156"></span></span>

<span data-ttu-id="062b8-157">Outlook およびその他の一般的な連絡先管理アプリケーションは、vCard (.vcf) ファイル形式を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="062b8-158">次の例では、MIME ストリームを使用して連絡先をエクスポートし、vCard を作成するのには、MIME ストリームを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="062b8-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="062b8-159">EWS からその他のプロパティをキャプチャするにはそれらを要求し、それらに保存します。</span><span class="sxs-lookup"><span data-stu-id="062b8-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="062b8-160">プライベート拡張として vCard。</span><span class="sxs-lookup"><span data-stu-id="062b8-160">vCard as private extensions.</span></span> <span data-ttu-id="062b8-161">"X-"では、これらの拡張子が付けられます。</span><span class="sxs-lookup"><span data-stu-id="062b8-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="062b8-162">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="062b8-162">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEContact(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Contacts);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(ContactSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Contact.Bind(service, item.Id, props);
        string vcfFileName = @"C:\export\contact.vcf";
        // Save as .vcf.
        using (FileStream fs = new FileStream(vcfFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

> [!NOTE]
> <span data-ttu-id="062b8-163">**MimeContent**プロパティを使用して、vCard ファイルをインポートすることはできません。</span><span class="sxs-lookup"><span data-stu-id="062b8-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="062b8-164">[Contact.Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS の操作を使用して連絡先をインポートできます。</span><span class="sxs-lookup"><span data-stu-id="062b8-164">You can import contacts by using the [Contact.Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="062b8-165">MIME ストリームを使用してアイテムをエクスポートするために EWS を使用する</span><span class="sxs-lookup"><span data-stu-id="062b8-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="062b8-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-166"></span></span>

<span data-ttu-id="062b8-167">**GetItem**操作を使用して、項目の MIME ストリームを取得します。</span><span class="sxs-lookup"><span data-stu-id="062b8-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="062b8-168">次の**GetItem**要求では、項目の MIME コンテンツを要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="062b8-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="062b8-p114">次の例は、MIME ストリームを取得する要求に対する応答を示しています。MIME ストリームは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="062b8-p114">The following example shows the response to a request to get the MIME stream. The MIME stream has been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="893" 
                         MinorBuildNumber="17" 
                         Version="V2_10" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:MimeContent CharacterSet="UTF-8">UmVjZ6IGZyb2b2suY29y5hMzgwZTA1YtDQo=</t:MimeContent>
              <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="062b8-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="062b8-171"></span></span>

<span data-ttu-id="062b8-172">アイテムをエクスポートするには後、は、 [Exchange にアイテムをインポート](how-to-import-items-by-using-ews-in-exchange.md)することができます。</span><span class="sxs-lookup"><span data-stu-id="062b8-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="062b8-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="062b8-173">See also</span></span>


- [<span data-ttu-id="062b8-174">Exchange で EWS を使用してアイテムをエクスポートおよびインポートする</span><span class="sxs-lookup"><span data-stu-id="062b8-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="062b8-175">Exchange EWS を使用してアイテムをインポート</span><span class="sxs-lookup"><span data-stu-id="062b8-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="062b8-176">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="062b8-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="062b8-177">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="062b8-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

