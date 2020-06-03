---
title: Exchange において EWS を使用して電子メール メッセージを移動およびコピーする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527937"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="00e55-103">Exchange において EWS を使用して電子メール メッセージを移動およびコピーする</span><span class="sxs-lookup"><span data-stu-id="00e55-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="00e55-104">Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="00e55-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="00e55-105">EWS マネージ API または EWS を使用すると、メールボックスの電子メール メッセージを移動およびコピーすることができます。</span><span class="sxs-lookup"><span data-stu-id="00e55-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="00e55-106">**表 1. 電子メール メッセージを移動およびコピーするための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="00e55-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="00e55-107">**タスク**</span><span class="sxs-lookup"><span data-stu-id="00e55-107">**Task**</span></span>|<span data-ttu-id="00e55-108">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="00e55-108">**EWS Managed API method**</span></span>|<span data-ttu-id="00e55-109">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="00e55-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00e55-110">電子メール メッセージの移動</span><span class="sxs-lookup"><span data-stu-id="00e55-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="00e55-111">EmailMessage.Move</span><span class="sxs-lookup"><span data-stu-id="00e55-111">EmailMessage.Move</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="00e55-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="00e55-112">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="00e55-113">電子メール メッセージのコピー</span><span class="sxs-lookup"><span data-stu-id="00e55-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="00e55-114">EmailMessage.Copy</span><span class="sxs-lookup"><span data-stu-id="00e55-114">EmailMessage.Copy</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="00e55-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="00e55-115">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="00e55-116">電子メール メッセージを別のフォルダーに移動したりコピーしたりすると、重要なこととして、新しいフォルダーに新しいアイテムが一意のアイテム ID で作成され、元のメッセージが削除されるという点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="00e55-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="00e55-117">同じメールボックスにある 2 つのフォルダーで電子メール メッセージを移動またはコピーすると、応答で新しいアイテムが返され、新しいアイテム ID に対するアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="00e55-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="00e55-118">ただし、2 つのメールボックス間で、またはメールボックスとパブリック フォルダー間で電子メール メッセージを移動またはコピーすると、応答で新しいアイテムが返されません。</span><span class="sxs-lookup"><span data-stu-id="00e55-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="00e55-119">このシナリオの場合に、移動したメッセージにアクセスするには、EWS マネージ API [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、[PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) プロパティの[拡張プロパティ定義を作成](properties-and-extended-properties-in-ews-in-exchange.md)するか、カスタムの拡張プロパティを作成および設定し、新しいフォルダーでそのカスタム拡張プロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="00e55-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="00e55-120">電子メール メッセージの削除は、[削除済みアイテム] フォルダーへの移動とは異なります。</span><span class="sxs-lookup"><span data-stu-id="00e55-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="00e55-121">EWS マネージ API [Item.Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) メソッドまたは EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用する場合、要求で指定されたアイテムは元のフォルダーから除去されて、新しいアイテム ID で [削除済みアイテム] フォルダーにコピーが配置されます。</span><span class="sxs-lookup"><span data-stu-id="00e55-121">If you use the EWS Managed API [Item.Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="00e55-122">アイテムを移動またはコピーする場合とは異なり、新しいアイテムが **Delete** メソッドまたは **DeleteItem** 操作の応答で返されません。</span><span class="sxs-lookup"><span data-stu-id="00e55-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="00e55-123">[EWS マネージ API または [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) を使用して電子メールを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma)ための手順は、Exchange ストアから汎用アイテムを削除する手順と同じです。</span><span class="sxs-lookup"><span data-stu-id="00e55-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="00e55-124">EWS マネージ API を使用して電子メール メッセージを移動する</span><span class="sxs-lookup"><span data-stu-id="00e55-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="00e55-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="00e55-125"><a name="bk_moveewsma"> </a></span></span>

<span data-ttu-id="00e55-126">次のコード例は、[EmailMessage.Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) メソッドを使用して既存の電子メール メッセージをフォルダー間で移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-126">The following code example shows how to use the [EmailMessage.Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="00e55-127">この例では、**service** は有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトで、**ItemId** は移動またはコピー対象のメール メッセージの [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) であると想定しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-127">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
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

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="00e55-128">EWS を使用して電子メール メッセージを移動する</span><span class="sxs-lookup"><span data-stu-id="00e55-128">Move an email message by using EWS</span></span>
<span data-ttu-id="00e55-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="00e55-129"><a name="bk_moveews"> </a></span></span>

<span data-ttu-id="00e55-130">次のコード例は、[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) 操作を使用して [迷惑メール] フォルダーに電子メール メッセージを移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-130">The following code example shows how to use the [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="00e55-131">これは、[Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) メソッドの呼び出し時に EWS マネージ API によって送信される XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="00e55-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="00e55-132">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="00e55-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="00e55-p104">サーバーは、**MoveItem** 要求に [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常に移動されたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。またこの応答には、新しいフォルダーにおけるこの電子メール メッセージの **ItemId** も含まれます。新しいフォルダーでは **ItemId** が異なるため、この値を格納することが重要となります。</span><span class="sxs-lookup"><span data-stu-id="00e55-p104">The server responds to the **MoveItem** request with a [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully. The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="00e55-135">EWS マネージ API を使用して電子メール メッセージをコピーする</span><span class="sxs-lookup"><span data-stu-id="00e55-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="00e55-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="00e55-136"><a name="bk_copyewsma"> </a></span></span>

<span data-ttu-id="00e55-137">次のコード例は、[EmailMessage.Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) メソッドを使用して既存の電子メール メッセージをフォルダー間でコピーする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-137">The following code example shows how to use the [EmailMessage.Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="00e55-138">この例では、**service** は有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトで、**ItemId** はコピー対象のメール メッセージの [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) であると想定しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-138">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="00e55-139">読みやすくするため、一部のパラメーターの値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="00e55-139">The values of some parameters have been shortened for readability.</span></span> 
  
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

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="00e55-140">EWS を使用して電子メール メッセージをコピーする</span><span class="sxs-lookup"><span data-stu-id="00e55-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="00e55-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="00e55-141"><a name="bk_copyews"> </a></span></span>

<span data-ttu-id="00e55-142">次のコード例は、[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) 操作を使用して同じでメールボックスにある別のフォルダーに電子メール メッセージをコピーする方法を示しています。コピーするために、移動する電子メール メッセージの [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) を送信し、[ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) 要素で宛先フォルダーを指定しています。</span><span class="sxs-lookup"><span data-stu-id="00e55-142">The following code example shows how to use the [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="00e55-143">これは、[Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) メソッドの呼び出し時に EWS マネージ API によって送信される XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="00e55-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="00e55-144">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="00e55-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="00e55-p107">サーバーは、**CopyItem** 要求に [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常にコピーされたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれます。またこの応答には、新しいフォルダーにおけるこの電子メール メッセージの **ItemId** も含まれます。新しいフォルダーでは **ItemId** が異なるため、この値を格納することが重要となります。</span><span class="sxs-lookup"><span data-stu-id="00e55-p107">The server responds to the **CopyItem** request with a [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully. The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="00e55-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="00e55-147">See also</span></span>


- [<span data-ttu-id="00e55-148">Exchange のメールと EWS</span><span class="sxs-lookup"><span data-stu-id="00e55-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="00e55-149">Exchange で EWS を使用してメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="00e55-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

