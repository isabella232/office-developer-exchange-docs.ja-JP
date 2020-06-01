---
title: Exchange で EWS を使用して永続的なアプリケーションの設定を管理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Exchange で EWS マネージ API または EWS を使用して、永続的なアプリケーションの設定を作成、検索、取得、更新、削除する方法について説明します。
ms.openlocfilehash: ab7b3ef5f87d8a26a412ca7187dc93c58d73112f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455731"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="74b05-103">Exchange で EWS を使用して永続的なアプリケーションの設定を管理する</span><span class="sxs-lookup"><span data-stu-id="74b05-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="74b05-104">Exchange で EWS マネージ API または EWS を使用して、永続的なアプリケーションの設定を作成、検索、取得、更新、削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="74b05-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="74b05-105">ユーザー構成オブジェクトが Exchange クライアント アプリケーションの構成設定を保存するための最適なオプションであるといえる主な理由は、ほとんどのクライアント アプリケーションでこれらの設定が検索結果から隠されるためです。</span><span class="sxs-lookup"><span data-stu-id="74b05-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="74b05-106">通常、クライアント アプリケーションはこれらの設定を非表示にします。これは、エンド ユーザーがこれらの設定を確認する必要がないため、またユーザーがこの情報に誤ってアクセスしないようにするためです。</span><span class="sxs-lookup"><span data-stu-id="74b05-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="74b05-107">この記事のコード例は、永続的な設定を管理するためにユーザー構成オブジェクトを使用する方法を示しています。それには、ユーザー構成オブジェクトに保存されている永続的なアプリケーションの設定を作成、検索、取得、更新および削除する方法が含まれます。</span><span class="sxs-lookup"><span data-stu-id="74b05-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="74b05-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-108"><a name="createconfiguration"> </a></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="74b05-109">EWS マネージ API を使用してアプリケーション設定を作成する</span><span class="sxs-lookup"><span data-stu-id="74b05-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="74b05-110">EWS マネージ API の [UserConfiguration.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) メソッドを使用して、カスタム構成設定を作成できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-110">You can use the [UserConfiguration.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="74b05-111">ユーザー構成オブジェクトには、XML、バイナリ、データ辞書、またはこれらの 3 つのデータ型の組み合わせを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="74b05-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="74b05-112">次の例では、EWS マネージ API を使用して、バイナリ データを含む ContosoDraftSettings という名前のユーザー構成オブジェクトを下書きフォルダーに保存する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="74b05-113">これは、下書きアイテムを表示する方法に関する構成情報をクライアント アプリケーションに保存する場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="74b05-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
```cs
private static void CreateUserConfiguration(ExchangeService service, byte[] binaryData)
{
    // Create the user configuration object.
    UserConfiguration configDrafts = new UserConfiguration(service);
    // Add user configuration data to the BinaryData property.
    configDrafts.BinaryData = binaryData;
    // Name and save the user configuration object on the Drafts folder.
    // This results in a call to EWS.
    configDrafts.Save("ContosoDraftSettings", WellKnownFolderName.Drafts);
}
```

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="74b05-114">EWS を使用してアプリケーション設定を作成する</span><span class="sxs-lookup"><span data-stu-id="74b05-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="74b05-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-115"><a name="bk_createEWS"> </a></span></span>

<span data-ttu-id="74b05-p103">EWS の [CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) 操作を使用して、カスタム構成設定を作成できます。次の例は、ContosoDraftSettings という名前のユーザー構成オブジェクトを作成するための要求 XML を示しています。この要求は、バイナリ ストリームを下書きフォルダーのユーザー構成オブジェクトに保存しようとします。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="74b05-p103">You can use the [CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting. The following example shows the request XML for creating a user configuration object named ContosoDraftSettings. The request attempts to save a binary stream to a user configuration object on the Drafts folder. This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="ContosoDraftSettings">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:BinaryData>iVBORw0KGH5UhKquRSzaeAAAAAElFTkSuQmCC</t:BinaryData>
      </m:UserConfiguration>
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74b05-120">[応答 XML](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) は単純なものであり、作成要求が成功したか、またはエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-120">The [response XML](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="74b05-121">EWS マネージ API を使用してアプリケーション設定を検索する</span><span class="sxs-lookup"><span data-stu-id="74b05-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="74b05-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-122"><a name="findconfiguration"> </a></span></span>

<span data-ttu-id="74b05-123">関連付けられているトラバーサル オプションと共に EWS マネージ API の [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) メソッドを使用して、ユーザー構成オブジェクトを検索できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-123">You can use the [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="74b05-124">次のコード例では、EWS マネージ API を使用して、下書きフォルダーに保存されているユーザー構成オブジェクトを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
```cs
private static void FindAssociated(ExchangeService service)
{
    // This is the ItemClass prefix of user configuration objects that are created by using EWS.
    const string userConfigPrefix = "IPM.Configuration.";
            
    // This is the name of a configuration setting created by using EWS.
    string userConfigName = "TestConfig";
    // Return the first five items. 
    ItemView view = new ItemView(5);
    // Request only the properties that you need. Because all the results will be user configuration 
    // objects, you won't need to request the ItemSchema.IsAssociated property, which identifies 
    // user configuration objects.
    PropertySet props = new PropertySet(BasePropertySet.IdOnly, 
                                        ItemSchema.ItemClass);
    view.PropertySet = props;
            
    // Set the traversal to find user configuration objects. 
    view.Traversal = ItemTraversal.Associated;
    // Send the request to search the Drafts folder for all the user configuration objects 
    // in the folder. You do not have to use a search restriction because you will not return
    // a large number of search results. For this scenario, it is better to sort the results
    // on the client. This method results in a call to EWS.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Drafts, view);
    // Output a list of the item classes for the associated items. 
    foreach (Item item in findResults)
    {
        if (item.ItemClass == userConfigPrefix + userConfigName)
        {
            Console.WriteLine("You found the configuration: " + userConfigPrefix + userConfigName);
        }
    }
}
```

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="74b05-125">EWS を使用してアプリケーション設定を検索する</span><span class="sxs-lookup"><span data-stu-id="74b05-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="74b05-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-126"><a name="bk_findEWS"> </a></span></span>

<span data-ttu-id="74b05-127">EWS の [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、ユーザー構成オブジェクトを検索できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-127">You can use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="74b05-p105">次の例は、ユーザー構成オブジェクトを検索するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="74b05-p105">The following example shows the request XML for finding user configuration objects. This is the same XML that is generated by the EWS Managed API example.</span></span>
  
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
    <m:FindItem Traversal="Associated">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemClass" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="5" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="drafts" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74b05-p106">次の例は、ユーザー構成オブジェクトの検索が成功した場合の応答 XML を示しています。これは、EWS マネージ API の例で処理されるものと同じ XML です。この応答 XML では次の点に注意してください。 </span><span class="sxs-lookup"><span data-stu-id="74b05-p106">The following example shows the successful response XML for finding user configuration objects. This is the same XML that is processed by the EWS Managed API example. Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="74b05-133">読みやすいように識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="74b05-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="74b05-134">メッセージとして 2 つのユーザー構成オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="74b05-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="74b05-135">これは、**FindItem** 操作がメッセージ アイテムとして EWS スキーマで定義されていないすべてのアイテムを返すためです。</span><span class="sxs-lookup"><span data-stu-id="74b05-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="74b05-136">2 つのユーザー構成オブジェクトでは、[ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) プロパティが異なります。</span><span class="sxs-lookup"><span data-stu-id="74b05-136">The [ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="74b05-137">最初のユーザー構成オブジェクトは、EWS を使用して作成されました。</span><span class="sxs-lookup"><span data-stu-id="74b05-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="74b05-138">2 番目のオブジェクトは、他の API によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="74b05-138">The second object was created by another API.</span></span> 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" 
                        TotalItemsInView="2" 
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
                <t:ItemClass>IPM.Configuration.TestConfig</t:ItemClass>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAkADEzOzFAAA=" ChangeKey="CQAAABQAAABAByOw==" />
                <t:ItemClass>IPM.Microsoft.FolderDesign.NamedView</t:ItemClass>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="74b05-139">EWS マネージ API を使用してアプリケーション設定を取得して更新する</span><span class="sxs-lookup"><span data-stu-id="74b05-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="74b05-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-140"><a name="getconfiguration"> </a></span></span>

<span data-ttu-id="74b05-141">ユーザー構成オブジェクトの検索後、EWS マネージ API の [UserConfiguration.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) メソッドを使用して、メールボックスから構成オブジェクトを取得できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="74b05-142">構成オブジェクトを取得すると、[UserConfiguration.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) メソッドを使用して、それを更新できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-142">After you get the configuration object, you can use the [UserConfiguration.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="74b05-143">次の例では、EWS マネージ API を使用して、ユーザー構成オブジェクトを取得して更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void GetAndUpdateUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object named "TestConfig" in the user's mailbox. 
    // Results in a call to EWS. You can also use the Load method to get the latest
    // server version of the user configuration object.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                         "TestConfig",
                                                         WellKnownFolderName.Drafts,
                                                         UserConfigurationProperties.All);
            
    // Display the returned configuration object property values.
    if (usrConfig.XmlData != null)
    {
        Console.WriteLine("XmlData: " + Encoding.UTF8.GetString(usrConfig.XmlData));
    }
    if (usrConfig.BinaryData != null)
    {
        Console.WriteLine("BinaryData: " + Encoding.UTF8.GetString(usrConfig.BinaryData));
    }
    if (usrConfig.Dictionary.Count > 0)
    {
        Console.WriteLine("Contains {0} dictionary entries", usrConfig.Dictionary.Count);
    }
    // Add dictionary property values to the local copy of the object.
    usrConfig.Dictionary.Add("Key5", 1);
    // Updates the server version of the user configuration object 
    // if it has changed on the client. Results in a call to EWS.
    if (usrConfig.IsDirty)
    {
        usrConfig.Update();
    }
}
```

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="74b05-144">EWS を使用してアプリケーション設定を取得して更新する</span><span class="sxs-lookup"><span data-stu-id="74b05-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="74b05-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-145"><a name="bk_getEWS"> </a></span></span>

<span data-ttu-id="74b05-p110">EWS の [GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) 操作を使用して、メールボックスから構成オブジェクトを取得できます。また [UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) を使用してオブジェクトを更新できます。次の例は、TestConfig という名前のユーザー構成オブジェクトを取得するための要求 XML を示しています。この要求は、すべての構成を応答で返す必要があることを示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="74b05-p110">You can use the [GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object. The following example shows the request XML for getting a user configuration object named TestConfig. The request states that all configurations should be returned in the response. This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74b05-p111">次の例は、ユーザー構成オブジェクトの取得が成功した場合の応答 XML を示しています。応答にはデータ辞書が含まれます。これは、EWS マネージ API の例で処理されるものと同じ XML です。 </span><span class="sxs-lookup"><span data-stu-id="74b05-p111">The following example shows the successful response XML for getting a user configuration objects. The response contains a data dictionary. This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts" />
            </t:UserConfigurationName>
            <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>Key1</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>Integer32</t:Type>
                  <t:Value>1</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="74b05-153">次の例は、ユーザー構成オブジェクトを更新するための要求 XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="74b05-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="74b05-154">この要求は、すべての構成を応答で返す必要があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="74b05-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="74b05-155">これは、**UserConfiguration.Update** メソッドを呼び出す EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="74b05-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="74b05-156">更新 XML に既存の辞書エントリと、更新前に追加された他の 1 つの辞書エントリが含まれていることが確認できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key1</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key5</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74b05-157">[応答 XML](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) は単純なものであり、更新が成功したかまたはエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-157">The [response XML](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="74b05-158">EWS マネージ API を使用してアプリケーション設定を削除する</span><span class="sxs-lookup"><span data-stu-id="74b05-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="74b05-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-159"><a name="deleteconfiguration"> </a></span></span>

<span data-ttu-id="74b05-160">EWS マネージ API の [UserConfiguration.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) メソッドを使用して、ユーザー構成オブジェクトを削除できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-160">You can use the [UserConfiguration.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="74b05-161">次のコード例は、EWS マネージ API を使用して、ユーザー構成オブジェクト ContosoDraftSettings を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void DeleteUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object. Results in a call to EWS.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                        "ContosoDraftSettings",
                                                        WellKnownFolderName.Drafts,
                                                        UserConfigurationProperties.Id);
    // Deletes the user configuration object.
    // Results in a call to EWS.
    usrConfig.Delete();
}
```

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="74b05-162">EWS を使用してアプリケーション設定を削除する</span><span class="sxs-lookup"><span data-stu-id="74b05-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="74b05-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="74b05-163"><a name="bk_deleteEWS"> </a></span></span>

<span data-ttu-id="74b05-164">EWS の [DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) 操作を使用して、ユーザー構成オブジェクトを削除できます。</span><span class="sxs-lookup"><span data-stu-id="74b05-164">You can use the [DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="74b05-p114">次の例は、下書きフォルダーに適用されていた ContosoDraftSettings という名前のユーザー構成オブジェクトを削除するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="74b05-p114">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder. This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="ContosoDraftSettings">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="74b05-167">[応答 XML](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) は単純なものであり、削除要求が成功したかエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74b05-167">The [response XML](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="74b05-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="74b05-168">See also</span></span>

- [<span data-ttu-id="74b05-169">Exchange の EWS の永続的なアプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="74b05-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="74b05-170">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="74b05-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="74b05-171">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="74b05-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

