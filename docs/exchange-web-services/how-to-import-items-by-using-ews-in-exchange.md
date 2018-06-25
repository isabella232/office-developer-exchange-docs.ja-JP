---
title: Exchange EWS を使用してアイテムをインポート
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをインポートする方法について説明します。
ms.openlocfilehash: c09c96eff455b7584b084e71b937853abfde731d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759010"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Exchange EWS を使用してアイテムをインポート

Exchange の EWS マネージ API または EWS を使用して、予定、電子メール、連絡先、タスクなどのアイテムをインポートする方法について説明します。
  
多数のシステムに予定、電子メール、連絡先およびタスクが格納されているときに、それらのアイテムをいくつかの方法で Exchange にインポートできます。Exchange へのアイテムのインポートは、それらのアイテムに対するメールボックスのリレーションシップを維持しない場合は簡単です。EWS マネージ API の [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) メソッドを使用するか、EWS の [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用して、Exchange メールボックスにアイテムを作成します。ただし、この単純なアプローチでは、サポートされないシナリオがあります。次に例を示します。 
  
- 出席者 (会議) によって予定をインポートするときに、開催者と出席者のリレーションシップを維持できません。つまり、開催者と出席者のリレーションシップを確立するには、会議の開催者が会議出席依頼を出席者に再送信する必要があるということです。出席者の予定表にインポートされた予定は、会議の開催者の予定に関連付けられることはありません。出席者は、開催者と出席者のリレーションシップを確立するために、開催者からの会議出席依頼の再送信を受け入れる必要があります。
    
- 割り当て済みのタスクがインポートされるときに、割り当て先に関する情報が保持されません。
    
どのインポート オプションを使用しても、Exchange にアイテムをバッチ インポートできます。
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>アイテムのインポートに EWS マネージ API または EWS のアイテムの種類を使用する
<a name="bk_importproperties"> </a>

EWS マネージ API または EWS を使用して、別のシステムから電子メール、連絡先、予定、またはタスクをインポートできます。インポートする内容に応じて、次のいずれかのオブジェクトにインポート元形式からの[プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)を設定するだけです。 
  
**表 1. EWS マネージ API のオブジェクトと EWS の要素**

|**EWS マネージ API のオブジェクト**|**EWS の要素**|
|:-----|:-----|
|[なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[カレンダー項目](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Task](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[タスク](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
EWS マネージ API の [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) メソッドまたは EWS の [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用して、アイテムのインポートを実行します。このアプローチでは、どのプロパティをインポートするかを制御できるため、別のシステムからアイテムをインポートする場合にお勧めします。アイテムにプロパティを設定して、アイテムを保存する方法の詳細については、「 [EWS マネージ API を使用してアイテムを作成する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma)」または「[EWS を使用してアイテムを作成する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews)」を参照してください。
  
## <a name="import-items-with-full-fidelity"></a>完全な再現性のあるアイテムをインポートする
<a name="bk_importproperties"> </a>

EWS の [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) 操作を使用すると、アイテムをデータ ストリームとしてアップロードできます。このアイテムのデータ ストリーム表現は、 [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) 操作の呼び出しの結果から得る必要があります。EWS マネージ API は **UploadItems** 操作を実装していないため、EWS マネージ API を使用する場合は、Web 要求を送信するルーチンを記述することが必要になります。 
  
これは、別の Exchange サーバーからエクスポートされたアイテムを最も簡単にインポートする方法です。
  
次に示す例では、読みやすくなるように識別子と **Data** 要素の内容が簡略化されています。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

サーバーは **UploadItems** 要求に [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) 要素で応答します。この要素には、アイテムが正常にアップロードされたことを示す [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 要素の値が含まれていてます。この応答には、アップロードしたアイテムのアイテム ID も含まれています。 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>一般的なファイル形式からのインポートに MIME ストリームを使用する
<a name="bk_importproperties"> </a>

EWS では、EML (.eml) ファイルと iCal (.ics) ファイルをインポートできます。独自の MIME コンテンツをテストして、Exchange の MIME パーサーが MIME ストリームのコンテンツを処理する方法を確認してください。MIME ストリームは便利に使用できますが、一般に、[アイテムのインポートに EWS マネージ API または EWS のアイテムの種類を使用する](#bk_importproperties)ほうが優れています。ここには、[vCard をインポートする](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50)方法の例があります。
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>MIME ストリームを使用して EML ファイルから電子メールをインポートするために EWS マネージ API を使用する

次の例は、EML ファイルのコンテンツで [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) プロパティを設定して、電子メールをメールボックスにインポートする方法を示しています。さらに、インポートした電子メールの [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) 拡張プロパティを設定して、メールボックス内で下書きアイテムとして表示されないようにする方法も示しています。この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに対して認証できることを前提としています。 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>MIME ストリームを使用して iCal ファイルから予定をインポートするために EWS マネージ API を使用する

MIME ストリームを使用することで、単純な予定を iCalendar ファイルの形式でインポートできます。会議 (出席者を伴う予定) はインポートできません。これは、開催者と出席者のリレーションシップは、[Exchange 予定表作成](calendars-and-ews-in-exchange.md)ワークフローの一環として設定される必要があるためです。MIME ストリームでは、出席者をキャプチャできません。 
  
次のコード例は、単純な .ics ファイルをユーザーのメールボックスにインポートする方法を示しています。
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a>MIME ストリームを使用してアイテムをインポートするために EWS を使用する

EWS の [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 操作を使用すると、EML アイテムと iCal アイテムは、それぞれの MIME ストリームを使用することでインポートできます。 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="next-steps"></a>次の手順
<a name="bk_importproperties"> </a>

メールボックスにアイテムをインポートしたら、[インポートしたアイテムを保存するためのカスタム フォルダーを作成する](how-to-work-with-folders-by-using-ews-in-exchange.md)ことや、[クライアントとメールボックスのアイテムを同期する](mailbox-synchronization-and-ews-in-exchange.md)ことが必要になります。
  
## <a name="see-also"></a>関連項目


- [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して項目をエクスポートします。](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    

