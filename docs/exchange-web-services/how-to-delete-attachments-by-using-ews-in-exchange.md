---
title: Exchange EWS を使用して添付ファイルを削除します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Exchange で EWS マネージ API または EWS を使用して、EWS アイテムから添付物を削除する方法について説明します。
ms.openlocfilehash: 458331f81493283efc20d24c7e2bebe0e74bbdbd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758946"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="98335-103">Exchange EWS を使用して添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-103">Delete attachments by using EWS in Exchange</span></span>

<span data-ttu-id="98335-104">Exchange で EWS マネージ API または EWS を使用して、EWS アイテムから添付物を削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="98335-104">Learn how to delete attachments from items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="98335-105">際に削除するファイルおよびアイテムの添付ファイルの項目から EWS のマネージ API を使用して、いくつかのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="98335-105">You have a number of options when it comes to deleting file and item attachments from items by using the EWS Managed API.</span></span> <span data-ttu-id="98335-106">メッセージからすべての添付ファイルを削除、ファイル名を削除したり、コレクション内の位置を削除できます。</span><span class="sxs-lookup"><span data-stu-id="98335-106">You can delete all the attachments from the message, delete by a file name, or delete by position in the collection.</span></span> <span data-ttu-id="98335-107">これらのオプションのそれぞれについては、 [AttachmentCollection](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx)メソッドがあります。</span><span class="sxs-lookup"><span data-stu-id="98335-107">For each of these options, there is an [AttachmentCollection](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="98335-p102">一方、EWS を使用して、アイテムからすべての添付物を削除する場合も、1 つだけ削除する場合も、一連の操作は同じです。EWS マネージ API とは異なり、EWS には添付物の配列内の名前または位置に基づいて削除するための別の操作はありません。</span><span class="sxs-lookup"><span data-stu-id="98335-p102">Conversely, with EWS, no matter whether you're deleting all attachments from an item or just one, the sequence of operations is same. Unlike the EWS Managed API, EWS does not include separate operations to delete based on name or position in the attachments array.</span></span>
  
<span data-ttu-id="98335-110">**表 1 です。EWS のマネージ API のメソッドおよび添付ファイルを削除するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="98335-110">**Table 1. EWS Managed API methods and EWS operations for deleting attachments**</span></span>

|<span data-ttu-id="98335-111">**タスク**</span><span class="sxs-lookup"><span data-stu-id="98335-111">**Task**</span></span>|<span data-ttu-id="98335-112">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="98335-112">**EWS Managed API method**</span></span>|<span data-ttu-id="98335-113">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="98335-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="98335-114">アイテムからすべての添付物を削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-114">Delete all attachments from an item.</span></span>  <br/> |<span data-ttu-id="98335-115">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、 [AttachmentCollection.Clear](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx)、 [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)の後に続く</span><span class="sxs-lookup"><span data-stu-id="98335-115">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Clear](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="98335-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="98335-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="98335-117">名前でアイテムから添付物を削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-117">Delete an attachment from an item by name.</span></span>  <br/> |<span data-ttu-id="98335-118">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、 [AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx)、 [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)の後に続く</span><span class="sxs-lookup"><span data-stu-id="98335-118">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="98335-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="98335-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="98335-120">コレクション内の位置でアイテムから添付物を削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-120">Delete an attachment from an item by position in the collection.</span></span>  <br/> |<span data-ttu-id="98335-121">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)、 [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx)、 [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)の後に続く</span><span class="sxs-lookup"><span data-stu-id="98335-121">[Item.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="98335-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="98335-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="98335-123">EWS マネージ API を使用して、電子メールからすべての添付物を削除する</span><span class="sxs-lookup"><span data-stu-id="98335-123">Delete all attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="98335-124"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="98335-124"></span></span>

<span data-ttu-id="98335-125">次のコード例は、電子メールから添付物をすべて削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98335-125">The following code example shows how to delete all attachments from an email by:</span></span>
  
1. <span data-ttu-id="98335-126">[EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを使用して、既存の電子メール メッセージにバインドし、[添付ファイル](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="98335-126">Using the [EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="98335-127">[AttachmentCollection.Clear](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx)メソッドを使用して、電子メールからのすべての添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-127">Using the [AttachmentCollection.Clear](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) method to delete all the attachments from the email.</span></span> 
    
3. <span data-ttu-id="98335-128">[EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)メソッドを使用して、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="98335-128">Using the [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="98335-129">次の使用例は、Exchange サーバーにユーザーが認証されていると**サービス**は有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクト、**アイテム Id**は、元の添付ファイルは削除され、メッセージの[アイテム Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)を想定しています。</span><span class="sxs-lookup"><span data-stu-id="98335-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="98335-130">EWS マネージ API を使用して、電子メールから名前ですべての添付物を削除する</span><span class="sxs-lookup"><span data-stu-id="98335-130">Delete an attachment by name from an email by using the EWS Managed API</span></span>
<span data-ttu-id="98335-131"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="98335-131"></span></span>

<span data-ttu-id="98335-132">次のコード例では、名前で添付物を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98335-132">The following code example shows how delete an attachment by name by:</span></span>
  
1. <span data-ttu-id="98335-133">[EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを使用して、既存の電子メール メッセージにバインドし、[添付ファイル](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="98335-133">Using the [EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="98335-134">FileAttachment.txt をという名前の添付ファイルを削除するのには[AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx)メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="98335-134">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete an attachment named FileAttachment.txt.</span></span> 
    
3. <span data-ttu-id="98335-135">[EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)メソッドを使用して、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="98335-135">Using the [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="98335-136">次の使用例は、Exchange サーバーにユーザーが認証されていると**サービス**は有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクト、**アイテム Id**は、元の添付ファイルは削除され、メッセージの[アイテム Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)を想定しています。</span><span class="sxs-lookup"><span data-stu-id="98335-136">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a><span data-ttu-id="98335-137">EWS マネージ API を使用して位置で添付物を削除する</span><span class="sxs-lookup"><span data-stu-id="98335-137">Delete attachments by position by using the EWS Managed API</span></span>
<span data-ttu-id="98335-138"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="98335-138"></span></span>

<span data-ttu-id="98335-139">次のコード例は、添付物を位置で削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98335-139">The following code example shows how to delete an attachment by position by:</span></span>
  
1. <span data-ttu-id="98335-140">[EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)メソッドを使用して、既存の電子メール メッセージにバインドし、[添付ファイル](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx)と、 [EmailMessage.HasAttachments](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx)プロパティのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="98335-140">Using the [EmailMessage.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) and the [EmailMessage.HasAttachments](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) property.</span></span> 
    
2. <span data-ttu-id="98335-141">[AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx)メソッドを使用して、コレクション内の最初の添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="98335-141">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete the first attachment in the collection.</span></span> 
    
3. <span data-ttu-id="98335-142">[EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)メソッドを使用して、変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="98335-142">Using the [EmailMessage.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="98335-143">次の使用例は、Exchange サーバーにユーザーが認証されていると**サービス**は有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクト、**アイテム Id**は、元の添付ファイルは削除され、メッセージの[アイテム Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)を想定しています。</span><span class="sxs-lookup"><span data-stu-id="98335-143">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-attachments-from-an-item-by-using-ews"></a><span data-ttu-id="98335-144">EWS を使用してアイテムから添付物を削除する</span><span class="sxs-lookup"><span data-stu-id="98335-144">Delete attachments from an item by using EWS</span></span>
<span data-ttu-id="98335-145"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="98335-145"></span></span>

<span data-ttu-id="98335-146">EWS を使用して添付ファイルを削除するのには最初に、メッセージと添付データのコレクションの添付ファイルの[AttachmentId](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx)を決定する削除するのにを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98335-146">To delete attachments by using EWS, you first need to retrieve the message and the attachment collection to determine the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to delete.</span></span> <span data-ttu-id="98335-147">削除する 1 つまたは複数の**AttachmentId**の値を取得したら、 [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx)操作が指定した添付ファイルをメッセージから削除するを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="98335-147">After you have one or more **AttachmentId** values to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation to remove the specified attachments from the message.</span></span> 
  
<span data-ttu-id="98335-148">次のコード例は、[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作を使用して電子メール メッセージとメッセージの添付物のコレクションを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98335-148">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message.</span></span> <span data-ttu-id="98335-149">EWS のマネージ API は、[電子メールからのすべての添付ファイルを削除](#bk_deleteattachewsma)するのには EWS のマネージ API を使用する場合を送信する最初の XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="98335-149">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [delete all attachments from an email](#bk_deleteattachewsma).</span></span> <span data-ttu-id="98335-150">読みやすくするため、一部の属性の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98335-150">The values of some attributes are shortened for readability.</span></span>
  
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

<span data-ttu-id="98335-151">サーバーは、 **GetItem** 要求に [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) メッセージで応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/ja-jp/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode ** 値 、および既存の添付物の [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="98335-151">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-jp/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
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
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="98335-152">した後、どの添付ファイルを削除、 [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx)操作を呼び出すし、 **AttachmentId**の値を削除する添付ファイルを含めるを確認します。</span><span class="sxs-lookup"><span data-stu-id="98335-152">After you determine which attachment to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation and include the **AttachmentId** values of the attachments to delete.</span></span> 
  
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

サーバー要求に応答し、 **DeleteAttachment** **NoError**の[ResponseCode](http://msdn.microsoft.com/ja-jp/library/aa580757%28v=exchg.150%29.aspx)値は、各[DeleteAttachmentResponseMessage](http://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx)、ことを示します[DeleteAttachmentResponse](http://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx)メッセージ各添付ファイルが削除されました。 <span data-ttu-id="98335-154">読みやすくするため、一部の属性の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98335-154">The values of some attributes are shortened for readability.</span></span>
  
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
    <m:DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="98335-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="98335-155">See also</span></span>


- [<span data-ttu-id="98335-156">Exchange の添付物と EWS</span><span class="sxs-lookup"><span data-stu-id="98335-156">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="98335-157">Exchange EWS を使用して添付ファイルを追加します。</span><span class="sxs-lookup"><span data-stu-id="98335-157">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="98335-158">Exchange EWS を使用して添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="98335-158">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    

