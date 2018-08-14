---
title: Exchange で EWS を使用して Exchange メールボックス アイテムを操作する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Exchange で EWS マネージ API または EWS を使用して、アイテムを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353967"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="a47a0-103">Exchange で EWS を使用して Exchange メールボックス アイテムを操作する</span><span class="sxs-lookup"><span data-stu-id="a47a0-103">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="a47a0-104">Exchange で EWS マネージ API または EWS を使用して、アイテムを作成、取得、更新、削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a47a0-105">EWS マネージ API または EWS を使用すると、メールボックスのアイテムを処理することができます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span> <span data-ttu-id="a47a0-106">汎用アイテム (EWS マネージ API の [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトや EWS の [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) 型) を使用して、いくつかの操作 (アイテム識別子を使用したアイテムの取得や削除) を実行することができます。ただし、ほとんどの場合、取得操作または更新操作を実行するためには、厳密に型指定されたアイテムに固有のプロパティにアクセスする必要があるため、[厳密に型指定されたアイテム](folders-and-items-in-ews-in-exchange.md#bk_item)を使用しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a47a0-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="a47a0-107">たとえば、汎用アイテムを使用して、開始日と終了日を含むアイテムを取得することはできません。これを行うには、EWS マネージ API の [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) オブジェクトまたは EWS の [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) 型が必要です。</span><span class="sxs-lookup"><span data-stu-id="a47a0-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="a47a0-108">また、EWS マネージ API を使用している場合は、汎用 **Item** クラスにはコンストラクターがないため、厳密に型指定されたアイテムを常に作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a47a0-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="a47a0-109">厳密に型指定されていないアイテムを処理する場合は、いつでも、基本 **Item** クラスを使用してアイテムを処理することができます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="a47a0-110">**表 1. アイテムを処理するための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="a47a0-110">**Table 1. EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="a47a0-111">**目的…**</span><span class="sxs-lookup"><span data-stu-id="a47a0-111">**In order to…**</span></span>|<span data-ttu-id="a47a0-112">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="a47a0-112">**EWS Managed API method**</span></span>|<span data-ttu-id="a47a0-113">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="a47a0-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a47a0-114">汎用アイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="a47a0-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="a47a0-p103">なし。EWS マネージ API を使用して特定のアイテムの種類のみを作成できます。汎用アイテムを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p103">None. You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="a47a0-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="a47a0-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a47a0-118">アイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="a47a0-118">Get an item</span></span>  <br/> |[<span data-ttu-id="a47a0-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="a47a0-119">Item.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a47a0-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="a47a0-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a47a0-121">アイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="a47a0-121">Update an item</span></span>  <br/> |[<span data-ttu-id="a47a0-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="a47a0-122">Item.Update</span></span>](http://msdn.microsoft.com/ja-JP/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a47a0-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a47a0-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a47a0-124">アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="a47a0-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="a47a0-125">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="a47a0-125">Item.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a47a0-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="a47a0-126">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="a47a0-p104">この記事では、タスクを実行するために、汎用基本クラスを使用する場合と、厳密に型指定されたアイテムを使用する場合とについて説明します。コード例では、基本クラスを使用する方法と、基本クラスを使用できないとき、または基本クラスがニーズに合わないときの対処法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p104">In this article, you'll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task. The code examples will show you how to use the base class, and what to do when you can't use the base class or it doesn't fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="a47a0-129">EWS マネージ API を使用してアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="a47a0-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="a47a0-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-130"></span></span>

<span data-ttu-id="a47a0-p105">EWS マネージ API には、[Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) クラスの公式コンストラクターがないため、アイテムを作成するには、作成したい特定のアイテムの種類のためのコンストラクターを使用する必要があります。たとえば、 [EmailMessage クラス コンストラクター](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)を使用して、新しい電子メール メッセージを作成したり、[Contact クラス コンストラクター](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)を使用して新しい連絡先を作成したりします。同様に、サーバーは応答で汎用 **Item** オブジェクトを返すことはありません。すべての汎用アイテムは、 **EmailMessage** オブジェクトとして返されます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p105">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item. For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact. Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="a47a0-p106">作成するアイテムの種類が分かっている場合、わずかな手順だけでタスクを完了できます。この手順は、すべてのアイテムの種類について同様になります。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p106">When you know the type of item to create, you can complete the task in just a few steps. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="a47a0-136">パラメータとして [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オプジェクトを持ついずれかの [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) クラスの新しいインスタンスを初期化します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="a47a0-p107">アイテムのプロパティを設定します。スキーマはアイテムの種類ごとに異なるため、利用できるプロパティはアイテムに応じて異なってきます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p107">Set properties on the item. The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="a47a0-139">アイテムを保存するか、アイテムを保存して送信します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="a47a0-140">たとえば、[EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) オブジェクトを作成して、 [Subject](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx)、[Body](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)、および [ToRecipients](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) の各プロパティを設定し、 [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを使用して送信できます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

<span data-ttu-id="a47a0-141">EWS マネージ API を使用して会議または予定アイテムを作成する方法については、「[Exchange 2013 で EWS を使用して予定と会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see [How to: Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="a47a0-142">EWS を使用してアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="a47a0-142">Create an item by using EWS</span></span>
<span data-ttu-id="a47a0-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-143"></span></span>

<span data-ttu-id="a47a0-p108">EWS を使用して、汎用アイテムまたは厳密に型指定されたアイテムを作成できます。この手順は、すべてのアイテムの種類について同様になります。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p108">You can create a generic item or a strongly typed item by using EWS. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="a47a0-146">[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) 操作を使用して、Exchange ストアのアイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="a47a0-147">[Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) 要素を使用して、作成する 1 つ以上のアイテムを含めます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="a47a0-148">アイテムのプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-148">Set properties on the item.</span></span>
    
<span data-ttu-id="a47a0-p109">たとえば、次の例のコードを使用し、電子メール メッセージを作成して送信できます。これは、[SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p109">For example, you can create an email message and send it by using the code in the following example. This is also the XML request that the EWS Managed API sends when you call the [SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
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
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a47a0-151">サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="a47a0-152">EWS を使用して会議または予定アイテムを作成する方法については、「[Exchange 2013 で EWS を使用して予定および会議を作成する](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-152">To learn how to create a meeting or appointment item by using EWS, see [How to: Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="a47a0-153">EWS マネージ API を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="a47a0-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="a47a0-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-154"></span></span>

<span data-ttu-id="a47a0-p110">取得するアイテムの [Item.Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) が分かっている場合に EWS マネージ API を使用してアイテムを取得するには、アイテムに対して [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドのいずれかを呼び出すだけでアイテムが取得されます。ベスト プラクティスとして、必要なものだけを返すようにプロパティを制限することをお勧めします。次の例では、アイテムの **Id** プロパティと **Subject** プロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p110">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved. As a best practice, we recommend that you limit the properties returned to only those that are required. This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="a47a0-p111">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p111">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server. The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="a47a0-160">特定の条件を満たすアイテムを検索している場合は、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="a47a0-160">If you're searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="a47a0-161">取得するアイテムを含むフォルダーにバインドします。</span><span class="sxs-lookup"><span data-stu-id="a47a0-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="a47a0-162">[SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) または [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) をインスタンス化して、返すアイテムをフィルターにかけます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="a47a0-163">[ItemView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) オブジェクトまたは [CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) オブジェクトをインスタンス化して、返すアイテムの数を指定します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-163">Instantiate an [ItemView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="a47a0-164">[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは [ExchangeService.FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="a47a0-p112">たとえば、受信トレイに未読の電子メール メッセージを取得する場合は、次の例のコードを使用します。この例では、 **SearchFilterCollection** を使用して **FindItems** メソッドの結果を未読のメッセージに制限し、 **ItemView** を制限して結果を 1 つのアイテムに制限します。 [EmailMessageSchema.IsRead](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) の値が [SearchFilter](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx).の一部であるため、この特定のコードは、 **EmailMessage** オブジェクトでのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p112">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example. This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item. This particular code only works on [EmailMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

<span data-ttu-id="a47a0-p113">また、次のコード例に示すように、[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) を使用して検索結果を制限することもできます。この例では、 [FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを使用して、次の 30 日間で発生する最大 5 つの予定を取得します。このコードは、予定表アイテムでのみ機能します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p113">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example. This example uses the [FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days. This code of course only works on calendar items.</span></span> 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

<span data-ttu-id="a47a0-p114">**Bind** メソッドの応答でサーバーが返す情報は、 **FindItem** メソッドまたは **FindAppointment** メソッドの応答でサーバーが返す情報とは異なります。 **Bind** メソッドは、すべてのスキーマ化されたプロパティを返すことができますが、 **FindItem** メソッドと **FindAppointment** メソッドは、スキーマ化されたすべてのプロパティを返しません。このため、アイテムに対するフル アクセスが必要な場合は、 **Bind** メソッドを使用する必要があります。取得するアイテムの **Id** アイテムがない場合は、 **FindItem** メソッドまたは **FindAppointment** メソッドを使用して ID を取得し、 **Bind** メソッドを使用して必要なプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p114">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response. The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties. So if you need full access to the item, you'll have to use the **Bind** method. If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="a47a0-175">EWS マネージ API を使用して会議または予定アイテムを取得する方法については、「[Exchange で EWS を使用して予定および会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see [How to: Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="a47a0-176">EWS を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="a47a0-176">Get an item by using EWS</span></span>
<span data-ttu-id="a47a0-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-177"></span></span>

<span data-ttu-id="a47a0-178">取得するアイテムの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が分かっている場合は、 [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用してアイテムを取得できます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="a47a0-p115">次の例は、特定の [ItemId](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) を持つアイテムの **件名**を取得する XML の要求を示しています。これは、 [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) で **Bind** メソッドを呼び出す際に EWS マネージ API が送信する XML 要求でもあります。読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p115">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**. This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**. The values of some attributes and elements have been shortened for readability.</span></span>
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a47a0-p116">次の例は、 **GetItem** 操作の処理後にサーバーから返される XML 応答を示しています。この応答は、アイテムが正常に取得されたことを示しています。読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p116">The following example shows the XML response that the server returns after it processes the **GetItem** operation. The response indicates the item was retrieved successfully. The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="a47a0-p117">取得したいアイテムの **ItemId** が分からない場合は、 [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用してアイテムを見つけることができます。 **FindItem** 操作を使用するには、検索しているフォルダーをまず識別する必要があります。 **DistinguinguishedFolderName** または [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) を使用して、フォルダーを識別できます。 [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) または [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作のいずれかを使用して、必要な **FolderId** を取得することができます。 **FindItem** 操作を使用して、検索フィルターに一致する結果をそのフォルダーで検索します。EWS マネージ APIとは異なり、EWS は、予定のための別の検索操作を提供しません。 **FindItem** 操作がすべての種類のアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p117">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item. In order to use the **FindItem** operation, you must first identify the folder that you're searching. You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need. Then use the **FindItem** operation to search that folder for results that match the search filter. Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments. The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="a47a0-p118">次の例では、次の 30 日以内に発生する予定表フォルダー内で予定を検索するためにサーバーに送信される XMLの **FindItem** 操作要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p118">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a47a0-p119">サーバーは、**FindItemResponse** メッセージで [FindItem](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) 要求に応答します。このメッセージには、操作が正常に完了したことを示す、 [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** の値が含まれます。予定表アイテムがフィルターの条件を満たしている場合、それらのアイテムは応答に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p119">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully. If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="a47a0-p120">**GetItem** 操作の応答でサーバーが返す情報は、 **FindItem** 操作または **FindAppointment** 操作の応答でサーバーが返す情報とは異なります。 **GetItem** 操作は、すべてのスキーマ化されたプロパティを返すことができますが、 **FindItem** 操作と **FindAppointment** 操作は、スキーマ化されたすべてのプロパティを返しません。このため、アイテムに対するフル アクセスが必要な場合は、 **GetItem** 操作を使用する必要があります。取得するアイテムの **ItemId** がない場合は、 **FindItem** 操作または **FindAppointment** 操作を使用して **ItemId** を取得し、 **GetItem** 操作を使用して必要な要素を取得します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p120">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response. The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties. So if you need full access to the item, you'll have to use the **GetItem** operation. If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="a47a0-200">EWS を使用して会議または予定アイテムを取得する方法については、「[Exchange で EWS を使用して予定および会議を取得する](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-200">To learn how to get a meeting or appointment item by using EWS, see [How to: Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="a47a0-201">EWS マネージ API を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="a47a0-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="a47a0-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-202"></span></span>

<span data-ttu-id="a47a0-p121">EWS マネージ API を使用してアイテムを更新する手順は、すべてのアイテムの種類について同様になります。ただし、アイテムのプロパティは、アイテムの種類ごとに異なり、[Update](http://msdn.microsoft.com/ja-JP/library/office/dd635915%28v=exchg.80%29.aspx) メソッドには、選択できる多くのオーバーロードされたメソッドがあります。アイテムを更新するには:</span><span class="sxs-lookup"><span data-stu-id="a47a0-p121">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Update](http://msdn.microsoft.com/ja-JP/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from. To update an item:</span></span> 
  
1. <span data-ttu-id="a47a0-p122">最新バージョンのアイテムをまだ持っていない場合は、[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) メソッドを使用して取得します。厳密に型指定されたアイテム固有のプロパティを更新するには、その種類のアイテムにバインドする必要があります。汎用アイテムの種類で利用できるプロパティを更新するために、 [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトにバインドできます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p122">Use the [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get the latest version of the item, unless you already have it. To update properties specific to a strongly typed item, you'll have to bind to that item type. To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="a47a0-208">アイテムのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="a47a0-209">**Update** メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="a47a0-210">たとえば、次の例のコードに示すように、汎用アイテムの種類を使用して、電子メールの件名を更新できます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="a47a0-p123">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p123">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server. The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

<span data-ttu-id="a47a0-213">EWS マネージ API を使用して会議または予定アイテムを更新する方法については、「[Exchange で EWS を使用して予定および会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see [How to: Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="a47a0-214">EWS を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="a47a0-214">Update an item by using EWS</span></span>
<span data-ttu-id="a47a0-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-215"></span></span>

<span data-ttu-id="a47a0-216">EWS を使用してアイテムを更新するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="a47a0-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="a47a0-217">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) 操作を使用し、最新バージョンのアイテムをまだ持っていない場合は取得します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="a47a0-218">[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 操作を使用して、更新するフィールドを指定し、それらのフィールドに新しい値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="a47a0-p124">次の例は、電子メール メッセージの **Subject** の値を更新するためにサーバーに送信される XML [UpdateItem](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) 操作要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p124">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message. The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a47a0-221">サーバーは、**UpdateItemResponse** メッセージを含む [UpdateItem](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) 要求に応答します。このメッセージには、アイテムが正常に更新されたことを示す、 [NoError](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="a47a0-222">EWS を使用して会議または予定アイテムを更新する方法については、「[Exchange で EWS を使用して予定および会議を更新する](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-222">To learn how to update a meeting or appointment item by using EWS, see [How to: Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="a47a0-223">EWS マネージ API を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="a47a0-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="a47a0-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-224"></span></span>

<span data-ttu-id="a47a0-p125">アイテムを、削除済みアイテム フォルダーまたはごみ箱に移動して、削除できます。削除するアイテムの [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) が分かっている場合は、アイテムに対して [Delete](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p125">You can delete items by moving them to the Deleted Items folder or to the dumpster. If you know the [ItemId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="a47a0-227">削除する前にアイテムを検索する必要がある場合は、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="a47a0-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="a47a0-228">[FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドまたは [FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) メソッドを呼び出して、削除するアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-228">Call the [FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="a47a0-229">[PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) をインスタンス化して返すプロパティに制限するか、 [SearchFilterCollection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) を使用して特定のアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-229">Instantiate a [PropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="a47a0-230">[ItemView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) または [CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) をインスタンス化して、返すアイテムの数を指定します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-230">Instantiate an [ItemView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="a47a0-231">[Delete](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a47a0-231">Call the [Delete](http://msdn.microsoft.com/ja-JP/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="a47a0-232">たとえば次のコードは、電子メール メッセージを、削除済みアイテム フォルダーに移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="a47a0-p126">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。ローカル変数  *itemId*  は、更新するアイテムの [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) です。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p126">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server. The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="a47a0-235">アイテムの削除の詳細については、「[Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="a47a0-236">EWS マネージ API を使用して会議または予定アイテムを削除する方法については、「[Exchange で EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-236">To learn how to delete a meeting or appointment item by using the EWS Managed API, see [How to: Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="a47a0-237">EWS を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="a47a0-237">Delete an item by using EWS</span></span>
<span data-ttu-id="a47a0-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-238"></span></span>

<span data-ttu-id="a47a0-239">[DeleteItem](../web-service-reference/deleteitem-operation.md) 操作を使用して、アイテムを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-239">You can delete an item by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> 
  
<span data-ttu-id="a47a0-p128">次の例は、電子メール メッセージを削除済みアイテム フォルダーに移動するためにサーバーに送信される XML 要求を示しています。読みやすくするため、一部の属性と要素の値が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p128">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder. The values of some attributes and elements have been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a47a0-242">サーバーは、**DeleteItemResponse** メッセージを含む [DeleteItem](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) 要求に応答します。このメッセージには、アイテムが正常に更新されたことを示す、 [NoError](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) の **ResponseCode** 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a47a0-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/ja-JP/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="a47a0-243">アイテムの削除の詳細については、「[Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="a47a0-244">EWS を使用して会議または予定アイテムを削除する方法については、「[Exchange で EWS を使用して、予定を削除し、会議をキャンセルする](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-244">To learn how to delete a meeting or appointment item by using EWS, see [How to: Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="a47a0-245">別のメールボックスにアイテムを移動またはコピーする</span><span class="sxs-lookup"><span data-stu-id="a47a0-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="a47a0-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="a47a0-246"></span></span>

<span data-ttu-id="a47a0-p130">[ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) 操作と [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) 操作を使用して、メールボックス間でアイテムを移動またはコピーできます。詳細については、「 [Exchange で EWS を使用してアイテムをエクスポートおよびインポートする](exporting-and-importing-items-by-using-ews-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a47a0-p130">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations. To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a47a0-249">関連項目</span><span class="sxs-lookup"><span data-stu-id="a47a0-249">See also</span></span>

- [<span data-ttu-id="a47a0-250">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="a47a0-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="a47a0-251">Exchange で EWS を使用してフォルダーを操作する</span><span class="sxs-lookup"><span data-stu-id="a47a0-251">How to: Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="a47a0-252">Exchange で EWS を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="a47a0-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

