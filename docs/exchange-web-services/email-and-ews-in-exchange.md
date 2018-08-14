---
title: Exchange の電子メールと EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: 電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
ms.openlocfilehash: 2cd4613635bd2a5ecc061b50b0aecbdde1d32d46
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353673"
---
# <a name="email-and-ews-in-exchange"></a><span data-ttu-id="25e6e-103">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="25e6e-103">Email and EWS in Exchange</span></span>

<span data-ttu-id="25e6e-104">電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-104">Find out how to work with email messages, including how to create an email and how to perform other email-related tasks by using the EWS Managed API or EWS in Exchange.</span></span>
  

  
<span data-ttu-id="25e6e-105">Exchange で中核となるのは電子メールです。</span><span class="sxs-lookup"><span data-stu-id="25e6e-105">At its core, Exchange is about email.</span></span> <span data-ttu-id="25e6e-106">ところで、電子メールとは何でしょうか? </span><span class="sxs-lookup"><span data-stu-id="25e6e-106">But what makes an email an email?</span></span> <span data-ttu-id="25e6e-107">Exchange では電子メール メッセージは[厳密に型指定されたアイテム](folders-and-items-in-ews-in-exchange.md#bk_item)です。つまり、送信する前であっても特定の[一連のプロパティ](email-properties-and-elements-in-ews-in-exchange.md)が含まれます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-107">Well, email messages are one of the [strongly typed items](folders-and-items-in-ews-in-exchange.md#bk_item) in Exchange, which means that they contain a particular [set of properties](email-properties-and-elements-in-ews-in-exchange.md), even before they're sent.</span></span> <span data-ttu-id="25e6e-108">電子メール メッセージは、EWS マネージ API では [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) クラスによって、EWS では [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素とその子要素として表されます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-108">Email messages are represented by the [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) class in the EWS Managed API and by the [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element and its child elements in EWS.</span></span> 
  
<span data-ttu-id="25e6e-109">EWS マネージ API では、**EmailMessage** オブジェクトは [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="25e6e-109">In the EWS Managed API, the **EmailMessage** object derives from the [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="25e6e-110">**EmailMessage** クラスは、ほぼすべてのメッセージング シナリオで共通な [EmailMessage.Sender](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) および [EmailMessage.IsRead](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx) などの追加プロパティを提供して **Item** クラスを拡張します。</span><span class="sxs-lookup"><span data-stu-id="25e6e-110">The **EmailMessage** class extends the **Item** class by providing additional properties like [EmailMessage.Sender](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) and [EmailMessage.IsRead](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), which are now common to nearly all messaging scenarios.</span></span> <span data-ttu-id="25e6e-111">電子メール メッセージを取得、更新、削除するほとんどの操作は、**EmailMessage** オブジェクトまたは基本 **Item** オブジェクトを使用して行えます。作業対象のプロパティが [EmailMessageSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) クラスまたは [ItemSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) クラスのどちらにあるかによって使用するオブジェクトが異なります。</span><span class="sxs-lookup"><span data-stu-id="25e6e-111">When you get, update, or delete an email message, in most cases you can do that by using the **EmailMessage** object or the base **Item** object, depending on whether the properties you're working with are in the [EmailMessageSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) or the [ItemSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) class.</span></span> <span data-ttu-id="25e6e-112">アイテムの作成の場合には異なります。**Item** クラスにはコンストラクターがないため、電子メールを作成する場合、[EmailMessage コンストラクター](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)を使用して作成し、[EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) または [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) を使用して保存したり、送信してから保存したりします。</span><span class="sxs-lookup"><span data-stu-id="25e6e-112">Item creation is different because the **Item** class does not have a constructor, so when you're creating an email, you'll use the [EmailMessage constructor](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create it and the [EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) or [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) methods to save it, or send it and save it.</span></span> 
  
<span data-ttu-id="25e6e-p103">同様に、EWS では、[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素と併用して電子メール メッセージを作成します。EWS を使用してメールを取得、更新、削除するには、追加プロパティが電子メール メッセージで使用できるという点を除き、変更対象が電子メール メッセージであるということは重要とはなりません。その他の厳密に型指定されたアイテムに使用されるのと同じ操作が電子メール メッセージにも使用されます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-p103">Similarly, in EWS, use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element to create an email message. To get, update, or delete emails by using EWS, the fact that the item being modified is an email message is not important, aside from the fact that additional properties are available on email messages. The same operations that are used for other strongly typed items are also used for email messages.</span></span> 
  
|<span data-ttu-id="25e6e-116">**タスク**</span><span class="sxs-lookup"><span data-stu-id="25e6e-116">**Task**</span></span>|<span data-ttu-id="25e6e-117">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="25e6e-117">**EWS Managed API method**</span></span>|<span data-ttu-id="25e6e-118">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="25e6e-118">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25e6e-119">作成</span><span class="sxs-lookup"><span data-stu-id="25e6e-119">Create</span></span>  <br/> |[<span data-ttu-id="25e6e-120">EmailMessage.Save</span><span class="sxs-lookup"><span data-stu-id="25e6e-120">EmailMessage.Save</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25e6e-121">CreateItem</span><span class="sxs-lookup"><span data-stu-id="25e6e-121">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25e6e-122">取得</span><span class="sxs-lookup"><span data-stu-id="25e6e-122">Get</span></span>  <br/> |[<span data-ttu-id="25e6e-123">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="25e6e-123">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25e6e-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="25e6e-124">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25e6e-125">更新</span><span class="sxs-lookup"><span data-stu-id="25e6e-125">Update</span></span>  <br/> |[<span data-ttu-id="25e6e-126">Item.Update</span><span class="sxs-lookup"><span data-stu-id="25e6e-126">Item.Update</span></span>](http://msdn.microsoft.com/ja-JP/library/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25e6e-127">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="25e6e-127">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25e6e-128">削除</span><span class="sxs-lookup"><span data-stu-id="25e6e-128">Delete</span></span>  <br/> |[<span data-ttu-id="25e6e-129">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="25e6e-129">Item.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25e6e-130">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="25e6e-130">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="25e6e-131">電子メール メッセージは単純な[厳密に型指定されたアイテム](folders-and-items-in-ews-in-exchange.md#bk_item)であるため、場合によっては、[汎用アイテムを処理する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)のと同じ方法で扱えます。 </span><span class="sxs-lookup"><span data-stu-id="25e6e-131">Because email messages are simply [strongly typed items](folders-and-items-in-ews-in-exchange.md#bk_item), in some cases you work with them in the same way that you [work with generic items](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).</span></span> 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="25e6e-132">EWS マネージ API を使用して電子メール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="25e6e-132">Create an email message by using the EWS Managed API</span></span>
<span data-ttu-id="25e6e-133"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25e6e-133"></span></span>

<span data-ttu-id="25e6e-134">次の例のコードに示されているように、EWS マネージ API の [Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) メソッドを使用して電子メール メッセージを作成できます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-134">You can create an email message by using the EWS Managed API [Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) method, as shown in the code in the following example.</span></span> <span data-ttu-id="25e6e-135">この例では、[下書き] フォルダーにメッセージを保存しますが、メッセージは送信しません。</span><span class="sxs-lookup"><span data-stu-id="25e6e-135">Note that the example only saves the messages in the Drafts folder; it does not send the messages. For more about how to send the messages, see Send email messages in batches.</span></span> <span data-ttu-id="25e6e-136">メッセージを送信したり、メッセージの作成と送信を 1 ステップで行う方法については、[「Exchange で EWS を使用してメール メッセージを送信する」](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-136">For information about how to send the message or create and send the message in one step, see [Send email messages by using EWS in Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="25e6e-137">この例では、**service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="25e6e-137">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a new email message.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.ToRecipients.Add("mack@contoso.com");
message.Subject = "Project priorities";
message.Body = "(1) Buy pizza, (2) Eat pizza";
// Save the email message to the Drafts folder (where it can be retrieved, updated, and sent at a later time).
// This method call results in a CreateItem call to EWS.
message.Save(WellKnownFolderName.Drafts);
Console.WriteLine("A draft email message with the subject '" + message.Subject + "' has been saved to the Drafts folder.");
```

## <a name="create-an-email-message-by-using-ews"></a><span data-ttu-id="25e6e-138">EWS を使用して電子メール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="25e6e-138">Create an email message by using EWS</span></span>
<span data-ttu-id="25e6e-139"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="25e6e-139"></span></span>

<span data-ttu-id="25e6e-140">次の例に示されているように、EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して電子メール メッセージを作成できます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-140">You can create an email message by using the EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="25e6e-141">また、これは[電子メール メッセージが作成](#bk_createewsma)されるときに EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="25e6e-141">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](#bk_createewsma).</span></span> <span data-ttu-id="25e6e-142">次の例では、[下書き] フォルダーにメッセージを保存しますが、メッセージは送信しません。</span><span class="sxs-lookup"><span data-stu-id="25e6e-142">Note that the following example only saves the message in the Drafts folder, it does not send the message.</span></span> <span data-ttu-id="25e6e-143">メッセージを送信したり、メッセージの作成と送信を 1 ステップで行う方法については、[「Exchange で EWS を使用してメール メッセージを送信する」](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-143">For information about how to send the message or create and send the message in one ste, see [Send email messages by using EWS in Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="25e6e-144">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-144">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="25e6e-145">EWS マネージ API を使用して電子メール メッセージを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="25e6e-145">Get, update, and delete an email message by using the EWS Managed API</span></span>
<span data-ttu-id="25e6e-146"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25e6e-146"></span></span>

<span data-ttu-id="25e6e-147">EWS マネージ API を使用すると、Exchange ストアの汎用アイテムで実行するのと同じ方法で電子メール メッセージの取得、更新、削除を行えます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-147">You can use the EWS Managed API to get, update, or delete an email message in the same way that you perform these actions on any generic item from the Exchange store. For more information, see How to: Work with Exchange mailbox items by using EWS in Exchange.</span></span> <span data-ttu-id="25e6e-148">詳細は、[「Exchange で EWS を使用して Exchange メールボックス アイテムを操作する」](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-148">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>
  
<span data-ttu-id="25e6e-149">電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージ プロパティの一覧を[「Exchange における EWS でのメールのプロパティと要素」](email-properties-and-elements-in-ews-in-exchange.md)で確認してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-149">If you're updating an email message, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md) for a list of writable email message properties.</span></span> <span data-ttu-id="25e6e-150">下書きメッセージを更新してから送信するには、「[EWS マネージ API を使用して下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-150">If you’re updating an email message, see Email properties and elements for a list of writable email message properties. To send a draft message after you’ve updated it, see [Send a draft email message by using the EWS Managed API](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).</span></span>
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a><span data-ttu-id="25e6e-151">EWS を使用して電子メール メッセージを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="25e6e-151">Get, update, and delete an email message by using EWS</span></span>
<span data-ttu-id="25e6e-152"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="25e6e-152"></span></span>

<span data-ttu-id="25e6e-153">EWS を使用すると、Exchange ストアの汎用アイテムで実行するのと同じ方法で電子メール メッセージの取得、更新、削除を行えます。</span><span class="sxs-lookup"><span data-stu-id="25e6e-153">You can use EWS to get, update, and delete an email message in the same way that you perform these actions on any generic item from the Exchange store. For more information, see Get an item by using EWS.</span></span> <span data-ttu-id="25e6e-154">詳細は、[「Exchange で EWS を使用して Exchange メールボックス アイテムを操作する」](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-154">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>
  
<span data-ttu-id="25e6e-155">電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージ プロパティの一覧を[「Exchange における EWS でのメールのプロパティと要素」](email-properties-and-elements-in-ews-in-exchange.md)で確認してください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-155">If you're updating an email message, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md) for a list of writable email message properties.</span></span> <span data-ttu-id="25e6e-156">下書きメッセージを更新してから送信するには、「[EWS を使用して下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="25e6e-156">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="25e6e-157">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="25e6e-157">In this section</span></span>
<span data-ttu-id="25e6e-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="25e6e-158"></span></span>

- [<span data-ttu-id="25e6e-159">Exchange における EWS の電子メール プロパティと要素</span><span class="sxs-lookup"><span data-stu-id="25e6e-159">Email properties and elements in EWS in Exchange</span></span>](email-properties-and-elements-in-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-160">Exchange で EWS を使用してメール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="25e6e-160">How to: Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-161">Exchange において EWS を使用してメール メッセージに応答する</span><span class="sxs-lookup"><span data-stu-id="25e6e-161">How to: Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-162">Exchange において EWS を使用してメール メッセージを移動およびコピーする</span><span class="sxs-lookup"><span data-stu-id="25e6e-162">How to: Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-163">Exchange において EWS を使用して会話を処理する</span><span class="sxs-lookup"><span data-stu-id="25e6e-163">How to: Work with conversations by using EWS in Exchange</span></span>](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-164">Exchange において EWS を使用してメール メッセージからエンティティを抽出する</span><span class="sxs-lookup"><span data-stu-id="25e6e-164">How to: Extract an entity from an email message by using EWS in Exchange</span></span>](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="25e6e-165">Exchange で EWS を使用してバッチ処理でメール メッセージを処理する</span><span class="sxs-lookup"><span data-stu-id="25e6e-165">How to: Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="25e6e-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="25e6e-166">See also</span></span>


- [<span data-ttu-id="25e6e-167">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="25e6e-167">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="25e6e-168">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="25e6e-168">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

