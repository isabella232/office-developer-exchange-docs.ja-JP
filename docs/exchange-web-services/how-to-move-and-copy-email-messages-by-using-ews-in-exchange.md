---
title: 移動し、EWS を使用して Exchange が電子メール メッセージをコピー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。
ms.openlocfilehash: 16f0604a16785c34dd04bdabedeedd331668a479
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759024"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>移動し、EWS を使用して Exchange が電子メール メッセージをコピー

Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。
  
EWS マネージ API または EWS を使用すると、メールボックスの電子メール メッセージを移動およびコピーすることができます。
  
**表 1 です。EWS のマネージ API のメソッドと移動し、電子メール メッセージのコピーの EWS の操作**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|電子メール メッセージの移動  <br/> |[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|電子メール メッセージのコピー  <br/> |[EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
移動したり、電子メール メッセージを別のフォルダーにコピーすると、一意の項目の ID を持つ新しいフォルダーに新しい項目を作成し、元のメッセージの削除を確認する必要があります。 応答を使用する新しいアイテムの ID にアクセスする新しいアイテムが返された場合の移動や同じメールボックスに 2 つのフォルダー間で電子メール メッセージをコピー、 ただし場合の移動や 2 つのメールボックスまたはメールボックスとパブリック フォルダーの間で電子メール メッセージをコピー、新しいアイテムが応答として返されません。 メッセージにアクセスする、移動したこのシナリオでは、マネージ API の EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)メソッドまたは EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作、 [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102) プロパティでは、[拡張プロパティの定義を作成](properties-and-extended-properties-in-ews-in-exchange.md)を使用または作成し、設定、プロパティは、新しいフォルダーにユーザー設定の拡張プロパティを検索し、ユーザー設定が拡張されます。 
  
電子メール メッセージを削除することは、削除済みアイテム フォルダーにアイテムを移動すると異なっています。 EWS のマネージ API の[Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx)メソッドまたは EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)操作を使用する場合は、要求で指定されたアイテムは、元のフォルダーから削除し、コピーは、新しい項目の ID を使用して削除済みアイテム フォルダーに格納されます。 移動またはコピーする任意の項目とは異なり、 **Delete**メソッドまたは**DeleteItem**操作の応答に、新しいアイテムは返されません。 に関する手順は[、EWS のマネージ API を使用して電子メールを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma)か、 [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews)は、Exchange ストアから任意の汎用的な項目を削除するのと同じです。 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを移動する
<a name="bk_moveewsma"> </a>

次のコード例では、既存の電子メール メッセージを別の 1 つのフォルダーに移動する[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。 
  
次の使用例は、**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと、その**アイテム Id**では、 [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx)電子メール メッセージの移動またはコピーすることを想定しています。 
  
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

[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)操作を使用して、電子メール メッセージを [迷惑メール フォルダーに移動するのには次のコード例を次に示します。 
  
これは、 [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx)メソッドを呼び出すときに、EWS のマネージ API によって送信される XML の要求。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
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

サーバーは、 **MoveItem**要求[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、電子メール メッセージが正常に移動されたことを示す値を含む[MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx)メッセージに応答します。 応答には、[新しいフォルダーの新しいフォルダーに**アイテム Id**が異なるために保管する必要が電子メール メッセージの**アイテム Id**も含まれています。 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージをコピーする
<a name="bk_copyewsma"> </a>

次のコード例では、1 つのフォルダーから既存の電子メール メッセージをコピーするには、 [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。 
  
次の使用例は、**サービス**は、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトの有効なその**アイテム Id**は、コピーするのには電子メール メッセージの[Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx)を想定しています。 いくつかのパラメーターの値は、読みやすくするために短縮されています。 
  
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

コード例を次の電子メール メッセージを移動するには、[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を送信して、 [ToFolderId のインストール先フォルダーを指定することによって、同じメールボックスに別のフォルダーに電子メール メッセージをコピーするのには、 [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx)操作を使用する方法を示しています。](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)要素です。 
  
[Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx)メソッドを呼び出すときに、EWS のマネージ API によって送信される XML の要求にもです。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
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

サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、電子メール メッセージが正常にコピーされたことを示す値を含む[CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx)メッセージで**CopyItem**要求に応答します。 応答には、[新しいフォルダーの新しいフォルダーに**アイテム Id**が異なるために保管する必要が電子メール メッセージの**アイテム Id**も含まれています。 
  
## <a name="see-also"></a>関連項目


- [Exchange の電子メールと EWS](email-and-ews-in-exchange.md)
    
- [EWS を使用して Exchange が電子メール メッセージを送信します。](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

