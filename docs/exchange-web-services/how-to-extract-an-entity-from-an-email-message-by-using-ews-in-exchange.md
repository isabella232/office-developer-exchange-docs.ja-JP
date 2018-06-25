---
title: EWS を使用して Exchange が電子メール メッセージからエンティティを抽出します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 6396b009-5f6e-41eb-a75a-224d43e864ae
description: Exchange において  EWS マネージ API または EWS を使用して、メール メッセージの本文から情報を抽出する方法を説明します。
ms.openlocfilehash: d3d5c4b756347a4cedede184709884d5ed8f08b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758949"
---
# <a name="extract-an-entity-from-an-email-message-by-using-ews-in-exchange"></a><span data-ttu-id="76a00-103">EWS を使用して Exchange が電子メール メッセージからエンティティを抽出します。</span><span class="sxs-lookup"><span data-stu-id="76a00-103">Extract an entity from an email message by using EWS in Exchange</span></span>

<span data-ttu-id="76a00-104">Exchange において  EWS マネージ API または EWS を使用して、メール メッセージの本文から情報を抽出する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="76a00-104">Learn how to extract information from the body of an email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="76a00-p101">EWS マネージ API または EWS を使用して、Exchange サーバーがメール メッセージから抽出する住所、連絡先、メール アドレス、提案された会議、電話番号、タスク、URL にアクセスできます。この情報を新しいアプリのために使用したり、既存のアプリでこの情報を使用してさまざまなアクションの次の処理を提案したりできます。たとえば、連絡先エンティティ、提案された会議、タスクのヒントがメールの中で識別された場合、お客様のアプリで、情報を事前設定して新しいアイテムの作成を提案できます。抽出されたエンティティを使用して、データの背後にある意図を十分に生かすことができます。さらに、メール メッセージのコンテンツを実行できる成果へとシームレスに統合できるよう、ユーザーを支援します。</span><span class="sxs-lookup"><span data-stu-id="76a00-p101">You can use the EWS Managed API or EWS to access the addresses, contacts, email addresses, meeting suggestions, phone numbers, tasks, and URLs that an Exchange server extracts from email messages. You can then use this information for new applications or to suggest follow up actions in existing applications. For example, if a contact entity, meeting suggestion, or task suggestion is identified in an email, your application can suggest that a new item with prepopulated information be created. By using extracted entities, you can capitalize on the intent behind the data — and help users seamlessly integrate their email message content into actionable results.</span></span>
  
<span data-ttu-id="76a00-109">アドレス、連絡先、電子メール アドレス、会議提案、電話番号、タスク、および Url のエンティティの抽出は、Exchange ストア内のすべての項目に既に組み込まれて。</span><span class="sxs-lookup"><span data-stu-id="76a00-109">Entity extraction for addresses, contacts, email addresses, meeting suggestions, phone numbers, tasks, and URLs is already built in to every item in the Exchange store.</span></span> <span data-ttu-id="76a00-110">EWS のマネージ API を使用する場合、 [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx)プロパティは、 [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドの呼び出しでのエンティティを取得します。</span><span class="sxs-lookup"><span data-stu-id="76a00-110">If you're using the EWS Managed API, the [Item.EntityExtractionResult](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx) property retrieves the entities for you in an [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method call.</span></span> <span data-ttu-id="76a00-111">EWS を使用する場合、 [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx)要素は、 [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)操作の呼び出しでの抽出されたすべてのエンティティを取得します。</span><span class="sxs-lookup"><span data-stu-id="76a00-111">If you're using EWS, the [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) element gets all the extracted entities for you in a [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="76a00-112">抽出されたエンティティの結果を取得した後に関連する情報を収集する各エンティティのコレクションを移動することができます。</span><span class="sxs-lookup"><span data-stu-id="76a00-112">After you retrieve the results of the extracted entities, you can walk through each entity collection to gather pertinent information.</span></span> <span data-ttu-id="76a00-113">など、提案された会議が抽出された場合は、提案された会議の件名、出席者リスト、開始時刻、および終了時刻を取得できます。</span><span class="sxs-lookup"><span data-stu-id="76a00-113">For example, if a meeting suggestion was extracted, you can retrieve the suggested meeting subject, attendee list, start time, and end time.</span></span> 
  
<span data-ttu-id="76a00-114">**表 1 です。EWS のマネージ API のプロパティと、EWS の要素が含まれているエンティティを展開します。**</span><span class="sxs-lookup"><span data-stu-id="76a00-114">**Table 1. EWS Managed API properties and EWS elements that contain extracted entities**</span></span>

|<span data-ttu-id="76a00-115">**抽出されたエンティティ**</span><span class="sxs-lookup"><span data-stu-id="76a00-115">**Extracted entity**</span></span>|<span data-ttu-id="76a00-116">**EWS のマネージ API のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="76a00-116">**EWS Managed API property**</span></span>|<span data-ttu-id="76a00-117">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="76a00-117">**EWS element**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="76a00-118">住所</span><span class="sxs-lookup"><span data-stu-id="76a00-118">Addresses</span></span>  <br/> |[<span data-ttu-id="76a00-119">EntityExtractionResult.Addresses</span><span class="sxs-lookup"><span data-stu-id="76a00-119">EntityExtractionResult.Addresses</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-120">アドレス</span><span class="sxs-lookup"><span data-stu-id="76a00-120">Addresses</span></span>](http://msdn.microsoft.com/library/0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-121">連絡先</span><span class="sxs-lookup"><span data-stu-id="76a00-121">Contacts</span></span>  <br/> |[<span data-ttu-id="76a00-122">EntityExtractionResult.Contacts</span><span class="sxs-lookup"><span data-stu-id="76a00-122">EntityExtractionResult.Contacts</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.contacts%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-123">連絡先</span><span class="sxs-lookup"><span data-stu-id="76a00-123">Contacts</span></span>](http://msdn.microsoft.com/library/a2c1e833-5f8c-438d-bad7-bb5dcc29ca9e%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-124">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="76a00-124">Email addresses</span></span>  <br/> |[<span data-ttu-id="76a00-125">EntityExtractionResult.EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="76a00-125">EntityExtractionResult.EmailAddresses</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.emailaddresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-126">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="76a00-126">EmailAddresses</span></span>](http://msdn.microsoft.com/library/2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-127">提案された会議</span><span class="sxs-lookup"><span data-stu-id="76a00-127">Meeting suggestions</span></span>  <br/> |[<span data-ttu-id="76a00-128">EntityExtractionResult.MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="76a00-128">EntityExtractionResult.MeetingSuggestions</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.meetingsuggestions%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-129">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="76a00-129">MeetingSuggestions</span></span>](http://msdn.microsoft.com/library/c99e9a60-9e38-425d-ad03-47c8917f41da%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-130">電話番号</span><span class="sxs-lookup"><span data-stu-id="76a00-130">Phone numbers</span></span>  <br/> |[<span data-ttu-id="76a00-131">EntityExtractionResult.PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="76a00-131">EntityExtractionResult.PhoneNumbers</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.phonenumbers%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-132">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="76a00-132">PhoneNumbers</span></span>](http://msdn.microsoft.com/library/9ff6ae98-34a1-47f7-bde5-608251a789f7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-133">タスクのヒント</span><span class="sxs-lookup"><span data-stu-id="76a00-133">Task suggestions</span></span>  <br/> |[<span data-ttu-id="76a00-134">EntityExtractionResult.TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="76a00-134">EntityExtractionResult.TaskSuggestions</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-135">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="76a00-135">TaskSuggestions</span></span>](http://msdn.microsoft.com/library/7d3c6314-2a5c-4fc3-b5f9-ae6d4946aac3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="76a00-136">URL</span><span class="sxs-lookup"><span data-stu-id="76a00-136">URLs</span></span>  <br/> |[<span data-ttu-id="76a00-137">EntityExtractionResult.Urls</span><span class="sxs-lookup"><span data-stu-id="76a00-137">EntityExtractionResult.Urls</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.entityextractionresult.addresses%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="76a00-138">Url</span><span class="sxs-lookup"><span data-stu-id="76a00-138">Urls</span></span>](http://msdn.microsoft.com/library/c39744ea-0cee-4954-8653-8279d6b10161%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="76a00-p103">エンティティの抽出は自然言語の認識機能に依存するため、エンティティの認識は非決定的で、成功するかどうかはコンテキストに依存しています。自然言語の認識がどのように機能するかを示すため、この記事の例では入力として次のメールを使用します。</span><span class="sxs-lookup"><span data-stu-id="76a00-p103">Because entity extraction relies on natural language recognition, the recognition of entities can be non-deterministic and success sometimes relies on the context. To demonstrate how natural language recognition works, the examples in this article use the following email as input.</span></span>
  
 `From: Ronnie Sturgis`
  
 `To: Sadie Daniels`
  
 `Subject: Dinner party`
  
 `Hi Sadie`
  
 `Are you free this Friday at 7 to join us for a dinner party at our house?`
  
 `We're at 789 International Blvd, St Paul MN 55104.`
  
 `Our number is 612-555-0158 if you have trouble finding it.`
  
 `Please RSVP to either myself or Mara (mara@contoso.com) before Friday morning. Best for you organics (http://www.bestforyouorganics.com) will be catering so we can fully enjoy ourselves!`
  
 `Also, can you forward this to Magdalena? I don't have her contact information.`
  
 `See you then!`
  
 `Ronnie`
  
## <a name="extract-all-entities-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="76a00-141">EWS マネージ API を使用して、メールからすべてのエンティティを抽出する</span><span class="sxs-lookup"><span data-stu-id="76a00-141">Extract all entities from an email by using the EWS Managed API</span></span>
<span data-ttu-id="76a00-142"><a name="bk_extractewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="76a00-142"></span></span>

<span data-ttu-id="76a00-143">次のコード例では、 [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)メソッドを使用し、抽出されたエンティティとそのプロパティの各反復で、サーバーによって抽出されたすべてのエンティティを表示する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="76a00-143">The following code example shows how to display all the entities extracted by the server, by using the [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method, and then enumerating through each of the extracted entities and their properties.</span></span> 
  
<span data-ttu-id="76a00-144">次の使用例は、**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと、その**アイテム Id**では、 [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx)電子メール メッセージの移動またはコピーすることを想定しています。</span><span class="sxs-lookup"><span data-stu-id="76a00-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
```cs
public static void ExtractEntities(ExchangeService service, ItemId ItemId)
{
    // Create a property set that limits the properties returned 
    // by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.EntityExtractionResult);
    // Get the item from the server.
    // This method call results in an GetItem call to EWS.
    Item item = Item.Bind(service, ItemId, propSet);
    Console.WriteLine("The following entities have been extracted from the message:");
    Console.WriteLine(" ");
    // If address entities are extracted from the message, print the results.
    if (item.EntityExtractionResult != null)
    {
        if (item.EntityExtractionResult.Addresses != null)
        {
            Console.WriteLine("--------------------Addresses---------------------------");
            foreach (AddressEntity address in item.EntityExtractionResult.Addresses)
            {
                Console.WriteLine("Address: {0}", address.Address);
            }
            Console.WriteLine(" ");
        }
        // If contact entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Contacts != null)
        {
            Console.WriteLine("--------------------Contacts----------------------------");
            foreach (ContactEntity contact in item.EntityExtractionResult.Contacts)
            {
                Console.WriteLine("Addresses:       {0}", contact.Addresses);
                Console.WriteLine("Business name:   {0}", contact.BusinessName);
                Console.WriteLine("Contact string:  {0}", contact.ContactString);
                Console.WriteLine("Email addresses: {0}", contact.EmailAddresses);
                Console.WriteLine("Person name:     {0}", contact.PersonName);
                Console.WriteLine("Phone numbers:   {0}", contact.PhoneNumbers);
                Console.WriteLine("URLs:            {0}", contact.Urls);
            }
            Console.WriteLine(" ");
        }
        // If email address entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.EmailAddresses != null)
        {
            Console.WriteLine("--------------------Email addresses---------------------");
            foreach (EmailAddressEntity email in item.EntityExtractionResult.EmailAddresses)
            {
                Console.WriteLine("Email addresses: {0}", email.EmailAddress);
            }
            Console.WriteLine(" ");
        }
        // If meeting suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.MeetingSuggestions != null)
        {
            Console.WriteLine("--------------------Meeting suggestions-----------------");
            foreach (MeetingSuggestion meetingSuggestion in item.EntityExtractionResult.MeetingSuggestions)
            {
                Console.WriteLine("Meeting subject:  {0}", meetingSuggestion.Subject);
                Console.WriteLine("Meeting string:   {0}", meetingSuggestion.MeetingString);
                foreach (EmailUserEntity attendee in meetingSuggestion.Attendees)
                {
                    Console.WriteLine("Attendee name:    {0}", attendee.Name);
                    Console.WriteLine("Attendee user ID: {0}", attendee.UserId);
                }
                Console.WriteLine("Start time:       {0}", meetingSuggestion.StartTime);
                Console.WriteLine("End time:         {0}", meetingSuggestion.EndTime);
                Console.WriteLine("Location:         {0}", meetingSuggestion.Location);
            }
            Console.WriteLine(" ");
        }
        // If phone number entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.PhoneNumbers != null)
        {
            Console.WriteLine("--------------------Phone numbers-----------------------");
            foreach (PhoneEntity phone in item.EntityExtractionResult.PhoneNumbers)
            {
                Console.WriteLine("Original phone string:  {0}", phone.OriginalPhoneString);
                Console.WriteLine("Phone string:           {0}", phone.PhoneString);
                Console.WriteLine("Type:                   {0}", phone.Type);
            }
            Console.WriteLine(" ");
        }
        // If task suggestion entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.TaskSuggestions != null)
        {
            Console.WriteLine("--------------------Task suggestions--------------------");
            foreach (TaskSuggestion task in item.EntityExtractionResult.TaskSuggestions)
            {
                foreach (EmailUserEntity assignee in task.Assignees)
                {
                    Console.WriteLine("Assignee name:    {0}", assignee.Name);
                    Console.WriteLine("Assignee user ID: {0}", assignee.UserId);
                }
                Console.WriteLine("Task string:      {0}", task.TaskString);
            }
            Console.WriteLine(" ");
        }
        // If URL entities are extracted from the message, print the results.
        if (item.EntityExtractionResult.Urls != null)
        {
            Console.WriteLine("--------------------URLs--------------------------------");
            foreach (UrlEntity url in item.EntityExtractionResult.Urls)
            {
                Console.WriteLine("URL: {0}", url.Url);
            }
            Console.WriteLine(" ");
        }
    }
    // If no entities are extracted from the message, print the result.
    else if (item.EntityExtractionResult == null)
    {
        Console.WriteLine("No entities extracted");
    }
}
```

<span data-ttu-id="76a00-145">次の出力がコンソールに表示されます。</span><span class="sxs-lookup"><span data-stu-id="76a00-145">The following output is displayed on the console.</span></span>
  
```text
The following entities have been extracted from the message:
 
--------------------Addresses---------------------------
Address: 789 International Blvd, St Paul MN 55104
 
--------------------Contacts----------------------------
Addresses:       
Business name:   
Contact string:  Mara (mara@contoso.com)
Email addresses: mara@contoso.com
Person name:     Mara
Phone numbers:   
URLs:            
 
--------------------Email addresses---------------------
Email addresses: mara@contoso.com
 
--------------------Meeting suggestions-----------------
Meeting subject:  dinner party
Meeting string:   Are you free this Friday at 7 to join us for a dinner party at our house?
Attendee name:    Ronnie Sturgis
Attendee user ID: ronnie@contoso.com
Attendee name:    Sadie Daniels
Attendee user ID: sadie@cntoso.com
Start time:       10/1/0104 2:00:00 PM
End time:         10/1/0104 2:30:00 PM
Location:         
 
--------------------Phone numbers-----------------------
Original phone string:  612-555-0158
Phone string:           6125550158
Type:                   Unspecified
 
--------------------Task suggestions--------------------
Assignee name:    Sadie Daniels
Assignee user ID: sadie@contoso.com
Task string:      Also, can you forward this to Magdalena?
 
--------------------URLs--------------------------------
URL: http://www.bestforyouorganics.com
```

<span data-ttu-id="76a00-146">すべてのアドレス、連絡先、電子メール アドレス、電話番号、タスク、および Url が展開されたこと期待どおりに注意してください。</span><span class="sxs-lookup"><span data-stu-id="76a00-146">Notice that all addresses, contacts, email addresses, phone numbers, tasks, and URLs were extracted as expected.</span></span> <span data-ttu-id="76a00-147">ただし、会議候補は、少し複雑です。</span><span class="sxs-lookup"><span data-stu-id="76a00-147">The meeting suggestion, however, is a bit more complex.</span></span> <span data-ttu-id="76a00-148">通知、提案された会議の終了時刻と開始時刻は、期待どおりでない場合があります。</span><span class="sxs-lookup"><span data-stu-id="76a00-148">Notice the start time and end time of the meeting suggestion are not what you might expect.</span></span> <span data-ttu-id="76a00-149">電子メールの開始時刻は「この金曜日 7 時」ですが、抽出された開始時刻の値は、10/1/0104 午後 2:00:00 です。</span><span class="sxs-lookup"><span data-stu-id="76a00-149">The start time in the email is "this Friday at 7", but the extracted value for the start time is 10/1/0104 2:00:00 PM.</span></span> <span data-ttu-id="76a00-150">これは、開始時刻と終了時刻の抽出には、サーバーがエンコードされた日付であるためです。</span><span class="sxs-lookup"><span data-stu-id="76a00-150">This is because the start time and end time extracted by the server are encoded dates.</span></span> <span data-ttu-id="76a00-151">会議の提案では、 **dateTime**値を解釈する方法の詳細についてを参照してください[[MS OXCEXT]: クライアント拡張機能のメッセージ オブジェクト プロトコル](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="76a00-151">For more information about how to interpret **dateTime** values in meeting suggestions, see [[MS-OXCEXT]: Client Extension Message Object Protocol](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span></span>
  
## <a name="extract-all-entities-from-an-email-by-using-ews"></a><span data-ttu-id="76a00-152">EWS を使用して、メールからすべてのエンティティを抽出する</span><span class="sxs-lookup"><span data-stu-id="76a00-152">Extract all entities from an email by using EWS</span></span>
<span data-ttu-id="76a00-153"><a name="bk_extractews"> </a></span><span class="sxs-lookup"><span data-stu-id="76a00-153"></span></span>

<span data-ttu-id="76a00-154">アイテムから抽出されたエンティティを取得するために[GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)操作と[EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx)の要素を使用する方法を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="76a00-154">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation and the [EntityExtractionResult](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx) element to retrieve the extracted entities from an item.</span></span> 
  
<span data-ttu-id="76a00-155">[EWS のマネージ API を使用して、電子メールからのすべてのエンティティを抽出](#bk_extractewsma)するのには**Bind**メソッドを使用するときに、EWS のマネージ API で送信される XML の要求にもです。</span><span class="sxs-lookup"><span data-stu-id="76a00-155">This is also the XML request that is sent by the EWS Managed API when you use the **Bind** method to [Extract all entities from an email by using the EWS Managed API](#bk_extractewsma).</span></span>
  
<span data-ttu-id="76a00-156">[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)要素の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="76a00-156">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element is shortened for readability.</span></span> 
  
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
          <t:FieldURI FieldURI="item:EntityExtractionResult" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="sVC5AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、電子メール メッセージが正常に取得されたことを示す値を含む[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx)メッセージの**GetItem**要求に応答します。 <span data-ttu-id="76a00-158">応答には、抽出された各エンティティの**EntityExtractionResult**も含まれています。</span><span class="sxs-lookup"><span data-stu-id="76a00-158">The response also includes the **EntityExtractionResult** for each extracted entity.</span></span> 
  
<span data-ttu-id="76a00-159">**アイテム Id**要素の値は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="76a00-159">The value of the **ItemId** element is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
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
              <t:ItemId Id="sVC5AAA="
                        ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAOOqJN" />
              <t:EntityExtractionResult>
                <t:Addresses>
                  <t:AddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Address>789 International Blvd, St Paul MN 55104</t:Address>
                  </t:AddressEntity>
                </t:Addresses>
                <t:MeetingSuggestions>
                  <t:MeetingSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:Attendees>
                      <t:EmailUser>
                        <t:Name>Ronnie Sturgis</t:Name>
                        <t:UserId>ronnie@contoso.com</t:UserId>
                      </t:EmailUser>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Attendees>
                    <t:Subject>dinner party</t:Subject>
                    <t:MeetingString>Are you free this Friday at 7 to join us for a dinner party at our house?</t:MeetingString>
                    <t:StartTime>0104-10-01T19:00:00Z</t:StartTime>
                    <t:EndTime>0104-10-01T19:30:00Z</t:EndTime>
                  </t:MeetingSuggestion>
                </t:MeetingSuggestions>
                <t:TaskSuggestions>
                  <t:TaskSuggestion>
                    <t:Position>LatestReply</t:Position>
                    <t:TaskString>Also, can you forward this to Magdalena?</t:TaskString>
                    <t:Assignees>
                      <t:EmailUser>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:UserId>sadie@contoso.com</t:UserId>
                      </t:EmailUser>
                    </t:Assignees>
                  </t:TaskSuggestion>
                </t:TaskSuggestions>
                <t:EmailAddresses>
                  <t:EmailAddressEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                  </t:EmailAddressEntity>
                </t:EmailAddresses>
                <t:Contacts>
                  <t:Contact>
                    <t:Position>LatestReply</t:Position>
                    <t:PersonName>Mara</t:PersonName>
                    <t:EmailAddresses>
                      <t:EmailAddress>mara@contoso.com</t:EmailAddress>
                    </t:EmailAddresses>
                    <t:ContactString>Mara (mara@contoso.com</t:ContactString>
                  </t:Contact>
                </t:Contacts>
                <t:Urls>
                  <t:UrlEntity>
                    <t:Position>LatestReply</t:Position>
                    <t:Url>http://www.bestforyouorganics.com</t:Url>
                  </t:UrlEntity>
                </t:Urls>
                <t:PhoneNumbers>
                  <t:Phone>
                    <t:Position>LatestReply</t:Position>
                    <t:OriginalPhoneString>612-555-0158</t:OriginalPhoneString>
                    <t:PhoneString>6125550158</t:PhoneString>
                    <t:Type>Unspecified</t:Type>
                  </t:Phone>
                </t:PhoneNumbers>
              </t:EntityExtractionResult>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="76a00-160">すべてのアドレス、連絡先、電子メール アドレス、電話番号、タスク、および Url が展開されたこと期待どおりに注意してください。</span><span class="sxs-lookup"><span data-stu-id="76a00-160">Notice that all addresses, contacts, email addresses, phone numbers, tasks, and URLs were extracted as expected.</span></span> <span data-ttu-id="76a00-161">ただし、会議候補は、少し複雑です。</span><span class="sxs-lookup"><span data-stu-id="76a00-161">The meeting suggestion, however, is a bit more complex.</span></span> <span data-ttu-id="76a00-162">通知、提案された会議の終了時刻と開始時刻は、期待どおりでない場合があります。</span><span class="sxs-lookup"><span data-stu-id="76a00-162">Notice the start time and end time of the meeting suggestion are not what you might expect.</span></span> <span data-ttu-id="76a00-163">電子メールの開始時刻が「この金曜日 7 時」であるが、抽出された開始時刻の値、10/1/0104 午後 2:00:00 です。</span><span class="sxs-lookup"><span data-stu-id="76a00-163">The start time in the email was "this Friday at 7", but the extracted value for the start time is 10/1/0104 2:00:00 PM.</span></span> <span data-ttu-id="76a00-164">これは、開始時刻と終了時刻の抽出には、サーバーがエンコードされた日付であるためです。</span><span class="sxs-lookup"><span data-stu-id="76a00-164">This is because the start time and end time extracted by the server are encoded dates.</span></span> <span data-ttu-id="76a00-165">会議の提案では、 **dateTime**値の解釈の詳細についてを参照してください[[MS OXCEXT]: クライアント拡張機能のメッセージ オブジェクト プロトコル](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="76a00-165">For more information about interpreting **dateTime** values in meeting suggestions, see [[MS-OXCEXT]: Client Extension Message Object Protocol](http://msdn.microsoft.com/en-us/library/hh968601%28v=exchg.80%29.aspx).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="76a00-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="76a00-166">See also</span></span>

- [<span data-ttu-id="76a00-167">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="76a00-167">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="76a00-168">Item.EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="76a00-168">Item.EntityExtractionResult</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.entityextractionresult%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="76a00-169">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="76a00-169">EntityExtractionResult</span></span>](http://msdn.microsoft.com/library/643b99ab-ff90-4411-864c-1077623028d6%28Office.15%29.aspx)
    

