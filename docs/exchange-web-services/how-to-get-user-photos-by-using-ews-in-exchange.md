---
title: EWS を使用して Exchange でのユーザーの写真を取り込み
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758987"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>EWS を使用して Exchange でのユーザーの写真を取り込み

Exchange の EWS マネージ API または EWS を使用して、メールボックスまたは連絡先に関連付けられているユーザーの写真を取得する方法について説明します。
  
顔と名前を並べて配置すると便利です。ユーザーが顔と名前を並べて配置することを望む場合は、アプリケーションから Exchange にある電子メール アカウントを表すイメージ (通常は写真) を要求できます。Exchange サーバーに保存されたメールボックス用のユーザーの写真を取得することも、自分のメールボックスに保存されている連絡先から得た連絡先の写真を取得することもできます。
  
さまざまなテクノロジを使用すると、メールボックスまたは Active Directory ドメイン サービス (AD DS) から写真を取得します。 写真を取得する最良の方法から写真を取得する連絡先の種類によって異なります。 
  
**表 1 です。テクノロジを使用して連絡先の種類に基づいて、ユーザーの写真を取得するには**

|**連絡先の種類**|**テクノロジを使用するには**|
|:-----|:-----|
|メールボックス ユーザーの写真  <br/> |[残りの部分を使用してメールボックスのユーザーの写真を取得します。](#bk_REST)<br/><br/> [EWS を使用してユーザーの写真を取得します。](#bk_EWS) <br/> |
|連絡先ユーザーの写真  <br/> |[EWS のマネージ API を使用してユーザーの連絡先の写真を取得します。](#bk_EWSMA)<br/><br/> [EWS を使用してユーザーの写真を取得します。](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>REST を使用してメールボックス ユーザーの写真を取得する

標準的な**取得**を HTTPS 要求を使用して Exchange サーバーからユーザーの写真を要求できます。 次の例に示すように、依頼の電子メール アカウントのアドレスと、イメージのサイズのコードを指定します。 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

自動検出サービスの[GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)操作を使用して、Exchange Web サービス (EWS) のエンドポイントの URL と**Exchange.asmx** HTTP ハンドラーを表すオブジェクトの場所を含む**ExternalEwsUrl**の設定を取得するために、ユーザーの写真です。 
  
各サイズのコードは、ピクセル単位でイメージの幅と高さを示します。 サイズ コード**HR48x48**は、高さ 48 ピクセル、幅 48 ピクセルであるイメージを返します。 サイズ ・ コード ・ パラメーターの値は、 [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx)要素の値と同じです。 要求では、無効なサイズを指定する場合は、最大の使用可能な写真が返されます。 Exchange サーバー上の写真が格納されていない場合、は、アカウントを AD DS に格納されているサムネイル イメージが返されます。 
  
> [!NOTE]
> **HR48x48**サイズのコードは、使用可能である場合、AD DS の縮小版イメージを常に返します。 
  
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
  
**表 2 になります。GetUserPhoto 要求の応答コード**

|**応答コード**|**説明**|
|:-----|:-----|
|200  <br/> |指定された電子メール アカウントのイメージが使用可能であり、応答にはバイナリ イメージが含まれています。  <br/> |
|304  <br/> |**ETag**は、アプリケーションに返された最後の時間以降は、イメージは変更されていません。  <br/> |
|404  <br/> |指定された電子メール アカウントに使用可能なイメージがありません。  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>キャッシュのユーザーの写真

Exchange では、コンテンツ タイプ ヘッダー値のコレクションとは、イメージと jpeg のデータを返します。 **ETag**ヘッダーは、キーの変更に似ています。 値は、写真が更新された最終時刻を表す文字列です。 写真が変更されるまで、ユーザーの写真を同じ**ETag**のままです。 この**ETag**値は、HTTPS **GET**要求**なしに If-match**ヘッダー内のサーバーに送信できます。 写真が前回の要求以降変更されていない場合、HTTP 304 応答を示すようにサーバの応答がします。 以前を要求し、保存したユーザーの写真を使用することができますこれは、新しい 1 つを処理する代わりにします。 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>EWS マネージ API を使用して連絡先ユーザーの写真を取得する 

アプリケーションは、ユーザーのメールボックスの連絡先フォルダーに連絡先が保存されている場合、連絡先の写真を取得するために、EWS のマネージ API を使用できます。 **ItemId**を最初に、これを行うには、検索、連絡先に使用します。 その連絡先にバインドすると後、は、添付ファイルのコレクションに読み込みます。 連絡先に写真がある場合、添付ファイルのいずれかを写真になります。 **IsContactPhoto**プロパティの値を確認、添付ファイルのコレクションをループします。 連絡先の写真を検索するときに、ローカル コンピューターに保存することができ、アプリケーションがアクセスできます。 
  
次の使用例は、このプロセスを示しています。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="get-a-user-photo-by-using-ews"></a>EWS を使用してユーザーの写真を取得します。

AD DS からユーザーの写真がある場合、(e メール アドレスがわからない) 場合、 [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx)操作 (電子メール アドレスを知っている) 場合や、 [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx)操作を使用できます。 メールボックスの連絡先フォルダーからユーザーの写真がある場合、 [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)操作の後に、 [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx)操作を使用します。 どちらの場合も、写真は XML 応答に Base64 でエンコードされた文字列として返されます。 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>GetUserPhoto 操作を使用してメールボックス ユーザーの写真を取得する

**GetUserPhoto**操作を使用することは簡単です。 XML 要求に、ユーザー、および[写真のサイズ](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx)( [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx)要素) で取得するの電子メール アドレスを指定します。 Sadie Daniels が 360 ピクセル、高さ、幅が 360 ピクセルの写真を取得するのには次の XML 要求の例を次に示します。 
  
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

XML 応答は、次のようにします。 [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx)要素 (コンテンツが小さすぎると読みやすさ優先) で、Base64 でエンコードされた写真が含まれています。 
  
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

写真を取得するユーザーの電子メール アドレスがわからない場合は[ResolveNames オペレーションを使用](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)可能な一致の候補を取得することができます。 [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx)要素の**ContactDataShape**属性の"AllProperties"を指定すると、各候補者への多くのユーザーの写真を含む、データが返されます。 "Sadie"の名前を解決し、各候補者へのすべてのプロパティを返す XML 要求の例を次に示します。 
  
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

応答には、大量のデータが表示されます。 次の例では、ユーザーの写真に関連するデータのみを示します。 **写真**の要素には、Base64 でエンコードされたユーザーの写真 (コンテンツが小さすぎると読みやすさ優先) にはが含まれています。 
  
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

EWS を使用すると、メールボックスに格納されている連絡先から写真を取得します。 まず、 **GetItem**操作を使用して、写真のようにすべてのプロパティを取得します。 連絡先アイテムを取得するのには、XML 要求の例を次に示します。 品目 ID が小さすぎると読みやすくするためです。 
  
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

連絡先に関連付けられている写真があることを確認するのには[HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx)要素を検索します。 [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx)要素の true の値を持つ 1 つの添付ファイルのコレクションを検索します。 次の応答の例は、関連データのみを示します。 ID の値は、読みやすさに短縮されます。 
  
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

次に、連絡先の写真を添付ファイルを要求するのに**AttachmentId**と**GetAttachment**操作を使用します。 次の使用例は、添付ファイルを取得するのには XML の要求を示しています。 ID は、読みやすくするために短縮されます。 
  
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

要求した添付ファイルに関する情報を使用して XML 応答の例を次に示します。 [コンテンツ](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx)要素には、短く読みやすくするためには、この例では、ユーザーの写真を Base64 でエンコードされた文字列が含まれています。 
  
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

## <a name="decode-a-base64-encoded-string"></a>Base64 でエンコードされた文字列をデコードします。

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
- [Exchange 2013 の EWS を使用してあいまいな名前を解決するには](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Exchange EWS を使用してバッチ プロセスの連絡先](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

