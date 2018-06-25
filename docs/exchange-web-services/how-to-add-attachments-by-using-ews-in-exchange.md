---
title: Exchange EWS を使用して添付ファイルを追加します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0cbce436-2ae6-4fcc-bd8b-f517a0724e55
description: EWS マネージ API または Exchange の EWS を使用して、添付物を伴う新しくアイテムを作成するか、既存のアイテムに添付物を追加する方法について説明します。
ms.openlocfilehash: dbfff879c92dafeec588d79cddd92e294b763c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758947"
---
# <a name="add-attachments-by-using-ews-in-exchange"></a>Exchange EWS を使用して添付ファイルを追加します。

EWS マネージ API または Exchange の EWS を使用して、添付物を伴う新しくアイテムを作成するか、既存のアイテムに添付物を追加する方法について説明します。
  
EWS マネージ API または EWS を使用して、新規アイテムまたは既存のアイテムに、ファイル添付またはアイテム添付を追加できます。EWS マネージ API を使用している場合は、同じメソッドで新規アイテムまたは既存のアイテムに添付物を追加できますが、ファイル添付またはアイテム添付を使用している場合はメソッドが変わります。一方、EWS を使用している場合は、同じ操作でファイル添付またはアイテム添付をアイテムに追加できますが、新規または既存のアイテムに添付物を追加する場合は操作が変わります。
  
**表 1. 添付物を追加するためのEWS マネージ API とEWS の操作**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|新規または既存の電子メールにファイル添付を追加する  <br/> |[AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) <br/> |新しい電子メールは、 [createitem メソッド](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)  <br/> [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)を既存の電子メールに追加するには  <br/> |
|新規または既存の電子メールにアイテム添付を追加する  <br/> |[AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/en-us/library/dd634986%28v=exchg.80%29.aspx) <br/> |新しい電子メールは、 [createitem メソッド](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)  <br/> [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)を既存の電子メールに追加するには  <br/> |
   
## <a name="create-an-email-with-file-and-item-attachments-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、ファイル添付およびアイテム添付のある電子メールを作成する
<a name="bk_createattachewsma"> </a>

次のコード例は、複数のファイル添付とアイテム添付のある電子メールを作成する方法を示しています。  
  
1. [なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトを使用して、電子メール メッセージを作成します。 
    
2. メッセージに添付ファイルを追加するのには、 [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx)メソッドと[AttachmentCollection.AddItemAttachment](http://msdn.microsoft.com/en-us/library/dd634986%28v=exchg.80%29.aspx)メソッドを使用します。 
    
3. [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)メソッドを使用して、受信者にメッセージを送信し、メッセージを送信済みアイテム フォルダーに保存します。 
    
このコード例は、EWS マネージ API を使用してファイル添付をアイテムに追加できる 4 つの方法を示しています。
  
- 完全修飾ファイルの場所を使用します。
    
- 完全修飾ファイルの場所と新しい添付名を使用します。
    
- バイト配列を使用します。
    
- ストリームを使用します。
    
この例ではアイテムの添付ファイルが電子メール メッセージと同時に作成されたことに注意してください。 アイテムの添付ファイルとして既存の電子メール メッセージを追加するには、 [MimeContent と EWS のマネージ API を使用して新しいメール アドレスに既存の項目の追加](#bk_addexistingemailewsma)を参照してください。
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="create-an-email-with-file-and-item-attachments-by-using-ews"></a>EWS を使用して、ファイル添付およびアイテム添付のある電子メールを作成する
<a name="bk_createattachews"> </a>

次のコード例は、 [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用して、4 つのファイルの添付ファイルと 1 つのアイテムの添付ファイルを電子メール メッセージを作成する方法を示しています。 これも EWS のマネージ API に送信する場合、XML 要求のいずれかの[ファイルおよびアイテムの添付ファイル付き電子メールを作成](#bk_createattachewsma)します。
  
この例ではアイテムの添付ファイルが電子メール メッセージと同時に作成されたことに注意してください。 アイテムの添付ファイルとして既存の電子メール メッセージを追加するには、 [MimeContent と EWS のマネージ API を使用して新しいメール アドレスに既存の項目の追加](#bk_addexistingemailewsma)を参照してください。
  
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

サーバーは、 **CreateItem**要求[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**電子メールと添付ファイルが正常に作成されたことを示す値を含む[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。 新しく作成されたメッセージと添付ファイルの[AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx)値の[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)は、応答にも含まれます。 いくつかの属性の値は、読みやすくするために短縮されています。 
  
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

[このメッセージを新しく作成した送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を、 [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx)操作を呼び出します。 
  
## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-the-ews-managed-api"></a>MimeContent および EWS マネージ API を使用して、既存アイテムを新しい電子メールに追加する
<a name="bk_addexistingemailewsma"> </a>

既存のアイテムをアイテム添付として別のアイテムに追加するには、新しいアイテム添付を作成し、既存のアイテムの内容をその新しいアイテムにコピーする必要があります。これを実行するには、次の 2 つの方法があります。  
  
1. 電子メール メッセージを具体的に作業している場合は、新しく作成されたアイテムの添付ファイルに電子メールから[MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx)プロパティの値をコピーできます。 フォロー アップ フラグおよびカテゴリでは、このプロセス中にいくつかのプロパティが失われますが、標準の電子メール メッセージをうまきます。 
    
2. すべての種類のアイテムに完全な再現性が必要な場合は、既存のアイテムにバインドし、すべてのプロパティと拡張プロパティを新しい添付物にコピーできます。
    
次のコード例は、 **MimeContent**を新しいアイテムの添付ファイルにコピー、最初の方法を示しています。 2 番目のアプローチを使用するコードを変更する方法を示す手順は、以下の例です。 
  
この例ではその**サービス**が有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと Exchange サーバーに、ユーザーが認証されていると**アイテム Id**は、添付するアイテムの[アイテム Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)をします。 
  
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

この例を変更して、既存アイテムの各プロパティを新しいアイテム添付にコピーするには、次の操作を行います。  
  
1. **PropertySet.FirstClassProperties**およびその他のプロパティやする必要がある拡張のプロパティを含むように設定するプロパティを変更します。 
    
  ```cs
  // Add additional properties to the PropertySet.
  EmailMessage msgToAttach = EmailMessage.Bind(service, itemId, new PropertySet(PropertySet.FirstClassProperties));
  ```

2. **MimeContent**プロパティを必要としないために、次の行を削除します。 
    
  ```cs
  itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
  ```

3. 既存のアイテムから新しい添付ファイルにコピーするには、各プロパティについては、この行を繰り返します。 読み取り専用プロパティであるために、新しいアイテムの添付ファイルに**アイテム Id**をコピーしないでください。 
    
  ```cs
  itemAttachment.Item.Subject = msgToAttach.Subject;
  ```

4. **送信済みアイテム**に添付ファイルの[PidTagMessageFlags](http://msdn.microsoft.com/en-us/library/cc839733.aspx) (0x0E070003) のプロパティを設定します。
    
  ```cs
  ExtendedPropertyDefinition sent = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
  msgToAttach.Item.SetExtendedProperty(sent, "1");
  ```

## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-ews"></a>MimeContent および EWS を使用して、既存アイテムを新しい電子メールに追加する
<a name="bk_addexistingemailews"> </a>

既存のアイテムを新しいアイテムに追加するには、2 つの方法があります。  
  
1. 電子メール メッセージを具体的に作業している場合は、新しく作成されたアイテムの添付ファイルに電子メールから[MimeContent](http://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx)要素の値をコピーできます。 フォロー アップ フラグおよびカテゴリでは、このプロセス中にいくつかのプロパティが失われますが、標準の電子メール メッセージをうまきます。 
    
2. すべての種類のアイテムに完全な再現性が必要な場合は、既存のアイテムにバインドし、すべてのプロパティと拡張プロパティを新しい添付物にコピーできます。
    
**MimeContent**要素を使用して、新しいアイテムの添付ファイルの**MimeContent**値に元のアイテムのコンテンツをコピーする方法を次のコード例に示します。 例では、次の操作を使用します。 
  
1. [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) : **MimeContent**と新しいメッセージのアイテムの添付ファイルとなるメッセージの[件名](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)を取得します。 
    
2. [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) : 新しい電子メール メッセージを作成します。 
    
3. [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)- **GetItem**操作によって新しい添付ファイルを作成するには、 **MimeContent**と**件名**を使用して取得します。 
    
4. [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) -を送信し、メッセージを保存します。 
    
**MimeContent**と既存のアイテムの**件名**を取得することによって、例を開始します。 
  
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

サーバー要求に応答し、 **GetItem** **NoError**メールが正常に取得されたことを示す、および**MimeContent**と**の[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)の値が含まれています[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx)メッセージ件名**電子メールの。 
  
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

次に、新しい電子メールを作成するのには、 **CreateItem**操作を呼び出します。 
  
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

サーバーは、 **CreateItem**要求[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**電子メールが正常に作成されたことを示す値を含む[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。
  
**MimeContent** **GetItem**操作によって取得された**件名**を使用して次に、新しいアイテムの添付ファイルを作成します。 [ParentItemId](http://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx)要素の値は、 **createitem メソッド**の応答で返された**アイテム Id**の値を使用して設定されます。 
  
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

サーバー要求に応答し、 **CreateAttachment** **NoError**、添付ファイルが正常に作成されたことを示す、および、[の[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)の値が含まれています[CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx)メッセージAttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx)の新しく作成された添付ファイルです。 
  
新しいメッセージが作成され、アイテムの添付、[送信](how-to-send-email-messages-by-using-ews-in-exchange.md)するこのメッセージを新しく作成された[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx)操作を呼び出すことによって。 
  
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

サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**メールが正常に送信されたことを示す値を含む[SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx)メッセージが**SendItem**要求に応答します。
  
## <a name="create-an-email-with-an-inline-attachment-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、インライン添付のある電子メールを作成する
<a name="bk_createinlineattachewsma"> </a>

次のコード例は、インライン添付のある電子メールを作成する方法を示しています。
  
1. [なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)オブジェクトを使用して、電子メール メッセージを作成します。 
    
2. インライン添付ファイルを含む HTML の本文に[EmailMessage.Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)プロパティを設定します。 
    
3. [AttachmentCollection.AddFileAttachment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx)メソッドを使用して、メッセージに添付ファイルを追加します。 
    
4. [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)メソッドを使用して、受信者にメッセージを送信し、メッセージを送信済みアイテム フォルダーに保存します。 
    
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="create-an-email-with-an-inline-attachment-by-using-ews"></a>EWS を使用して、インライン添付のある電子メールを作成する
<a name="bk_createinlineattachewsma"> </a>

次のコード例は、 [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用して、インライン ファイルの添付ファイル付き電子メール メッセージを作成する方法を示しています。 [Body](http://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx)要素の**BodyType**属性では、コンテンツは HTML 形式でされ、イメージ ソースが含まれて ことを示します。 これは、EWS のマネージ API が[インライン添付ファイル付き電子メールを作成](#bk_createinlineattachewsma)するのには EWS のマネージ API を使用するときに送信される XML 要求の 1 つ。
  
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

サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
[このメッセージを新しく作成した送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を、 [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx)操作を呼び出します。 
  
## <a name="add-an-attachment-to-an-existing-email-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、添付物を既存の電子メールに追加する
<a name="bk_createinlineattachewsma"> </a>

次のコード例は、既存の電子メールに添付物を追加する方法を示しています。  
  
1. [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを使用して、既存の電子メール メッセージにバインドします。 
    
2. **AddFileAttachment**メソッドを使用してメッセージに添付ファイルを追加します。 
    
3. [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)メソッドを呼び出すことによって、更新プログラムを保存しています。 
    
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="add-an-attachment-to-an-existing-email-by-using-ews"></a>EWS を使用して、添付物を既存の電子メールに追加する
<a name="bk_createinlineattachewsma"> </a>

[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)操作を使用して、既存の電子メール メッセージに添付ファイルを追加するのには次のコード例を次に示します。 これは、EWS のマネージ API は、[既存の電子メールの添付ファイルを追加](#bk_createinlineattachewsma)するのには EWS のマネージ API を使用する場合を送信する XML 要求の 1 つ。
  
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

サーバー要求に応答し、 **CreateAttachment** **NoError**、添付ファイルが正常に作成されたことを示す、および、[の[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)の値が含まれています[CreateAttachmentResponse](http://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx)メッセージAttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx)の新しく作成された添付ファイルです。 
  
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

## <a name="see-also"></a>関連項目


- [Exchange の添付物と EWS](attachments-and-ews-in-exchange.md)
    
- [Exchange EWS を使用して添付ファイルを追加します。](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して添付ファイルを削除します。](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して添付ファイルを取得します。](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange が電子メール メッセージを送信します。](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

