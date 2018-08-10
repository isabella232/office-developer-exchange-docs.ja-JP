---
title: Exchange で EWS を使用してアイテムをエクスポートする
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをエクスポートする方法について説明します。
ms.openlocfilehash: 65b5b2ef1eba66877d5b6f6c3d4237a26a254196
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758952"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Exchange で EWS を使用してアイテムをエクスポートする

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

EWS マネージ API の [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) メソッドの呼び出しの結果を使用するか、EWS の [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) 操作の結果を解析することで、カスタム アプリケーションの要件で動作する形式に変換できます。 このオプションは、アイテムをエクスポートして、データベースや .csv ファイルなどの形式やシステムにインポートする場合に使用します。 アイテムを EWS XML の形式で保存することもできます。多くのシステムに XML の解析機能があるため、この形式は実用的です。 **Item.Bind** メソッドまたは **GetItem** 操作を ([Item.MimeContent](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) プロパティなしで) 使用することをお勧めします。このオプションにより、エクスポートするプロパティを制御できるようになります。 
  
## <a name="export-items-with-full-fidelity"></a>完全な再現性のあるアイテムをエクスポートする
<a name="bk_exportfullfidelity"> </a>

完全な再現性のあるアイテムをエクスポートする場合は、EWS の [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) 操作を使用できます。 **ExportItems** 操作では、データ ストリームとして各アイテムをエクスポートします。 このデータ ストリームは解析には向いていませんが、Exchange メールボックスにインポートして戻せるアイテム レベルのバックアップとして使用できます。 それぞれの **ExportItems** 要求には多数のアイテムを含めることができますが、呼び出しごとに含めるアイテム数は 100 個を超えないようにしてください。 EWS マネージ API は **ExportItems** 操作を実装していないため、EWS マネージ API を使用する場合は、Web 要求を送信するルーチンを記述することが必要になります。 [Item.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドをオプションとして使用するとアイテムに関するメタデータを取得できます。これにより、データ ストリームに関する情報のインデックス作成と保存が可能になります。 
  
Exchange メールボックスにインポートする予定のあるアイテムをエクスポートする場合は、**ExportItems** 操作の使用をお勧めします。 
  
次の例は、**ExportItems** 操作の使用方法を示しています。 この例では、読みやすくなるようにアイテム ID が短くしてあります。 
  
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

サーバーは **ExportItems** 要求に [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) 要素で応答します。この要素には、値が **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素が含まれており、それは、アイテムが正常にアップロードされたことを示しています。 この応答には、エクスポートしたアイテムのアイテム ID とエクスポートしたコンテンツを格納しているデータ ストリームも含まれています。 次の例は、エクスポートしたアイテムを格納している SOAP ボディを示しています。
  
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

EWS マネージ API の [Item.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドまたは EWS の [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用すると、アイテムの MIME 表現を得られます。 Exchange は各アイテムの MIME コンテンツを保存しないため、各アイテムのデータベース表現を MIME ストリームに変換する必要があります。 この変換にはコストがかかるため、規模の大きなアイテムに対する MIME ストリームの要求はお勧めできません。 また、MIME ストリームには限定的なプロパティのセットが含まれている点にも注意してください。そのプロパティのセットに必要とするものが含まれていない場合は、別のオプションを検討することが必要になります。 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>MIME ストリームを使用して電子メールを .eml ファイルと .mht ファイルにエクスポートするために EWS マネージ API を使用する
<a name="bk_exportemailmime"> </a>

Outlook などの一般的なメール アプリケーションは、EML (.eml) ファイル形式を開くことができます。 次の例は、MIME ストリームを使用して電子メールをエクスポートする方法と、EML および MIME HTML (.mht) ファイルを作成するために MIME ストリームを使用する方法を示しています。 多数の Web ブラウザーが MIME HTML ファイル形式をサポートしています。 この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 
  
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

Outlook などの一般的な予定表アプリケーションは、iCal (.ics) ファイル形式を開くことができます。 次の例は、MIME ストリームを使用して予定をエクスポートする方法と、iCal ファイルを作成するために MIME ストリームを使用する方法を示しています。 MIME ストリームでは、多くのプロパティ (出席者や添付物関連のプロパティなど) がエクスポートされない点に注意してください。 その他のプロパティを EWS から取得するには、そのプロパティを要求してプライベート拡張機能として iCal ファイルに保存します。 こうしたプライベート拡張機能には、プレフィックスの "x-" が付いています。 
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 また、予定表フォルダー内に "2015 Financial Projections" という件名の予定があることも前提としています。 
  
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

Outlook などの連絡先管理アプリケーションは、vCard (.vcf) ファイル形式を開くことができます。 次の例は、MIME ストリームを使用して連絡先をエクスポートする方法と、vCard を作成するために MIME ストリームを使用する方法を示しています。 その他のプロパティを EWS から取得するには、そのプロパティを要求してプライベート拡張機能として . vCard に保存します。 こうした拡張機能には、プレフィックスの "x-" が付いています。 
  
この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 
  
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
> vCard のファイルは、**MimeContent** プロパティを使用してインポートすることはできません。 EWS マネージ API の [Contact.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) メソッドまたは EWS の [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) 操作を使用すると、連絡先をインポートできます。 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>MIME ストリームを使用してアイテムをエクスポートするために EWS を使用する
<a name="bk_exportewsmime"> </a>

**GetItem** 操作を使用して、アイテムの MIME ストリームを取得します。 次の **GetItem** 要求は、アイテムの MIME コンテンツの要求方法を示しています。 
  
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

次の例に、MIME ストリームを取得する要求への応答を示します。MIME ストリームは、読みやすくするために短縮されています。
  
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

アイテムをエクスポートしたら、[アイテムを Exchange にインポート](how-to-import-items-by-using-ews-in-exchange.md)します。
  
## <a name="see-also"></a>関連項目


- [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exchange の EWS を使用してアイテムをインポートする](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    

