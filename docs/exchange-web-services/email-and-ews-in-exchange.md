---
title: Exchange の電子メールと EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: 電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
ms.openlocfilehash: d222be7409a3c3f4613a2be39b83b977fabb09e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758886"
---
# <a name="email-and-ews-in-exchange"></a><span data-ttu-id="5ac03-103">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="5ac03-103">Email and EWS in Exchange</span></span>

<span data-ttu-id="5ac03-104">電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-104">Find out how to work with email messages, including how to create an email and how to perform other email-related tasks by using the EWS Managed API or EWS in Exchange.</span></span>
  

  
<span data-ttu-id="5ac03-105">中核となる、Exchange はメールです。</span><span class="sxs-lookup"><span data-stu-id="5ac03-105">At its core, Exchange is about email.</span></span> <span data-ttu-id="5ac03-106">電子メール e メールは、何でしょうか。</span><span class="sxs-lookup"><span data-stu-id="5ac03-106">But what makes an email an email?</span></span> <span data-ttu-id="5ac03-107">電子メール メッセージは[厳密に型指定の項目](folders-and-items-in-ews-in-exchange.md#bk_item)のいずれかの Exchange に含まれること、特定[のプロパティの設定](email-properties-and-elements-in-ews-in-exchange.md)、送信することにも。</span><span class="sxs-lookup"><span data-stu-id="5ac03-107">Well, email messages are one of the [strongly typed items](folders-and-items-in-ews-in-exchange.md#bk_item) in Exchange, which means that they contain a particular [set of properties](email-properties-and-elements-in-ews-in-exchange.md), even before they're sent.</span></span> <span data-ttu-id="5ac03-108">電子メール メッセージは、EWS のマネージ API の[なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)のクラスと[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)の要素および EWS では、その子要素によって表されます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-108">Email messages are represented by the [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) class in the EWS Managed API and by the [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element and its child elements in EWS.</span></span> 
  
<span data-ttu-id="5ac03-109">EWS のマネージ API では、 **email メッセージ**オブジェクトは、 [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)オブジェクトから派生します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-109">In the EWS Managed API, the **EmailMessage** object derives from the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="5ac03-110">**なか**クラスは、ほぼすべてのメッセージング シナリオに共通では[EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx)と[EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx)のような追加のプロパティを提供することにより**項目**クラスを拡張します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-110">The **EmailMessage** class extends the **Item** class by providing additional properties like [EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) and [EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), which are now common to nearly all messaging scenarios.</span></span> <span data-ttu-id="5ac03-111">取得、更新、または**なか**オブジェクトまたは[EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx)または、[プロパティを扱う場合は、基本**項目**オブジェクトを使用して行うことができますほとんどの場合、電子メール メッセージを削除するときItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx)クラス。</span><span class="sxs-lookup"><span data-stu-id="5ac03-111">When you get, update, or delete an email message, in most cases you can do that by using the **EmailMessage** object or the base **Item** object, depending on whether the properties you're working with are in the [EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) or the [ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) class.</span></span> <span data-ttu-id="5ac03-112">アイテムの作成とは異なる**項目**クラスがコンス トラクターを持たないためため、電子メールを作成するときに使用する[コンス トラクターのなか](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)と、 [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx)または[EmailMessage.SendAndSaveCopy を作成するには](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)保存または送信し、それを保存するためのメソッドです。</span><span class="sxs-lookup"><span data-stu-id="5ac03-112">Item creation is different because the **Item** class does not have a constructor, so when you're creating an email, you'll use the [EmailMessage constructor](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create it and the [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) or [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) methods to save it, or send it and save it.</span></span> 
  
<span data-ttu-id="5ac03-113">同様に、EWS でを使用して[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)要素を使用して電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-113">Similarly, in EWS, use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element to create an email message.</span></span> <span data-ttu-id="5ac03-114">取得、更新、または EWS を使用して電子メールを削除、変更されている項目が電子メール メッセージであることは重要ですが、追加のプロパティが電子メール メッセージで使用可能であること以外ではありません。</span><span class="sxs-lookup"><span data-stu-id="5ac03-114">To get, update, or delete emails by using EWS, the fact that the item being modified is an email message is not important, aside from the fact that additional properties are available on email messages.</span></span> <span data-ttu-id="5ac03-115">電子メール メッセージを他の厳密に型指定された項目に使用されるのと同じ操作が使用されます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-115">The same operations that are used for other strongly typed items are also used for email messages.</span></span> 
  
|<span data-ttu-id="5ac03-116">**タスク**</span><span class="sxs-lookup"><span data-stu-id="5ac03-116">**Task**</span></span>|<span data-ttu-id="5ac03-117">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="5ac03-117">**EWS Managed API method**</span></span>|<span data-ttu-id="5ac03-118">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5ac03-118">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5ac03-119">作成</span><span class="sxs-lookup"><span data-stu-id="5ac03-119">Create</span></span>  <br/> |[<span data-ttu-id="5ac03-120">EmailMessage.Save</span><span class="sxs-lookup"><span data-stu-id="5ac03-120">EmailMessage.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5ac03-121">CreateItem</span><span class="sxs-lookup"><span data-stu-id="5ac03-121">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5ac03-122">取得</span><span class="sxs-lookup"><span data-stu-id="5ac03-122">Get</span></span>  <br/> |[<span data-ttu-id="5ac03-123">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="5ac03-123">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5ac03-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="5ac03-124">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5ac03-125">更新</span><span class="sxs-lookup"><span data-stu-id="5ac03-125">Update</span></span>  <br/> |[<span data-ttu-id="5ac03-126">Item.Update</span><span class="sxs-lookup"><span data-stu-id="5ac03-126">Item.Update</span></span>](http://msdn.microsoft.com/en-us/library/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5ac03-127">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5ac03-127">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5ac03-128">削除</span><span class="sxs-lookup"><span data-stu-id="5ac03-128">Delete</span></span>  <br/> |[<span data-ttu-id="5ac03-129">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="5ac03-129">Item.Delete</span></span>](http://msdn.microsoft.com/en-us/library/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5ac03-130">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5ac03-130">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="5ac03-131">電子メールは、メッセージの[項目を厳密に型指定](folders-and-items-in-ews-in-exchange.md#bk_item)をするだけであるため場合によっては、作業中と同じようにその[汎用的な項目を操作します](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="5ac03-131">Because email messages are simply [strongly typed items](folders-and-items-in-ews-in-exchange.md#bk_item), in some cases you work with them in the same way that you [work with generic items](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).</span></span> 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="5ac03-132">EWS マネージ API を使用して電子メール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="5ac03-132">Create an email message by using the EWS Managed API</span></span>
<span data-ttu-id="5ac03-133"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5ac03-133"></span></span>

<span data-ttu-id="5ac03-134">次の例のコードに示すように、EWS のマネージ API の[保存](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx)メソッドを使用して、電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-134">You can create an email message by using the EWS Managed API [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) method, as shown in the code in the following example.</span></span> <span data-ttu-id="5ac03-135">例は、下書きフォルダーにメッセージを保存するだけで、メッセージは送信されないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-135">Note that the example only saves the message in the Drafts folder, it does not send the message.</span></span> <span data-ttu-id="5ac03-136">メッセージを送信または作成し、1 つのステップで、メッセージを送信する方法の詳細については、 [Exchange での EWS を使用して、電子メール メッセージの送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-136">For information about how to send the message or create and send the message in one step, see [Send email messages by using EWS in Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="5ac03-137">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="5ac03-137">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="create-an-email-message-by-using-ews"></a><span data-ttu-id="5ac03-138">EWS を使用して電子メール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="5ac03-138">Create an email message by using EWS</span></span>
<span data-ttu-id="5ac03-139"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="5ac03-139"></span></span>

<span data-ttu-id="5ac03-140">EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用して電子メール メッセージを作成するには、次の例のようにします。</span><span class="sxs-lookup"><span data-stu-id="5ac03-140">You can create an email message by using the EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="5ac03-141">これは、XML の要求の場合、EWS のマネージ API を送信する[電子メール メッセージを作成](#bk_createewsma)します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-141">This is also the XML request that the EWS Managed API sends when you [create an email message](#bk_createewsma).</span></span> <span data-ttu-id="5ac03-142">注意してください次の例は、下書きフォルダーにメッセージを保存するだけのメッセージを送信しません。</span><span class="sxs-lookup"><span data-stu-id="5ac03-142">Note that the following example only saves the message in the Drafts folder, it does not send the message.</span></span> <span data-ttu-id="5ac03-143">メッセージを送信または作成し、1 つのサイトで、メッセージを送信する方法の詳細については、 [Exchange での EWS を使用して、電子メール メッセージの送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-143">For information about how to send the message or create and send the message in one ste, see [Send email messages by using EWS in Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).</span></span>
  
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

<span data-ttu-id="5ac03-144">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-144">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="5ac03-145">EWS マネージ API を使用して電子メール メッセージを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="5ac03-145">Get, update, and delete an email message by using the EWS Managed API</span></span>
<span data-ttu-id="5ac03-146"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5ac03-146"></span></span>

<span data-ttu-id="5ac03-147">取得、更新、または Exchange ストアからの任意の一般的な項目では、これらのアクションを実行することと同じ方法で電子メール メッセージを削除するのには、EWS のマネージ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-147">You can use the EWS Managed API to get, update, or delete an email message in the same way that you perform these actions on any generic item from the Exchange store.</span></span> <span data-ttu-id="5ac03-148">詳細については、 [Exchange EWS を使用して Exchange メールボックスのアイテムの作業](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-148">For more information, see [Work with Exchange mailbox items by using EWS in Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="5ac03-149">電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージのプロパティの一覧については[プロパティおよび EWS での要素を Exchange メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-149">If you're updating an email message, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md) for a list of writable email message properties.</span></span> <span data-ttu-id="5ac03-150">下書きメッセージを送信するには、それを更新した後に、 [EWS のマネージ API を使用して、下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-150">To send a draft message after you've updated it, see [Send a draft email message by using the EWS Managed API](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).</span></span>
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a><span data-ttu-id="5ac03-151">EWS を使用して電子メール メッセージを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="5ac03-151">Get, update, and delete an email message by using EWS</span></span>
<span data-ttu-id="5ac03-152"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="5ac03-152"></span></span>

<span data-ttu-id="5ac03-153">取得、更新、および Exchange ストアからの任意の一般的な項目では、これらのアクションを実行することと同じ方法で電子メール メッセージを削除するのには、EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="5ac03-153">You can use EWS to get, update, and delete an email message in the same way that you perform these actions on any generic item from the Exchange store.</span></span> <span data-ttu-id="5ac03-154">詳細については、 [Exchange EWS を使用して Exchange メールボックスのアイテムの作業](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-154">For more information, see [Work with Exchange mailbox items by using EWS in Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="5ac03-155">電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージのプロパティの一覧については[プロパティおよび EWS での要素を Exchange メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-155">If you're updating an email message, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md) for a list of writable email message properties.</span></span> <span data-ttu-id="5ac03-156">下書きメッセージを送信するは、それを更新した後、 [EWS を使用して、下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac03-156">To send a draft message after you've updated it, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="5ac03-157">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="5ac03-157">In this section</span></span>
<span data-ttu-id="5ac03-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="5ac03-158"></span></span>

- [<span data-ttu-id="5ac03-159">EWS での要素のプロパティとの Exchange 電子メールします。</span><span class="sxs-lookup"><span data-stu-id="5ac03-159">Email properties and elements in EWS in Exchange</span></span>](email-properties-and-elements-in-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-160">EWS を使用して Exchange が電子メール メッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-160">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-161">EWS を使用して Exchange が電子メール メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-161">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-162">移動し、EWS を使用して Exchange が電子メール メッセージをコピー</span><span class="sxs-lookup"><span data-stu-id="5ac03-162">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-163">Exchange EWS を使用して会話を扱う</span><span class="sxs-lookup"><span data-stu-id="5ac03-163">Work with conversations by using EWS in Exchange</span></span>](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-164">EWS を使用して Exchange が電子メール メッセージからエンティティを抽出します。</span><span class="sxs-lookup"><span data-stu-id="5ac03-164">Extract an entity from an email message by using EWS in Exchange</span></span>](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5ac03-165">電子メール メッセージを Exchange で EWS を使用してバッチ プロセス</span><span class="sxs-lookup"><span data-stu-id="5ac03-165">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="5ac03-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ac03-166">See also</span></span>


- [<span data-ttu-id="5ac03-167">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="5ac03-167">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="5ac03-168">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="5ac03-168">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    

