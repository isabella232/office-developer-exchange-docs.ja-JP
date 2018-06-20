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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758952"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Exchange EWS を使用して項目をエクスポートします。

Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをエクスポートする方法について説明します。
  
EWS マネージ API または EWS を使用すると、さまざまな方法で Exchange からアイテムをエクスポートできます。次の事項によって、使用するオプションが決まります。
  
- エクスポートするアイテムの種類。
    
- Exchange 内のアイテム状態とエクスポートしたアイテムの間で維持する必要のある再現性の程度。
    
- エクスポートしたアイテムの形式。
    
- 後処理の要件。
    
- Exchange にアイテムをインポートして戻す必要があるかどうか。
    
この記事では、さまざまなオプションを使用してアイテムをエクスポートする方法について説明します。どのオプションを使用しても Exchange のアイテムのバッチ エクスポートができます。
  
## <a name="export-an-item-into-a-custom-format"></a>カスタム形式でアイテムをエクスポートする
<a name="bk_exportcustom"> </a>

[Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS のマネージ API のメソッド呼び出しの結果を使用したり、アプリケーションの要件に合った形式に、EWS の[GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews)操作の結果を解析します。 データベース、.csv ファイル、または別の形式またはシステムにインポートするためにアイテムをエクスポートするときは、このオプションを使用します。 できますもアイテムを保存する項目、EWS の XML の形式でできる便利な多くのシステムは、XML の解析機能を持つためです。 プロパティを制御するこのオプションは、エクスポートされるため、 **Item.Bind**メソッドまたは、 **GetItem**操作 (せずに、 [Item.MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx)プロパティ) を使用することをお勧めします。 
  
## <a name="export-items-with-full-fidelity"></a>完全な再現性のあるアイテムをエクスポートする
<a name="bk_exportfullfidelity"> </a>

忠実にアイテムをエクスポートする場合は、 [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx)の EWS の操作を使用できます。 **ExportItems**操作は、データ ストリームとして、各項目をエクスポートします。 このデータ ストリームは、解析するためではありませんが、Exchange メールボックスにインポートできるアイテム レベルのバックアップとして使用することができます。 呼び出しごとに 100 個を超えるアイテムを含めることを推奨しますが、 **ExportItems**要求のたびに多くの項目を含めることができます。 EWS 管理 API、実装していない**ExportItems**操作では、EWS のマネージ API を使用する場合のための web 要求を送信するルーチンを記述する必要があります。 オプションでインデックスを作成して、データ ストリームに関する情報を格納できるように、項目に関するメタデータを取得するのに[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドを使用できます。 
  
Exchange メールボックスにインポートするアイテムをエクスポートするのには、 **ExportItems**操作を使用することをお勧めします。 
  
次の例では、 **ExportItems**操作を使用する方法を示します。 この例では、読みやすさの項目の識別子が短くなります。 
  
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

サーバーは、 **NoError**アイテムが正常にエクスポートされることを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx)要素を使用して**ExportItems**の要求に応答します。 応答には、エクスポートされたアイテムと、書き出されたコンテンツが含まれているデータ ストリームの品目 ID も含まれています。 エクスポートされたアイテムが含まれる SOAP 本文の例を次に示します。
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>一般的なファイル形式へのエクスポートに MIME ストリームを使用する
<a name="bk_exportfullfidelity"> </a>

[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS の操作を使用するには、項目の MIME の表現を取得します。 Exchange では、各項目の MIME コンテンツを格納するため、MIME ストリームの各項目のデータベース形式に変換する必要があります。 この変換は、お勧めしませんがコストがかかるために、規模が大きい項目の MIME ストリームを要求します。 MIME ストリームにプロパティのセットが含まれているにも注意してください。プロパティ セットに必要なプロパティが含まれていない場合は、他のオプションを検討する必要があります。 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>MIME ストリームを使用して電子メールを .eml ファイルと .mht ファイルにエクスポートするために EWS マネージ API を使用する 
<a name="bk_exportemailmime"> </a>

Outlook およびその他の一般的なメール ・ アプリケーションは、EML (.eml) ファイル形式を開くことができます。 次の使用例は、MIME ストリームを使用して電子メールをエクスポートし、EML および MIME HTML (.mht) ファイルを作成するのには、MIME ストリームを使用する方法を示しています。 多くの web ブラウザーでは、MIME HTML ファイル形式をサポートします。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>MIME ストリームを使用して iCal ファイルに予定をエクスポートするために EWS マネージ API を使用する
<a name="bk_exporticalmime"> </a>

Outlook およびその他の共通のカレンダー アプリケーションには、iCal (.ics) ファイル形式を開くことができます。 次の例では、MIME ストリームを使用して予定をエクスポートし、MIME ストリームを使用して、iCal ファイルを作成する方法を示します。 出席者と添付ファイルに関連するプロパティを含む、MIME ストリームを持つ多くのプロパティはエクスポートされないことを確認します。 EWS からその他のプロパティをキャプチャするにはそれらを要求し、プライベートの拡張機能としての iCal ファイルに保存します。 "X-"では、これらのプライベート拡張機能が付けられます。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 この例では、予定表フォルダーに件名が「財務予測 2015」予定があることも想定しています。 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>MIME ストリームを使用して vCard ファイルに連絡先をエクスポートするために EWS マネージ API を使用する
<a name="bk_exportvcardmime"> </a>

Outlook およびその他の一般的な連絡先管理アプリケーションは、vCard (.vcf) ファイル形式を開くことができます。 次の例では、MIME ストリームを使用して連絡先をエクスポートし、vCard を作成するのには、MIME ストリームを使用する方法を示します。 EWS からその他のプロパティをキャプチャするにはそれらを要求し、それらに保存します。 プライベート拡張として vCard。 "X-"では、これらの拡張子が付けられます。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 
  
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
> **MimeContent**プロパティを使用して、vCard ファイルをインポートすることはできません。 [Contact.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS の操作を使用して連絡先をインポートできます。 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>MIME ストリームを使用してアイテムをエクスポートするために EWS を使用する
<a name="bk_exportewsmime"> </a>

**GetItem**操作を使用して、項目の MIME ストリームを取得します。 次の**GetItem**要求では、項目の MIME コンテンツを要求する方法を示します。 
  
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

次の例は、MIME ストリームを取得する要求に対する応答を示しています。MIME ストリームは、読みやすくするために短縮されています。
  
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
<a name="bk_exportfullfidelity"> </a>

アイテムをエクスポートするには後、は、 [Exchange にアイテムをインポート](how-to-import-items-by-using-ews-in-exchange.md)することができます。
  
## <a name="see-also"></a>関連項目


- [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用してアイテムをインポート](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    

