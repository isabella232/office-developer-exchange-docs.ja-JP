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
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="95968-103">移動し、EWS を使用して Exchange が電子メール メッセージをコピー</span><span class="sxs-lookup"><span data-stu-id="95968-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="95968-104">Exchange で EWS マネージ API または EWS を使用して電子メール メッセージを移動およびコピーする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="95968-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="95968-105">EWS マネージ API または EWS を使用すると、メールボックスの電子メール メッセージを移動およびコピーすることができます。</span><span class="sxs-lookup"><span data-stu-id="95968-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="95968-106">**表 1 です。EWS のマネージ API のメソッドと移動し、電子メール メッセージのコピーの EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="95968-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="95968-107">**タスク**</span><span class="sxs-lookup"><span data-stu-id="95968-107">**Task**</span></span>|<span data-ttu-id="95968-108">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="95968-108">**EWS Managed API method**</span></span>|<span data-ttu-id="95968-109">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="95968-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="95968-110">電子メール メッセージの移動</span><span class="sxs-lookup"><span data-stu-id="95968-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="95968-111">EmailMessage.Move</span><span class="sxs-lookup"><span data-stu-id="95968-111">EmailMessage.Move</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="95968-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="95968-112">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="95968-113">電子メール メッセージのコピー</span><span class="sxs-lookup"><span data-stu-id="95968-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="95968-114">EmailMessage.Copy</span><span class="sxs-lookup"><span data-stu-id="95968-114">EmailMessage.Copy</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="95968-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="95968-115">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="95968-116">移動したり、電子メール メッセージを別のフォルダーにコピーすると、一意の項目の ID を持つ新しいフォルダーに新しい項目を作成し、元のメッセージの削除を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="95968-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="95968-117">応答を使用する新しいアイテムの ID にアクセスする新しいアイテムが返された場合の移動や同じメールボックスに 2 つのフォルダー間で電子メール メッセージをコピー、</span><span class="sxs-lookup"><span data-stu-id="95968-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="95968-118">ただし場合の移動や 2 つのメールボックスまたはメールボックスとパブリック フォルダーの間で電子メール メッセージをコピー、新しいアイテムが応答として返されません。</span><span class="sxs-lookup"><span data-stu-id="95968-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="95968-119">メッセージにアクセスする、移動したこのシナリオでは、マネージ API の EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)メソッドまたは EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作、 [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102) プロパティでは、[拡張プロパティの定義を作成](properties-and-extended-properties-in-ews-in-exchange.md)を使用または作成し、設定、プロパティは、新しいフォルダーにユーザー設定の拡張プロパティを検索し、ユーザー設定が拡張されます。</span><span class="sxs-lookup"><span data-stu-id="95968-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="95968-120">電子メール メッセージを削除することは、削除済みアイテム フォルダーにアイテムを移動すると異なっています。</span><span class="sxs-lookup"><span data-stu-id="95968-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="95968-121">EWS のマネージ API の[Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx)メソッドまたは EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)操作を使用する場合は、要求で指定されたアイテムは、元のフォルダーから削除し、コピーは、新しい項目の ID を使用して削除済みアイテム フォルダーに格納されます。</span><span class="sxs-lookup"><span data-stu-id="95968-121">If you use the EWS Managed API [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="95968-122">移動またはコピーする任意の項目とは異なり、 **Delete**メソッドまたは**DeleteItem**操作の応答に、新しいアイテムは返されません。</span><span class="sxs-lookup"><span data-stu-id="95968-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="95968-123">に関する手順は[、EWS のマネージ API を使用して電子メールを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma)か、 [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews)は、Exchange ストアから任意の汎用的な項目を削除するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="95968-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="95968-124">EWS マネージ API を使用して電子メール メッセージを移動する</span><span class="sxs-lookup"><span data-stu-id="95968-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="95968-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="95968-125"></span></span>

<span data-ttu-id="95968-126">次のコード例では、既存の電子メール メッセージを別の 1 つのフォルダーに移動する[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="95968-126">The following code example shows how to use the [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="95968-127">次の使用例は、**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと、その**アイテム Id**では、 [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx)電子メール メッセージの移動またはコピーすることを想定しています。</span><span class="sxs-lookup"><span data-stu-id="95968-127">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
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

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="95968-128">EWS を使用して電子メール メッセージを移動する</span><span class="sxs-lookup"><span data-stu-id="95968-128">Move an email message by using EWS</span></span>
<span data-ttu-id="95968-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="95968-129"></span></span>

<span data-ttu-id="95968-130">[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)操作を使用して、電子メール メッセージを [迷惑メール フォルダーに移動するのには次のコード例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95968-130">The following code example shows how to use the [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="95968-131">これは、 [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx)メソッドを呼び出すときに、EWS のマネージ API によって送信される XML の要求。</span><span class="sxs-lookup"><span data-stu-id="95968-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="95968-132">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="95968-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="95968-133">サーバーは、 **MoveItem**要求[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、電子メール メッセージが正常に移動されたことを示す値を含む[MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx)メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="95968-133">The server responds to the **MoveItem** request with a [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="95968-134">応答には、[新しいフォルダーの新しいフォルダーに**アイテム Id**が異なるために保管する必要が電子メール メッセージの**アイテム Id**も含まれています。</span><span class="sxs-lookup"><span data-stu-id="95968-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="95968-135">EWS マネージ API を使用して電子メール メッセージをコピーする</span><span class="sxs-lookup"><span data-stu-id="95968-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="95968-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="95968-136"></span></span>

<span data-ttu-id="95968-137">次のコード例では、1 つのフォルダーから既存の電子メール メッセージをコピーするには、 [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="95968-137">The following code example shows how to use the [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="95968-138">次の使用例は、**サービス**は、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトの有効なその**アイテム Id**は、コピーするのには電子メール メッセージの[Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx)を想定しています。</span><span class="sxs-lookup"><span data-stu-id="95968-138">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="95968-139">いくつかのパラメーターの値は、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="95968-139">The values of some parameters have been shortened for readability.</span></span> 
  
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

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="95968-140">EWS を使用して電子メール メッセージをコピーする</span><span class="sxs-lookup"><span data-stu-id="95968-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="95968-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="95968-141"></span></span>

<span data-ttu-id="95968-142">コード例を次の電子メール メッセージを移動するには、[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を送信して、 [ToFolderId のインストール先フォルダーを指定することによって、同じメールボックスに別のフォルダーに電子メール メッセージをコピーするのには、 [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx)操作を使用する方法を示しています。](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)要素です。</span><span class="sxs-lookup"><span data-stu-id="95968-142">The following code example shows how to use the [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="95968-143">[Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx)メソッドを呼び出すときに、EWS のマネージ API によって送信される XML の要求にもです。</span><span class="sxs-lookup"><span data-stu-id="95968-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="95968-144">読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="95968-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="95968-145">サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、電子メール メッセージが正常にコピーされたことを示す値を含む[CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx)メッセージで**CopyItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="95968-145">The server responds to the **CopyItem** request with a [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="95968-146">応答には、[新しいフォルダーの新しいフォルダーに**アイテム Id**が異なるために保管する必要が電子メール メッセージの**アイテム Id**も含まれています。</span><span class="sxs-lookup"><span data-stu-id="95968-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="95968-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="95968-147">See also</span></span>


- [<span data-ttu-id="95968-148">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="95968-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="95968-149">EWS を使用して Exchange が電子メール メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="95968-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

