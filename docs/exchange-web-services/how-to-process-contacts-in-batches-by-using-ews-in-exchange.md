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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759046"
---
# <a name="process-contacts-in-batches-by-using-ews-in-exchange"></a>Exchange EWS を使用してバッチ プロセスの連絡先

Exchange で EWS マネージ API または EWS を使用して、1 回の呼び出しで連絡先の作成、取得、更新、削除をバッチ処理する方法について説明します。
  
EWS のマネージ API を使用することができます。 または EWS 呼び出しの数を減らすには、取引先担当者のバッチがクライアントを使用すると、Exchange サーバーにします。 EWS のマネージ API を使用して、作成、取得、更新、およびバッチ内の連絡先を削除する[連絡先](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用する 1 つの連絡先を使用するときに、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトのメソッドを使用します。 EWS を使用する場合は、1 つの取引先担当者と取引先担当者のバッチの両方で動作する同じ操作を使用します。 
  
**表 1 です。EWS のマネージ API のメソッドとメンバーのバッチを処理するための EWS の操作**

|**目的…**|**この EWS 管理 API メソッドを使用します。**|**EWS 操作を使用します。**|
|:-----|:-----|:-----|
|バッチ処理による連絡先の作成  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|バッチ処理による連絡先の取得  <br/> |[ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx)または[ExchangeService.LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|バッチ処理による連絡先の更新  <br/> |[ExchangeService.UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|バッチ処理による連絡先の削除  <br/> |[ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
この記事では、EWS のマネージ API または EWS を使用して連絡先のバッチのための基本的なタスクを完了する方法について学習します。
  
## <a name="create-contacts-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で連絡先を作成する
<a name="bk_EWSMA"> </a>

次の例のように、マネージ API の EWS [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で連絡先を作成できます。 次の使用例を作成 3 つの[連絡先](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトをローカルにしてそれぞれの連絡先は、コレクションに追加、連絡先のコレクションで**CreateItems**メソッドを呼び出します。 
  
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

## <a name="create-contacts-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で連絡先を作成する
<a name="bk_EWSMA"> </a>

コード例を次に示すように、 [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS 操作を使用してバッチ処理で連絡先を作成できます。 EWS のマネージ API が[バッチ内の連絡先を作成](#bk_EWSMA)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。
  
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

サーバー要求に応答し、 **CreateItem** **NoError**の[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値を含む、新しい取引先担当者、各連絡先が作成され、保存されたことを示すに[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージを正常にします。 
  
## <a name="get-contacts-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で連絡先を取得する
<a name="bk_EWSMAGet"> </a>

次の例のように、EWS のマネージ API の[BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx)メソッドを使用してバッチ処理で連絡先を取得できます。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="get-contacts-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で連絡先を取得する
<a name="bk_EWSMAGet"> </a>

次の例では、 [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作とコードを使用してバッチ処理での連絡先を取得できます。 EWS のマネージ API が[バッチ内の連絡先を取得](#bk_EWSMAGet)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。 **ItemId**属性が小さすぎると読みやすくするためです。 
  
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

サーバーは、ID、要求された取引先担当者のそれぞれの表示名を含む[GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx)メッセージの**GetItem**要求に応答します。 
  
## <a name="update-contacts-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で連絡先を更新する
<a name="bk_EWSMAUpdate"> </a>

、EWS のマネージ API の[UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx)メソッドを使用してバッチ内の連絡先を更新するには、次の例のようにします。 前の例では、連絡先を作成しますで働くが指定されていません。 この例では、コードを使用するには、会社名は、同時にすべての連絡先を更新します。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="update-contacts-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で連絡先を更新する
<a name="bk_EWSMAUpdate"> </a>

[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS 操作を使用してバッチ内の連絡先を更新するには、次のコード例に示すように。 EWS のマネージ API が[バッチ内の連絡先を更新](#bk_EWSMAUpdate)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。 **ItemId**属性が小さすぎると読みやすくするためです。 
  
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

サーバーは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**、更新プログラムのそれぞれのサーバー上でが正常に保存されたことを示す値を含む、 [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx)メッセージの**UpdateItem**要求に応答します。 [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx)要素内での競合が報告されます。 
  
## <a name="delete-contacts-in-batches-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してバッチ処理で連絡先を削除する
<a name="bk_EWSMADelete"> </a>

[DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) EWS 管理 API メソッドを使用してバッチ内の連絡先を削除するには、次の例に示すように。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

## <a name="delete-contacts-in-batches-by-using-ews"></a>EWS を使用してバッチ処理で連絡先を削除する
<a name="bk_EWSMADelete"> </a>

[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS 操作を使用してバッチ内の連絡先を削除するには、次のコード例に示すように。 EWS のマネージ API が[バッチ内の連絡先を削除](#bk_EWSMADelete)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。 **ItemId**属性が小さすぎると読みやすくするためです。 
  
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

サーバー要求に応答、 **DeleteItem** **NoError**の削除された項目ごとに[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)値を含む[DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx)のメッセージです。 返す成功アイテム ID が見つかりませんだった場合に注意してください。 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a>バッチ処理が正常に完了したことを確認する
<a name="bk_successful"> </a>

バッチ要求された 1 つ以上の連絡先を要求どおりに処理できないと、失敗した連絡先ごとにエラーが返されます。バッチ処理のそれ以外の連絡先は予期したとおりに処理されます。対象アイテムが削除されたために取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなり、送信されたアイテム ID で変更を行えなったりすると、バッチ処理でエラーが生じます。このセクションの情報には、連絡先のバッチ処理で生じたエラーの詳細を取得する方法が示されています。
  
EWS のマネージ API を使用して、バッチ処理の成功を確認するには、 [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx)の[OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx)プロパティが[ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx)に等しいかを確認できます。 その場合は、すべての連絡先が正常に処理されました。 **OverallResult**が**ServiceResult.Success**、1 つまたは複数の連絡先と同じでない場合は、正常に処理されませんでした。 **ServiceResponseCollection**で返されるオブジェクトの各には、次のプロパティが含まれます。 
  
- [エラー コード](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [エラー メッセージ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [結果](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
これらのプロパティには、なぜ連絡先を処理できませんでした要求に関する情報が含まれています。 この資料の例の出力**結果**、**エラー コード**とそれぞれの**エラー メッセージ**に連絡先が失敗しました。 これらの結果を使用すると、問題を調査します。 
  
EWS では、バッチ処理の成功を確認するには、処理中の各項目の[ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx)属性を確認します。 **ResponseMessageType**、するすべての応答メッセージの派生元の基本型の基本構造を次に示します。 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

**ResponseClass**属性は、連絡先が正常に処理されなかった場合に、連絡先が正常に処理された場合の**成功**または**エラー**に設定されます。 連絡先、バッチ処理中に**警告**は発生しません。 **ResponseClass**が**成功**の場合は、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の後も常に**NoError**に設定されています。 **ResponseClass**が**エラー**の場合は、問題の原因を特定するのには、[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)、 **ResponseCode**、および[MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx)の要素の値を確認する必要があります。 [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx)は、現在使用されていません。 
  
## <a name="see-also"></a>関連項目


- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)
    
- [電子メール メッセージを Exchange で EWS を使用してバッチ プロセス](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
- [Exchange 予定表のアイテムをまとめてを処理します。](how-to-process-calendar-items-in-batches-in-exchange.md)
    

