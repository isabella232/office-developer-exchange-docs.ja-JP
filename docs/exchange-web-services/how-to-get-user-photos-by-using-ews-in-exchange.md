---
title: Exchange で EWS を使用してユーザーの写真を取得する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758987"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Exchange で EWS を使用してユーザーの写真を取得する

Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。
  
顔と名前を並べて配置すると便利です。ユーザーが顔と名前を並べて配置することを望む場合は、アプリケーションから Exchange にある電子メール アカウントを表すイメージ (通常は写真) を要求できます。Exchange サーバーに保存されたメールボックス用のユーザーの写真を取得することも、自分のメールボックスに保存されている連絡先から得た連絡先の写真を取得することもできます。
  
数種のテクノロジを使用して、メールボックスまたは Active Directory ドメイン サービス (AD DS) から写真を取得できます。 写真を取得するための最適な方法は、どの種類の連絡先から写真を取得するかによって異なります。 
  
**表 1. ユーザーの写真を取得するために連絡先の種類に基づいて使用するテクノロジ**

|**連絡先の種類**|**使用するテクノロジ**|
|:-----|:-----|
|メールボックス ユーザーの写真  <br/> |[REST を使用してメールボックス ユーザーの写真を取得する](#bk_REST)<br/><br/> [EWS を使用してユーザーの写真を取得する](#bk_EWS) <br/> |
|連絡先ユーザーの写真  <br/> |[EWS マネージ API を使用して連絡先ユーザーの写真を取得する](#bk_EWSMA)<br/><br/> [EWS を使用してユーザーの写真を取得する](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>REST を使用してメールボックス ユーザーの写真を取得する

標準の HTTPS **GET** 要求を使用することで、Exchange サーバーのユーザーの写真を要求できます。 この要求では、次の例に示すように、電子メール アカウント アドレスとイメージのサイズ コードを指定しています。 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

自動検出サービスの [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) 操作を使用して **ExternalEwsUrl** 設定を取得します。この設定には、Exchange Web サービス (EWS) エンドポイントの URL と、ユーザーの写真を返す **Exchange.asmx** HTTP ハンドラーの場所が含まれています。 
  
それぞれのサイズ コードは、イメージの高さと幅をピクセル単位で示しています。 たとえば、サイズ コード **HR48x48** は、高さ 48 ピクセル × 幅 48 ピクセルのイメージを返します。 サイズ コード パラメーターに有効な値は、[SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) 要素に有効な値と同じになります。 要求で指定したサイズが使用できない場合は、使用可能な最大の写真が返されます。 Exchange サーバーに写真が保存されていない場合は、そのアカウント用に AD DS に保存されているサムネイル イメージが返されます。 
  
> [!NOTE]
> **HR48x48** サイズ コードは、常に AD DS サムネイル イメージを返します (使用可能な場合)。 
  
次の例は、GET 要求を使用して Sadie のユーザー写真を取得して、ローカル コンピューターに保存する方法を示しています。
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

この要求により、HTTP 応答が返されます。 
  
**表 2. GetUserPhoto 要求の応答コード**

|**応答コード**|**説明**|
|:-----|:-----|
|200  <br/> |指定された電子メール アカウントのイメージが使用可能であり、応答にはバイナリ イメージが含まれています。  <br/> |
|304  <br/> |イメージは前回 **ETag** がアプリケーションに返したものから変更されていません。  <br/> |
|404  <br/> |指定された電子メール アカウントに使用可能なイメージがありません。  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>ユーザーの写真をキャッシュする

Exchange は、コンテンツの種類が image/jpeg のデータをヘッダー値のコレクションと共に返します。 **ETag** ヘッダーは、変更キーと同様のものです。 この値は、前回写真が更新されたことを表す文字列です。 **ETag** は、写真が変更されるまでユーザーの写真に対して同じままに保たれます。 この **ETag** 値は、HTTPS **GET** 要求の **If-None-Match** ヘッダーでサーバーに送信できます。 前回の要求以降に写真が変更されていない場合は、それを表す HTTP 304 応答でサーバーが応答します。 そのため、新しいユーザーの写真を処理するのではなく、以前に要求して保存しておいたものを使用できるようになります。 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>EWS マネージ API を使用して連絡先ユーザーの写真を取得する

アプリケーションでは EWS マネージ API を使用して連絡先の写真を取得できます (連絡先がユーザーのメールボックスの連絡先フォルダーに保存されている場合)。 これを行うには、まず、使用する連絡先の **ItemId** を見つけます。 次に、その連絡先にバインドしてから、添付ファイルのコレクションに読み込みます。 連絡先に写真がある場合は、写真が添付ファイルの 1 つに含まれています。 添付ファイルのコレクションをループして、**IsContactPhoto** プロパティの値を確認します。 連絡先の写真を見つけたら、その写真をローカル コンピューターに保存して、アプリケーションからアクセスできるようにします。 
  
次の例は、このプロセスを示しています。 この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<a name="bk_EWS"> </a>

## <a name="get-a-user-photo-by-using-ews"></a>EWS を使用してユーザーの写真を取得する

ユーザーの写真を AD DS から取得するときに、電子メール アドレスがわかっている場合は [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) 操作を使用し、電子メール アドレスがわからない場合は [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作を使用します。 メールボックスの連絡先フォルダーからユーザーの写真を取得する場合は、[GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) 操作に続けて [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) 操作を使用します。 どちらの場合も、写真は Base64 エンコード文字列として XML 応答で返されます。 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>GetUserPhoto 操作を使用してメールボックス ユーザーの写真を取得する

**GetUserPhoto** 操作を使用すると、簡単になります。 XML 要求では、ユーザーの電子メール アドレスと、返される[写真のサイズ](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx)を指定します ([SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) 要素内)。 次の XML 要求の例は、幅 360 ピクセル×高さ 360 ピクセルの Sadie Daniels の写真を取得する方法を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

次に、XML 応答を示します。 Base64 エンコードされた写真が [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) 要素に含まれています (読みやすくするために内容が短縮されています)。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>ResolveNames 操作を使用してメールボックス ユーザーの写真を取得する

写真を取得するユーザーの電子メール アドレスがわからない場合は、[ResolveNames 操作を使用する](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)ことで一致する可能性のある候補を取得できます。 [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) 要素の **ContactDataShape** 属性に "AllProperties" を指定すると、候補ごとに大量のデータ (ユーザーの写真を含む) が返されます。 次の例は、名前 "Sadie" を解決して、候補ごとにプロパティをすべて返す XML 要求を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

この応答では、大量のデータが返されます。 次の例は、ユーザーの写真に関連するデータのみを示しています。 **Photo** 要素には、Base64 エンコードされたユーザーの写真が含まれています (読みやすくするために内容が短縮されています)。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>GetAttachment 操作を使用して連絡先ユーザーの写真を取得する

EWS を使用すると、メールボックスに保存された連絡先から写真を取得できます。 まず、**GetItem** 操作を使用してプロパティをすべて返して、写真を探せるようにします。 次の例は、連絡先アイテムを取得する XML 要求を示しています。 アイテム ID は、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

[HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) 要素を調べて、連絡先に関連付けられた写真があることを確認します。 その後で、添付ファイルのコレクションを 1 つずつ調べて、値が true の [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) 要素を見つけます。 次の応答例は、関連するデータのみを示しています。 ID の値は読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

次に、**AttachmentId** を指定した **GetAttachment** 操作を使用して、連絡先の写真がある添付ファイルを要求します。 次の例は、添付ファイルを取得する XML 要求を示しています。 ID は読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

次の例は、要求した添付ファイルに関する情報を含む XML 応答を示しています。 [Content](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) 要素には、ユーザーの写真の Base64 エンコード文字列が含まれています。読みやすくするために、この例の文字列は短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_EWS"> </a>

## <a name="decode-a-base64-encoded-string"></a>Base64 エンコード文字列をデコードする

どの操作を使用してユーザーの写真を取得したとしても、その文字列をデコードしてアプリケーションで使用できるようにする必要があります。次の例は、文字列をデコードし、ローカル コンピューターに保存して、後からアプリケーションでアクセスできるようにする方法を示しています。
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a>関連項目

- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)    
- [Exchange 2013 の EWS を使用して、あいまいな名前を解決する](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Exchange において EWS を使用してバッチ処理で連絡先を処理する](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

