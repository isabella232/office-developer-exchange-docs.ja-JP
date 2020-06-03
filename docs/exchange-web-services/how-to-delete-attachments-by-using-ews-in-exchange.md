---
title: Exchange で EWS を使用して添付物を削除する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Exchange で EWS マネージ API または EWS を使用して、EWS アイテムから添付物を削除する方法について説明します。
ms.openlocfilehash: 854f723e9c7452b955d0e7d7a38da7f6224dc8b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455892"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a>Exchange で EWS を使用して添付物を削除する

Exchange で EWS マネージ API または EWS を使用して、EWS アイテムから添付物を削除する方法について説明します。
  
EWS マネージ API を使用して、アイテムからファイルおよびアイテム添付を削除する場合、いくつかのオプションがあります。 メッセージからすべての添付物を削除して、ファイル名による削除やコレクション内の位置による削除を行うことができます。 これらのオプションそれぞれについて、[AttachmentCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) メソッドがあります。 
  
一方、EWS を使用して、アイテムからすべての添付物を削除する場合も、1 つだけ削除する場合も、一連の操作は同じです。EWS マネージ API とは異なり、EWS には添付物の配列内の名前または位置に基づいて削除するための別の操作はありません。
  
**表 1. 添付物を削除するための EWS マネージ API メソッドと EWS 操作**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|アイテムからすべての添付物を削除します。  <br/> |[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、その後に [AttachmentCollection.Clear](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx)、その後に [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)、その後に [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
|名前でアイテムから添付物を削除します。  <br/> |[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、その後に [AttachmentCollection.Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx)、その後に [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)、その後に [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
|コレクション内の位置でアイテムから添付物を削除します。  <br/> |[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、その後に [AttachmentCollection.RemoveAt](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx)、その後に [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)、その後に [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、電子メールからすべての添付物を削除する
<a name="bk_deleteattachewsma"> </a>

次のコード例は、電子メールから添付物をすべて削除する方法を示しています。
  
1. [EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) メソッドを使用して、既存の電子メール メッセージにバインドし、[Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) のコレクションを取得します。
    
2. [AttachmentCollection.Clear](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) メソッドを使用して、電子メールからすべての添付物を削除します。 
    
3. [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) メソッドを使用して、変更を保存します。 
    
この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、**itemId** が添付物を削除するメッセージの [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) であり、ユーザーが Exchange Server に認証されたと想定しています。 
  
```cs
public static void DeleteAllAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Delete all attachments from the message.
    message.Attachments.Clear();
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、電子メールから名前ですべての添付物を削除する
<a name="bk_deleteattachewsma"> </a>

次のコード例では、名前で添付物を削除する方法を示しています。
  
1. [EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) メソッドを使用して、既存の電子メール メッセージにバインドし、[Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) のコレクションを取得します。
    
2. [AttachmentCollection.Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) メソッドを使用して、FileAttachment.txt という名前の添付物を削除します。 
    
3. [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) メソッドを使用して、変更を保存します。 
    
この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、**itemId** が添付物を削除するメッセージの [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) であり、ユーザーが Exchange Server に認証されたと想定しています。 
  
```cs
public static void DeleteNamedAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and delete the attachment named "FileAttachment.txt," if it exists.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment.Name == "FileAttachment.txt")
        {
            message.Attachments.Remove(attachment);
            break;
        }
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して位置で添付物を削除する
<a name="bk_deleteattachewsma"> </a>

次のコード例は、添付物を位置で削除する方法を示しています。
  
1. [EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) メソッドを使用して、既存の電子メール メッセージにバインドし、[Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) のコレクションと [EmailMessage.HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) プロパティを取得します。 
    
2. [AttachmentCollection.Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) メソッドを使用して、コレクションの最初の添付物を削除します。 
    
3. [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) メソッドを使用して、変更を保存します。 
    
この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、**itemId** が添付物を削除するメッセージの [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) であり、ユーザーが Exchange Server に認証されたと想定しています。 
  
```cs
public static void DeleteAttachmentByPosition(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting the HasAttachments property and the attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(EmailMessageSchema.HasAttachments, ItemSchema.Attachments));
    // Remove attachments using the zero-based index position of the attachment in the attachments collection.
    if (message.HasAttachments)
    {
        message.Attachments.RemoveAt(0);
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-from-an-item-by-using-ews"></a>EWS を使用してアイテムから添付物を削除する
<a name="bk_deleteattachewsma"> </a>

EWS を使用して添付物を削除するには、最初にメッセージと添付物のコレクションを取得して、削除する添付物の [AttachmentId (GetAttachment と DeleteAttachment)](https://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) を取得します。 削除する 1 つ以上の **AttachmentId** の値を指定してから、[DeleteAttachment](https://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) 操作を呼び出して指定された添付物をメッセージから削除します。 
  
次のコード例は、[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して電子メール メッセージとメッセージの添付物のコレクションを取得する方法を示しています。これは、EWS マネージ API を使用して[電子メールからすべての添付物を削除する](#bk_deleteattachewsma)ときに EWS マネージ API が送信する最初の XML 要求でもあります。読みやすくするため、一部の属性の値が短縮されています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
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
        <t:ItemId Id="uqE1AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、 **GetItem** 要求に [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode ** 値 、および既存の添付物の [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) が含まれます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="uqE1AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="IpHLObE=" />
                  <t:Name>FileAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="QuHSSmY=" />
                  <t:Name>SecondAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="qf2KoPo=" />
                  <t:Name>ThirdAttachment.jpg</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="NFQMnMc=" />
                  <t:Name>FourthAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="jJvbLXQ=" />
                  <t:Name>Attached Message Item</t:Name>
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

どの添付物を削除するか判別し、[DeleteAttachment](https://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) 操作を呼び出し、削除する添付物の **AttachmentId** 値を含めます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="IpHLObE=" />
        <t:AttachmentId Id="QuHSSmY=" />
        <t:AttachmentId Id="qf2KoPo=" />
        <t:AttachmentId Id="NFQMnMc=" />
        <t:AttachmentId Id="jJvbLXQ=" />
      </m:AttachmentIds>
    </m:DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**DeleteAttachment** 要求に [DeleteAttachmentResponse](https://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx) メッセージで応答します。このメッセージには、それぞれの添付物が正常に削除されたことを示す、[DeleteAttachmentResponseMessage](https://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx) ごとの **NoError** の [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) 値が含まれます。 読みやすくするため、一部の属性の値が短縮されています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:DeleteAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>関連項目


- [Exchange における添付物と EWS](attachments-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用して添付物を追加する](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して添付物を取得する](how-to-get-attachments-by-using-ews-in-exchange.md)
    

