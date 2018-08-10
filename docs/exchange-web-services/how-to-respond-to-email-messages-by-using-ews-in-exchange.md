---
title: Exchange において EWS を使用してメール メッセージに応答する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d584991-4d67-4d36-ae2f-99970af8488f
description: Exchange で EWS マネージ API または EWS を使用してメール メッセージに応答する方法について説明します。
ms.openlocfilehash: 2f1428251084a7f2bf8d589a788c143f34b64d5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759052"
---
# <a name="respond-to-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="a757d-103">Exchange において EWS を使用してメール メッセージに応答する</span><span class="sxs-lookup"><span data-stu-id="a757d-103">How to: Respond to email messages by using EWS in Exchange</span></span>

<span data-ttu-id="a757d-104">Exchange で EWS マネージ API または EWS を使用してメール メッセージに応答する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a757d-104">Learn how to respond to email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a757d-105">EWS マネージ API または EWS を使用して、メッセージに返信したり、受信者にメッセージに転送したりすることでメッセージに応答できます。</span><span class="sxs-lookup"><span data-stu-id="a757d-105">You can use the EWS Managed API or EWS to respond to messages by replying to them or forwarding them to recipients.</span></span>
  
<span data-ttu-id="a757d-106">**表 1. メール メッセージに応答するための EWS マネージ API のメソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="a757d-106">**Table 1.  EWS Managed API methods and EWS operations for responding to email messages**</span></span>

|<span data-ttu-id="a757d-107">**タスク**</span><span class="sxs-lookup"><span data-stu-id="a757d-107">**Task**</span></span>|<span data-ttu-id="a757d-108">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="a757d-108">**EWS Managed API method**</span></span>|<span data-ttu-id="a757d-109">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="a757d-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a757d-110">メール メッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="a757d-110">Reply to an email message</span></span>  <br/> |[<span data-ttu-id="a757d-111">EmailMessage.Reply</span><span class="sxs-lookup"><span data-stu-id="a757d-111">EmailMessage.Reply</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a757d-112">EmailMessage.CreateReply</span><span class="sxs-lookup"><span data-stu-id="a757d-112">EmailMessage.CreateReply</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="a757d-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)。[Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) 要素には、[ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) または [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) という子要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a757d-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of either [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) or [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="a757d-114">メール メッセージの転送</span><span class="sxs-lookup"><span data-stu-id="a757d-114">Forward an email message</span></span>  <br/> |[<span data-ttu-id="a757d-115">EmailMessage.Forward</span><span class="sxs-lookup"><span data-stu-id="a757d-115">EmailMessage.Forward</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a757d-116">EmailMessage.CreateForward</span><span class="sxs-lookup"><span data-stu-id="a757d-116">EmailMessage.CreateForward</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="a757d-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)。[Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) 要素には [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) という子要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a757d-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span></span>  <br/> |
   
## <a name="reply-to-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="a757d-118">EWS マネージ API を使用してメール メッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="a757d-118">Reply to an email message by using the EWS Managed API</span></span>
<span data-ttu-id="a757d-119"><a name="bk_replyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a757d-119"></span></span>

<span data-ttu-id="a757d-120">EWS マネージ API には、メッセージへの応答に使用できる [ Reply ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) と [CreateReply](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) という 2 つのメソッドがあります。</span><span class="sxs-lookup"><span data-stu-id="a757d-120">The EWS Managed API provides two methods that you can use to respond to messages: [Reply](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) and [CreateReply](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="a757d-121">**Reply** メソッドは、2 つのパラメーターだけを取ります。既存の本文の先頭に追加する応答メッセージと、すべての受信者に送信するか (ture) 送信者だけに送信するか (false) を指定する **Boolean** 値です。</span><span class="sxs-lookup"><span data-stu-id="a757d-121">The **Reply** method only takes two parameters: the response message to prepend to the existing body, and a **Boolean** value that indicates whether the response should go to all recipients (true) or just the sender (false).</span></span> <span data-ttu-id="a757d-122">他の受信者をメッセージに追加したり、応答に追加プロパティを設定したり、添付物を追加したりする必要がある場合は、**CreateReply** メソッドを使用します。このメソッドでは、[EmailMessage](email-properties-and-elements-in-ews-in-exchange.md) オブジェクトで使用可能なすべての[ファースト クラスのプロパティ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)を設定できます。</span><span class="sxs-lookup"><span data-stu-id="a757d-122">If you need to add additional recipients to a message, set additional properties on a response, or add an attachment, use the **CreateReply** method, which enables you to set all the [first-class properties](email-properties-and-elements-in-ews-in-exchange.md) that are available on an [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="a757d-123">次のコード例は、**Reply** メソッドを使用してメール メッセージに応答する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-123">The following code example shows how to use the **Reply** method to respond to an email message.</span></span> 
  
<span data-ttu-id="a757d-124">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="a757d-125">ローカル変数 *ItemId* は、対応するアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="a757d-125">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> <span data-ttu-id="a757d-126">この例では、[FindRecentlySent メソッド](#bk_findlast)を呼び出して、メッセージに返信済みのマークが付けられたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a757d-126">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as replied to.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.LastModifiedTime);
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
string myReply = "This is the message body of the email reply.";
bool replyToAll = false;
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Reply(myReply, replyToAll);
// Verify that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="a757d-127">次のコード例は、**CreateReply** メソッドを使用してメール メッセージに応答する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-127">The following code example shows how to use the **CreateReply** method to respond to an email message.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
bool replyToAll = true;
ResponseMessage responseMessage = message.CreateReply(replyToAll);
// Prepend the reply to the message body. 
string myReply = "This is the message body of the email reply.";
responseMessage.BodyPrefix = myReply;
// Send the response message.
// This method call results in a CreateItem call to EWS.
responseMessage.SendAndSaveCopy();
// Check that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="a757d-128">応答メッセージに添付物を追加する場合は、**SendAndSaveCopy** メソッドへの呼び出しを次のコードに置換します。</span><span class="sxs-lookup"><span data-stu-id="a757d-128">If you need to add an attachment to the response message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage reply = responseMessage.Save();
reply.Attachments.AddFileAttachment("attachmentname.txt");
reply.Update(ConflictResolutionMode.AutoResolve);
reply.SendAndSaveCopy();
```

## <a name="reply-to-an-email-message-by-using-ews"></a><span data-ttu-id="a757d-129">EWS を使用してメール メッセージに返信する</span><span class="sxs-lookup"><span data-stu-id="a757d-129">Reply to an email message by using EWS</span></span>
<span data-ttu-id="a757d-130"><a name="bk_replyews"> </a></span><span class="sxs-lookup"><span data-stu-id="a757d-130"></span></span>

<span data-ttu-id="a757d-131">次のコード例は、EWS を使用してメッセージに返信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-131">The following code example shows how to reply to a message by using EWS.</span></span> <span data-ttu-id="a757d-132">**MessageDisposition** 属性が **SendAndSaveCopy** に設定されている [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して、メッセージを送信し、送信済みアイテム フォルダーに応答を保存します。</span><span class="sxs-lookup"><span data-stu-id="a757d-132">The following code example shows how to forward a message by using EWS. Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder. The ForwardItem element indicates that the item is a forwarded message.</span></span> <span data-ttu-id="a757d-133">[ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) 要素を [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) 要素の子として含めてメッセージ スレッド上の全員に返信するか、[ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) 要素を含めて送信者にのみ返信します。</span><span class="sxs-lookup"><span data-stu-id="a757d-133">The following code example shows how to reply to a message by using EWS. Use the CreateItem operation with the MessageDisposition attribute set to SendAndSaveCopy to send the message and save the response in the Sent Items folder. Include either the [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) element as a child of the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element to reply to everyone on the message thread, or include the [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) element to reply only to the sender.</span></span> 
  
<span data-ttu-id="a757d-134">これは、[Reply](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) メソッドまたは [CreateReply](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a757d-134">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) method on an [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ReplyAllToItem>
          <t:ReferenceItemId Id="AAMkADE4="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the email reply.</t:NewBodyContent>
        </t:ReplyAllToItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a757d-135">サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、応答が正常に作成および送信されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a757d-135">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the reply was created and sent successfully.</span></span>
  
<span data-ttu-id="a757d-136">応答メッセージに添付物を追加する必要がある場合、前述したように **CreateItem** 操作を呼び出しますが、**MessageDisposition** は **SaveOnly** に変更します。</span><span class="sxs-lookup"><span data-stu-id="a757d-136">If you need to add an attachment to your response message, call the CreateItem operation as specified above, but change the MessageDisposition to SaveOnly. Then call the CreateAttachment operation, followed by the SendItem operation.</span></span> <span data-ttu-id="a757d-137">次に、[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) 操作を呼び出してから、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a757d-137">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="forward-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="a757d-138">EWS マネージ API を使用してメール メッセージを転送する</span><span class="sxs-lookup"><span data-stu-id="a757d-138">Forward an email message by using the EWS Managed API</span></span>
<span data-ttu-id="a757d-139"><a name="bk_forwardewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a757d-139"></span></span>

<span data-ttu-id="a757d-140">EWS マネージ API には、メッセージの転送に使用できる [Forward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) と [CreateForward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) という 2 つのメソッドがあります。</span><span class="sxs-lookup"><span data-stu-id="a757d-140">The EWS Managed API provides two methods that you can use to forward messages: [Forward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) and [CreateForward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="a757d-141">**Forward** メソッドは、2 つのパラメーターだけを取ります。使用するオーバーロードに応じて、既存の本文に先頭に付加するメッセージと、受信者の配列またはコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a757d-141">The **Forward** method only takes two parameters: the message to prepend to the existing body, and an array or collection of recipients, depending on the overload you choose to use.</span></span> <span data-ttu-id="a757d-142">転送するメッセージに添付物を追加したり、新しいメッセージで追加プロパティを設定したりする必要がある場合は、**CreateForward** メソッドを使用します。このメソッドでは、[EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトで使用可能なすべてのプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="a757d-142">If you need to add an attachment to the message you're forwarding, or set additional properties on the new message, use the **CreateForward** method, which enables you to set all the properties that are available on an [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="a757d-143">次のコード例は、**Forward** メソッドを使用してメール メッセージを 1 人の受信者に転送する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-143">The following code example shows how to use the **Forward** method to forward an email message to one recipient.</span></span> 
  
<span data-ttu-id="a757d-144">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="a757d-145">ローカル変数 *ItemId* は、転送するアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="a757d-145">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> <span data-ttu-id="a757d-146">この例では、[FindRecentlySent メソッド](#bk_findlast) を呼び出して、メッセージに転送済みのマークが付けられたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a757d-146">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as forwarded.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
string myForward = "This is the message body of the forwarded email.";
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Forward(myForward, "sadie@contoso.com");
// Verify that the forwarded response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="a757d-147">次のコード例は、**CreateForward** メソッドを使用してメール メッセージを 1 人の受信者に転送する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-147">The following code example shows how to use the **CreateForward** method to forward an email message to one recipient.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
ResponseMessage forwardMessage = message.CreateForward();
// Set properties on the email message.
forwardMessage.ToRecipients.Add("sadie@contoso.com");
forwardMessage.Body = "Sadie,<br><br>I thought you'd be interested in this thread.<br><br>-Mack";
// Send and save a copy of the replied email message in the default Sent Items folder. 
forwardMessage.SendAndSaveCopy();
// Verify that the forwarded message was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="a757d-148">転送されるメッセージに添付物を追加する場合は、**SendAndSaveCopy** メソッドへの呼び出しを次のコードに置換します。</span><span class="sxs-lookup"><span data-stu-id="a757d-148">If you need to add an attachment to the forwarded message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage forward = forwardMessage.Save();
forward.Attachments.AddFileAttachment("attachmentname.txt");
forward.Update(ConflictResolutionMode.AutoResolve);
forward.SendAndSaveCopy();
```

## <a name="forward-an-email-message-by-using-ews"></a><span data-ttu-id="a757d-149">EWS を使用してメール メッセージを転送する</span><span class="sxs-lookup"><span data-stu-id="a757d-149">Forward an email message by using EWS</span></span>
<span data-ttu-id="a757d-150"><a name="bk_forwardews"> </a></span><span class="sxs-lookup"><span data-stu-id="a757d-150"></span></span>

<span data-ttu-id="a757d-151">次のコード例は、EWS を使用してメッセージを転送する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a757d-151">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span> <span data-ttu-id="a757d-152">**MessageDisposition** 属性が **SendAndSaveCopy** に設定されている [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して、メッセージを送信し、送信済みアイテム フォルダーに応答を保存します。</span><span class="sxs-lookup"><span data-stu-id="a757d-152">The following code example shows how to forward a message by using EWS. Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder. The ForwardItem element indicates that the item is a forwarded message.</span></span> <span data-ttu-id="a757d-153">[ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) 要素は、そのアイテムが転送されるメッセージであることを示します。</span><span class="sxs-lookup"><span data-stu-id="a757d-153">The [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) element indicates that the item is a forwarded message.</span></span> 
  
<span data-ttu-id="a757d-154">これは、[Forward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) メソッドまたは [CreateForward](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a757d-154">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) method on an [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ForwardItem>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:ReferenceItemId Id="AAAMkADE="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the forwarded email.</t:NewBodyContent>
        </t:ForwardItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a757d-155">サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、転送済みメッセージが正常に作成および送信されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a757d-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the forwarded message was created and sent successfully.</span></span>
  
<span data-ttu-id="a757d-156">応答メッセージに添付物を追加する必要がある場合、**CreateItem** 操作を呼び出しますが、**MessageDisposition** を **SaveOnly** に変更します。</span><span class="sxs-lookup"><span data-stu-id="a757d-156">If you need to add an attachment to your response message, call the CreateItem operation, but change the MessageDisposition to SaveOnly. Then call the CreateAttachment operation, followed by the SendItem operation.</span></span> <span data-ttu-id="a757d-157">次に、[CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) 操作を呼び出してから、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a757d-157">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="find-the-message-last-replied-to-or-forwarded-by-using-the-ews-managed-api"></a><span data-ttu-id="a757d-158">EWS マネージ API を使用して最後に返信または転送されたメッセージを検索する</span><span class="sxs-lookup"><span data-stu-id="a757d-158">Find the message last replied to or forwarded by using the EWS Managed API</span></span>
<span data-ttu-id="a757d-159"><a name="bk_findlast"> </a></span><span class="sxs-lookup"><span data-stu-id="a757d-159"></span></span>

<span data-ttu-id="a757d-p109">次のコード例は、指定されたアイテムで実行された最後の動詞と、最後の動詞が実行された時間を検索する方法を示しています。このメソッドは、このトピックの他の EWS マネージ API コード例から呼び出され、返信または転送したアイテムが受信トレイで返信済みまたは転送済みとしてマークされていることを確認します。 </span><span class="sxs-lookup"><span data-stu-id="a757d-p109">The following code example shows how to find the last verb executed and the time the last verb was executed on the item specified. This method is called from other EWS Managed API code examples in this topic to verify that the items you replied to or forwarded were marked as replied to or forwarded in your Inbox.</span></span> 
  
<span data-ttu-id="a757d-162">この例では、[PidTagLastVerbExecuted](http://msdn.microsoft.com/ja-JP/library/cc841968.aspx) (0x10820003) 拡張プロパティを使用して、メッセージが [返信]、[全員に返信]、[転送] のどれであるかを判別します。また、[PidTagLastVerbExecutionTime](http://msdn.microsoft.com/ja-JP/library/cc839918.aspx) (0x10820040) 拡張プロパティを使用して、返信または転送がいつ送信されたかを判別します。</span><span class="sxs-lookup"><span data-stu-id="a757d-162">The example uses the [PidTagLastVerbExecutedhttp://msdn.microsoft.com/ja-JP/library/cc841968.aspx](http://msdn.microsoft.com/ja-JP/library/cc841968.aspx) (0x10820003) extended property to determine whether the message was a reply, a reply all, or a forward, and the [PidTagLastVerbExecutionTimehttp://msdn.microsoft.com/ja-JP/library/cc839918.aspx](http://msdn.microsoft.com/ja-JP/library/cc839918.aspx) (0x10820040) extended property to determine when the reply or forward was sent.</span></span> 
  
```cs
public static void FindRecentlySent(EmailMessage messageToCheck)
{
    // Create extended property definitions for PidTagLastVerbExecuted and PidTagLastVerbExecutionTime.
    ExtendedPropertyDefinition PidTagLastVerbExecuted = new ExtendedPropertyDefinition(0x1081, MapiPropertyType.Integer);
    ExtendedPropertyDefinition PidTagLastVerbExecutionTime = new ExtendedPropertyDefinition(0x1082, MapiPropertyType.SystemTime);
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, PidTagLastVerbExecutionTime, PidTagLastVerbExecuted);
    messageToCheck = EmailMessage.Bind(service, messageToCheck.Id, propSet);
    // Determine the last verb executed on the message and display output.
    object responseType;
    if (messageToCheck.TryGetProperty(PidTagLastVerbExecuted, out responseType))
    {
        object ReplyTime = null;
        switch (((Int32)responseType))
        {
            case 102: Console.WriteLine("A reply was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 103: Console.WriteLine("A reply all was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 104: Console.WriteLine("The '" + messageToCheck.Subject.ToString() + "' email message was forwarded at");
                break;
        }
        if (messageToCheck.TryGetProperty(PidTagLastVerbExecutionTime, out ReplyTime))
        {
            Console.WriteLine(((DateTime)ReplyTime).ToString() + ".");
        }
    }
    else
    {
        Console.WriteLine("No changes were made to  '" + messageToCheck.Subject.ToString() + "'.");
    }
}
```

## <a name="see-also"></a><span data-ttu-id="a757d-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="a757d-163">See also</span></span>


- [<span data-ttu-id="a757d-164">Exchange のメールと EWS</span><span class="sxs-lookup"><span data-stu-id="a757d-164">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a757d-165">Exchange で EWS を使用してメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="a757d-165">How to: Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

