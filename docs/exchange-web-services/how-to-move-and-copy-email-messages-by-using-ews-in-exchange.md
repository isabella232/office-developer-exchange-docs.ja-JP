---
title: Exchange において EWS を使用して電子メール メッセージを移動およびコピーする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。
ms.openlocfilehash: 44d5834176b55ad041befbad2230b8b507a12ecc
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353470"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Exchange において EWS を使用して電子メール メッセージを移動およびコピーする

Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。
  
EWS マネージ API または EWS を使用すると、メールボックスの電子メール メッセージを移動およびコピーすることができます。
  
**表 1. 電子メール メッセージを移動およびコピーするための EWS マネージ API メソッドと EWS 操作**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|電子メール メッセージの移動  <br/> |[EmailMessage.Move](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|電子メール メッセージのコピー  <br/> |[EmailMessage.Copy](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
電子メール メッセージを別のフォルダーに移動したりコピーしたりすると、重要なこととして、新しいフォルダーに新しいアイテムが一意のアイテム ID で作成され、元のメッセージが削除されるという点に注意してください。 同じメールボックスにある 2 つのフォルダーで電子メール メッセージを移動またはコピーすると、応答で新しいアイテムが返され、新しいアイテム ID に対するアクセス権が付与されます。 ただし、2 つのメールボックス間で、またはメールボックスとパブリック フォルダー間で電子メール メッセージを移動またはコピーすると、応答で新しいアイテムが返されません。 このシナリオの場合に、移動したメッセージにアクセスするには、EWS マネージ API [FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、[PidTagSearchKey](http://msdn.microsoft.com/ja-JP/library/cc839918.aspx) (0x300B0102) プロパティの[拡張プロパティ定義を作成](properties-and-extended-properties-in-ews-in-exchange.md)するか、カスタムの拡張プロパティを作成および設定し、新しいフォルダーでそのカスタム拡張プロパティを検索します。 
  
電子メール メッセージの削除は、[削除済みアイテム] フォルダーへの移動とは異なります。 EWS マネージ API [Item.Delete](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) メソッドまたは EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用する場合、要求で指定されたアイテムは元のフォルダーから除去されて、新しいアイテム ID で [削除済みアイテム] フォルダーにコピーが配置されます。 アイテムを移動またはコピーする場合とは異なり、新しいアイテムが **Delete** メソッドまたは **DeleteItem** 操作の応答で返されません。 [EWS マネージ API または [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) を使用して電子メールを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma)ための手順は、Exchange ストアから汎用アイテムを削除する手順と同じです。 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを移動する
<a name="bk_moveewsma"> </a>

次のコード例は、[EmailMessage.Move](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) メソッドを使用して既存の電子メール メッセージをフォルダー間で移動する方法を示しています。 
  
この例では、**service** は有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトで、**ItemId** は移動またはコピー対象のメール メッセージの [Id](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) であると想定しています。 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a>EWS を使用して電子メール メッセージを移動する
<a name="bk_moveews"> </a>

次のコード例は、[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) 操作を使用して [迷惑メール] フォルダーに電子メール メッセージを移動する方法を示しています。 
  
これは、[Move](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) メソッドの呼び出し時に EWS マネージ API によって送信される XML 要求でもあります。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
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
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**MoveItem** 要求に [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常に移動されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。またこの応答には、新しいフォルダーにおけるこの電子メール メッセージの **ItemId** も含まれます。新しいフォルダーでは **ItemId** が異なるため、この値を格納することが重要となります。 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージをコピーする
<a name="bk_copyewsma"> </a>

次のコード例は、[EmailMessage.Copy](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) メソッドを使用して既存の電子メール メッセージをフォルダー間でコピーする方法を示しています。 
  
この例では、**service** は有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトで、**ItemId** はコピー対象のメール メッセージの [Id](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) であると想定しています。 読みやすくするため、一部のパラメーターの値が短縮されています。 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a>EWS を使用して電子メール メッセージをコピーする
<a name="bk_copyews"> </a>

次のコード例は、[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) 操作を使用して同じでメールボックスにある別のフォルダーに電子メール メッセージをコピーする方法を示しています。コピーするために、移動する電子メール メッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) を送信し、[ToFolderId](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) 要素で宛先フォルダーを指定しています。 
  
これは、[Copy](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) メソッドの呼び出し時に EWS マネージ API によって送信される XML 要求でもあります。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
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
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**CopyItem** 要求に [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常にコピーされたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。またこの応答には、新しいフォルダーにおけるこの電子メール メッセージの **ItemId** も含まれます。新しいフォルダーでは **ItemId** が異なるため、この値を格納することが重要となります。 
  
## <a name="see-also"></a>関連項目


- [Exchange のメールと EWS](email-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用してメール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

