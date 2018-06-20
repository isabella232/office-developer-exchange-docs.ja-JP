---
title: Exchange EWS を使用してバッチ プロセスの連絡先
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 455f475b-cb19-4e7a-8ff3-92f7028fceb0
description: Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで連絡先の作成、取得、更新、削除をバッチ処理する方法について説明します。
ms.openlocfilehash: 7dfbda7fe5e077f92bcf7ebd40af40d76c2d2d22
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759046"
---
# <a name="process-contacts-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="2b430-103">Exchange EWS を使用してバッチ プロセスの連絡先</span><span class="sxs-lookup"><span data-stu-id="2b430-103">Process contacts in batches by using EWS in Exchange</span></span>

<span data-ttu-id="2b430-104">Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで連絡先の作成、取得、更新、削除をバッチ処理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b430-104">Learn how to create, get, update, and delete batches of contacts in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2b430-105">EWS のマネージ API を使用することができます。 または EWS 呼び出しの数を減らすには、取引先担当者のバッチがクライアントを使用すると、Exchange サーバーにします。</span><span class="sxs-lookup"><span data-stu-id="2b430-105">You can use the EWS Managed API or EWS to work with batches of contacts to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="2b430-106">EWS のマネージ API を使用して、作成、取得、更新、およびバッチ内の連絡先を削除する[連絡先](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用する 1 つの連絡先を使用するときに、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="2b430-106">When you use the EWS Managed API to create, get, update, and delete contacts in batches, you use [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single contacts, you use [Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="2b430-107">EWS を使用する場合は、1 つの取引先担当者と取引先担当者のバッチの両方で動作する同じ操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="2b430-107">If you are using EWS, you use the same operations to work with both a single contact and batches of contacts.</span></span> 
  
<span data-ttu-id="2b430-108">**表 1 です。EWS のマネージ API のメソッドとメンバーのバッチを処理するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="2b430-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of contacts**</span></span>

|<span data-ttu-id="2b430-109">**目的…**</span><span class="sxs-lookup"><span data-stu-id="2b430-109">**In order to…**</span></span>|<span data-ttu-id="2b430-110">**この EWS 管理 API メソッドを使用します。**</span><span class="sxs-lookup"><span data-stu-id="2b430-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="2b430-111">**EWS 操作を使用します。**</span><span class="sxs-lookup"><span data-stu-id="2b430-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2b430-112">バッチ処理による連絡先の作成</span><span class="sxs-lookup"><span data-stu-id="2b430-112">Create contacts in batches</span></span>  <br/> |[<span data-ttu-id="2b430-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="2b430-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2b430-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="2b430-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2b430-115">バッチ処理による連絡先の取得</span><span class="sxs-lookup"><span data-stu-id="2b430-115">Get contacts in batches</span></span>  <br/> |<span data-ttu-id="2b430-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx)または[ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="2b430-116">[ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) or [ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="2b430-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="2b430-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2b430-118">バッチ処理による連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="2b430-118">Update contacts in batches</span></span>  <br/> |[<span data-ttu-id="2b430-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="2b430-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2b430-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2b430-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="2b430-121">バッチ処理による連絡先の削除</span><span class="sxs-lookup"><span data-stu-id="2b430-121">Delete contacts in batches</span></span>  <br/> |[<span data-ttu-id="2b430-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="2b430-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2b430-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="2b430-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="2b430-124">この記事では、EWS のマネージ API または EWS を使用して連絡先のバッチのための基本的なタスクを完了する方法について学習します。</span><span class="sxs-lookup"><span data-stu-id="2b430-124">In this article, you'll learn how to complete basic tasks for batches of contacts by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2b430-125">EWS マネージ API を使用してバッチ処理で連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="2b430-125">Create contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2b430-126"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-126"></span></span>

<span data-ttu-id="2b430-127">次の例のように、マネージ API の EWS [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で連絡先を作成できます。</span><span class="sxs-lookup"><span data-stu-id="2b430-127">You can create contacts in batches by using the EWS Managed API [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="2b430-128">次の使用例を作成 3 つの[連絡先](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトをローカルにしてそれぞれの連絡先は、コレクションに追加、連絡先のコレクションで**CreateItems**メソッドを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="2b430-128">This example creates three [Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) objects locally, adds each contact to a collection, then calls the **CreateItems** method on the collection of contacts.</span></span> 
  
```cs
public static Collection<ItemId> CreateContactsInBatch(ExchangeService service)
{
    // These are unsaved local instances of a Contact object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Contact contact1 = new Contact(service);
    Contact contact2 = new Contact(service);
    Contact contact3 = new Contact(service);
    // Set the properties on the first contact.
    contact1.DisplayName = "Sadie Daniels";
    contact1.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("sadie@contoso.com");
    
    // Set the properties on the second contact.
    contact2.DisplayName = "Alfred Welker";
    contact2.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("alfred@contoso.com");
    // Set the properties on the third contact.
    contact3.DisplayName = "Hope Gross";
    contact3.EmailAddresses[EmailAddressKey.EmailAddress1] = new EmailAddress("hope@contoso.com");
    // Add the Contact objects to a collection.
    Collection<Contact> contactItems = new Collection<Contact>() { contact1, contact2, contact3 };
    // Create the batch of contacts on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(contactItems, WellKnownFolderName.Contacts, null, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created contacts.
    foreach (Contact contact in contactItems)
    {
        try
        {
            itemIds.Add(contact.Id);
            Console.WriteLine("Contact '{0}' created successfully.", contact.DisplayName);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating contact {0}: {1}", contact.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Determine whether the CreateItems method call completed successfully.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created contacts were successfully created in the Contacts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each contact.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (contact {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

## <a name="create-contacts-in-batches-by-using-ews"></a><span data-ttu-id="2b430-129">EWS を使用してバッチ処理で連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="2b430-129">Create contacts in batches by using EWS</span></span>
<span data-ttu-id="2b430-130"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-130"></span></span>

<span data-ttu-id="2b430-131">コード例を次に示すように、 [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS 操作を使用してバッチ処理で連絡先を作成できます。</span><span class="sxs-lookup"><span data-stu-id="2b430-131">You can create contacts in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="2b430-132">EWS のマネージ API が[バッチ内の連絡先を作成](#bk_EWSMA)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="2b430-132">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create contacts in batches](#bk_EWSMA).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:CreateItem>
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:Items>
          <t:Contact>
            <t:DisplayName>Sadie Daniels</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">sadie@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Alfred Welker</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">alfred@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
          <t:Contact>
            <t:DisplayName>Hope Gross</t:DisplayName>
            <t:EmailAddresses>
              <t:Entry Key="EmailAddress1">hope@contoso.com</t:Entry>
            </t:EmailAddresses>
          </t:Contact>
        </m:Items>
      </m:CreateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="2b430-133">サーバー要求に応答し、 **CreateItem** **NoError**の[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値を含む、新しい取引先担当者、各連絡先が作成され、保存されたことを示すに[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージを正常にします。</span><span class="sxs-lookup"><span data-stu-id="2b430-133">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new contacts, which indicates that each contact was created and saved successfully.</span></span> 
  
## <a name="get-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2b430-134">EWS マネージ API を使用してバッチ処理で連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="2b430-134">Get contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2b430-135"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-135"></span></span>

<span data-ttu-id="2b430-136">次の例のように、EWS のマネージ API の[BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="2b430-136">You can get contacts in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="2b430-137">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2b430-137">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchGetContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Create a property set that limits the properties returned by the Bind method to only those that are required.
            PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ContactSchema.DisplayName);
            // Get the items from the server.
            // This method call results in a GetItem call to EWS.
            ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
            // Instantiate a collection of Contact objects to populate from the values that are returned by the Exchange server.
            Collection<Contact> contactItems = new Collection<Contact>();
            foreach (GetItemResponse getItemResponse in response)
            {
                try
                {
                    Item item = getItemResponse.Item;
                    Contact contact = (Contact)item;
                    contactItems.Add(contact);
                    // Print out confirmation and the last eight characters of the item ID.
                    Console.WriteLine("Found item {0}.", contact.Id.ToString().Substring(144));
                }
                catch (Exception ex)
                {
                    Console.WriteLine("Exception while getting a contact: {0}", ex.Message);
                }
            }
            // Check for success of the BindToItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts retrieved successfully.");
                Console.WriteLine("\r\n");
            }
            return contactItems;
        }

```

## <a name="get-contacts-in-batches-by-using-ews"></a><span data-ttu-id="2b430-138">EWS を使用してバッチ処理で連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="2b430-138">Get contacts in batches by using EWS</span></span>
<span data-ttu-id="2b430-139"><a name="bk_EWSMAGet"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-139"></span></span>

<span data-ttu-id="2b430-140">次の例では、 [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作とコードを使用してバッチ処理での連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="2b430-140">You can get contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="2b430-141">EWS のマネージ API が[バッチ内の連絡先を取得](#bk_EWSMAGet)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="2b430-141">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get contacts in batches](#bk_EWSMAGet).</span></span> <span data-ttu-id="2b430-142">**ItemId**属性が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="2b430-142">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetItem>
        <m:ItemShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="contacts:DisplayName" />
          </t:AdditionalProperties>
        </m:ItemShape>
        <m:ItemIds>
          <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
          <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
          <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
        </m:ItemIds>
      </m:GetItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="2b430-143">サーバーは、ID、要求された取引先担当者のそれぞれの表示名を含む[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx)メッセージの**GetItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="2b430-143">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the ID and the display name for each of the requested contacts.</span></span> 
  
## <a name="update-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2b430-144">EWS マネージ API を使用してバッチ処理で連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="2b430-144">Update contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2b430-145"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-145"></span></span>

<span data-ttu-id="2b430-146">、EWS のマネージ API の[UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx)メソッドを使用してバッチ内の連絡先を更新するには、次の例のようにします。</span><span class="sxs-lookup"><span data-stu-id="2b430-146">You can update contacts in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> <span data-ttu-id="2b430-147">前の例では、連絡先を作成しますで働くが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="2b430-147">The previous example creates the contact but does not specify who they work for.</span></span> <span data-ttu-id="2b430-148">この例では、コードを使用するには、会社名は、同時にすべての連絡先を更新します。</span><span class="sxs-lookup"><span data-stu-id="2b430-148">You can use the code in this example to update all your contacts at once to include their company name.</span></span> 
  
<span data-ttu-id="2b430-149">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2b430-149">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<Contact> BatchUpdateContactItems(ExchangeService service, Collection<Contact> contactItems)
        {
            // Update the company name of each contact locally.
            foreach (Contact contact in contactItems)
            {
                // Update the company name of the contact.
                contact.CompanyName = "Contoso";
                // Print out confirmation with the last eight characters of the item ID and the contact company name.
                Console.WriteLine("Updated local contact {0} with the company name '{1}'.", contact.Id.ToString().Substring(144), contact.CompanyName);
            }
            
            // Send the item updates to the server.
            // This method call results in an UpdateItem call to EWS.
            ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(contactItems, WellKnownFolderName.Contacts, ConflictResolutionMode.AutoResolve, null, null);
            // Verify the success of the UpdateItems method call.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("All contacts updated successfully.\r\n");
            }
            // If the method did not return success, print the result message for each contact.
            else
            {
                Console.WriteLine("All contacts were not successfully saved on the server.\r\n");
                int counter = 1;
                foreach (ServiceResponse resp in response)
                {
                    Console.WriteLine("Result for (contact {0}): {1}", counter, resp.Result);
                    Console.WriteLine("Error Code: {0}", resp.ErrorCode);
                    Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
                    counter++;
                }
            }
            return contactItems;
        }    

```

## <a name="update-contacts-in-batches-by-using-ews"></a><span data-ttu-id="2b430-150">EWS を使用してバッチ処理で連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="2b430-150">Update contacts in batches by using EWS</span></span>
<span data-ttu-id="2b430-151"><a name="bk_EWSMAUpdate"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-151"></span></span>

<span data-ttu-id="2b430-152">[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作を使用してバッチ内の連絡先を更新するには、次のコード例に示すように。</span><span class="sxs-lookup"><span data-stu-id="2b430-152">You can update contacts in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="2b430-153">EWS のマネージ API が[バッチ内の連絡先を更新](#bk_EWSMAUpdate)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="2b430-153">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update contacts in batches](#bk_EWSMAUpdate).</span></span> <span data-ttu-id="2b430-154">**ItemId**属性が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="2b430-154">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:UpdateItem ConflictResolution="AutoResolve">
        <m:SavedItemFolderId>
          <t:DistinguishedFolderId Id="contacts" />
        </m:SavedItemFolderId>
        <m:ItemChanges>
          <t:ItemChange>
            <t:ItemId Id="ceJwVAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yS" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwWAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yT" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
          <t:ItemChange>
            <t:ItemId Id="ceJwXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yU" />
            <t:Updates>
              <t:SetItemField>
                <t:FieldURI FieldURI="contacts:CompanyName" />
                <t:Contact>
                  <t:CompanyName>Contoso</t:CompanyName>
                </t:Contact>
              </t:SetItemField>
            </t:Updates>
          </t:ItemChange>
        </m:ItemChanges>
      </m:UpdateItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="2b430-155">サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、更新プログラムのそれぞれのサーバー上でが正常に保存されたことを示す値を含む、 [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx)メッセージの**UpdateItem**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="2b430-155">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="2b430-156">[ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx)要素内での競合が報告されます。</span><span class="sxs-lookup"><span data-stu-id="2b430-156">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-contacts-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="2b430-157">EWS マネージ API を使用してバッチ処理で連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="2b430-157">Delete contacts in batches by using the EWS Managed API</span></span>
<span data-ttu-id="2b430-158"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-158"></span></span>

<span data-ttu-id="2b430-159">[DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) EWS 管理 API メソッドを使用してバッチ内の連絡先を削除するには、次の例に示すように。</span><span class="sxs-lookup"><span data-stu-id="2b430-159">You can delete contacts in batches by using the [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="2b430-160">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="2b430-160">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void BatchDeleteContactItems(ExchangeService service, Collection<ItemId> itemIds)
        {
            // Delete the batch of contact objects.
            // This method call results in an DeleteItem call to EWS.
            ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
            // Check for success of the DeleteItems method call.
            // DeleteItems returns success even if it does not find all the item IDs.
            if (response.OverallResult == ServiceResult.Success)
            {
                Console.WriteLine("Contacts deleted successfully.\r\n");
            }
            // If the method did not return success, print a message.
            else
            {
                Console.WriteLine("Not all contacts deleted successfully.\r\n");
            }
        }

```

## <a name="delete-contacts-in-batches-by-using-ews"></a><span data-ttu-id="2b430-161">EWS を使用してバッチ処理で連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="2b430-161">Delete contacts in batches by using EWS</span></span>
<span data-ttu-id="2b430-162"><a name="bk_EWSMADelete"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-162"></span></span>

<span data-ttu-id="2b430-163">[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS 操作を使用してバッチ内の連絡先を削除するには、次のコード例に示すように。</span><span class="sxs-lookup"><span data-stu-id="2b430-163">You can delete contacts in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="2b430-164">EWS のマネージ API が[バッチ内の連絡先を削除](#bk_EWSMADelete)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="2b430-164">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete contacts in batches](#bk_EWSMADelete).</span></span> <span data-ttu-id="2b430-165">**ItemId**属性が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="2b430-165">The **ItemId** attribute has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:DeleteItem DeleteType="SoftDelete" AffectedTaskOccurrences="AllOccurrences">
        <m:ItemIds>
          <t:ItemId Id="ceJwYAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yY" />
          <t:ItemId Id="ceJwZAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51yZ" />
          <t:ItemId Id="ceJwaAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AAFc51ya" />
        </m:ItemIds>
      </m:DeleteItem>
    </soap:Body>
  </soap:Envelope>
```

<span data-ttu-id="2b430-166">サーバー要求に応答、 **DeleteItem** **NoError**の削除された項目ごとに[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値を含む[DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx)のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="2b430-166">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="2b430-167">返す成功アイテム ID が見つかりませんだった場合に注意してください。</span><span class="sxs-lookup"><span data-stu-id="2b430-167">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="2b430-168">バッチ処理が正常に完了したことを確認する</span><span class="sxs-lookup"><span data-stu-id="2b430-168">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="2b430-169"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="2b430-169"></span></span>

<span data-ttu-id="2b430-p112">バッチ要求された 1 つ以上の連絡先を要求どおりに処理できないと、失敗した連絡先ごとにエラーが返されます。バッチ処理のそれ以外の連絡先は予期したとおりに処理されます。対象アイテムが削除されたために取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更を行えなったりすると、バッチ処理でエラーが生じます。このセクションの情報には、連絡先のバッチ処理で生じたエラーの詳細を取得する方法が示されています。</span><span class="sxs-lookup"><span data-stu-id="2b430-p112">When one or more contacts in a batched request can't be processed as requested, an error is returned for each contact that failed, and the rest of the contacts in the batch are processed as expected. Failures in batch processing can occur if the item was deleted, and therefore can't be retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent. The information in this section shows how to get error details about failures in batch processing of contacts.</span></span>
  
<span data-ttu-id="2b430-173">EWS のマネージ API を使用して、バッチ処理の成功を確認するには、 [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx)の[OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx)プロパティが[ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx)に等しいかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="2b430-173">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="2b430-174">その場合は、すべての連絡先が正常に処理されました。</span><span class="sxs-lookup"><span data-stu-id="2b430-174">If so, all the contacts were processed successfully.</span></span> <span data-ttu-id="2b430-175">**OverallResult**が**ServiceResult.Success**、1 つまたは複数の連絡先と同じでない場合は、正常に処理されませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b430-175">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the contacts were not processed successfully.</span></span> <span data-ttu-id="2b430-176">**ServiceResponseCollection**で返されるオブジェクトの各には、次のプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2b430-176">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="2b430-177">エラー コード</span><span class="sxs-lookup"><span data-stu-id="2b430-177">ErrorCode</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="2b430-178">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="2b430-178">ErrorDetails</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="2b430-179">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="2b430-179">ErrorMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="2b430-180">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="2b430-180">ErrorProperties</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="2b430-181">結果</span><span class="sxs-lookup"><span data-stu-id="2b430-181">Result</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="2b430-182">これらのプロパティには、なぜ連絡先を処理できませんでした要求に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b430-182">These properties contain information about why the contacts could not be processed as requested.</span></span> <span data-ttu-id="2b430-183">この資料の例の出力**結果**、**エラー コード**とそれぞれの**エラー メッセージ**に連絡先が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="2b430-183">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed contact.</span></span> <span data-ttu-id="2b430-184">これらの結果を使用すると、問題を調査します。</span><span class="sxs-lookup"><span data-stu-id="2b430-184">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="2b430-185">EWS では、バッチ処理の成功を確認するには、処理中の各項目の[ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx)属性を確認します。</span><span class="sxs-lookup"><span data-stu-id="2b430-185">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="2b430-186">**ResponseMessageType**、するすべての応答メッセージの派生元の基本型の基本構造を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b430-186">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="2b430-187">**ResponseClass**属性は、連絡先が正常に処理されなかった場合に、連絡先が正常に処理された場合の**成功**または**エラー**に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2b430-187">The **ResponseClass** attribute is set to **Success** if the contact was processed successfully, or **Error** if the contact was not processed successfully.</span></span> <span data-ttu-id="2b430-188">連絡先、バッチ処理中に**警告**は発生しません。</span><span class="sxs-lookup"><span data-stu-id="2b430-188">For contacts, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="2b430-189">**ResponseClass**が**成功**の場合は、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の後も常に**NoError**に設定されています。</span><span class="sxs-lookup"><span data-stu-id="2b430-189">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="2b430-190">**ResponseClass**が**エラー**の場合は、問題の原因を特定するのには、[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、 **ResponseCode**、および[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx)の要素の値を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b430-190">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="2b430-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx)は、現在使用されていません。</span><span class="sxs-lookup"><span data-stu-id="2b430-191">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2b430-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b430-192">See also</span></span>


- [<span data-ttu-id="2b430-193">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="2b430-193">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="2b430-194">電子メール メッセージを Exchange で EWS を使用してバッチ プロセス</span><span class="sxs-lookup"><span data-stu-id="2b430-194">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="2b430-195">Exchange 予定表のアイテムをまとめてを処理します。</span><span class="sxs-lookup"><span data-stu-id="2b430-195">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    

