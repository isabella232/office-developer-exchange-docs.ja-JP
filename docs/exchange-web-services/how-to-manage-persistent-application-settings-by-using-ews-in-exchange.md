---
title: EWS を使用して Exchange 内で永続的なアプリケーションの設定を管理します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: 'Exchange で EWS マネージ API または EWS を使用して、永続的なアプリケーションの設定を作成、検索、取得、更新、削除する方法について説明します。 '
ms.openlocfilehash: ab5a9cc927bd0a6c4efacce622cc71db1a9b02a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758986"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="4515c-103">EWS を使用して Exchange 内で永続的なアプリケーションの設定を管理します。</span><span class="sxs-lookup"><span data-stu-id="4515c-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="4515c-104">Exchange で EWS マネージ API または EWS を使用して、永続的なアプリケーションの設定を作成、検索、取得、更新、削除する方法について説明します。 </span><span class="sxs-lookup"><span data-stu-id="4515c-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="4515c-105">ユーザー設定オブジェクトは、ほとんどのクライアント アプリケーションでの検索結果から隠されているために主に、Exchange のクライアント アプリケーションの構成設定を格納するための最適なオプション。</span><span class="sxs-lookup"><span data-stu-id="4515c-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="4515c-106">クライアント アプリケーション通常を非表示にこれらの設定とエンド ・ ユーザーは、それらを表示する必要があるため、ユーザーは、この情報に誤ってアクセスされないようにします。</span><span class="sxs-lookup"><span data-stu-id="4515c-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="4515c-107">この資料のコード例は、検索、取得、更新、およびユーザーの構成オブジェクトに格納されている永続的なアプリケーションの設定を削除、作成する方法など、永続的な設定を管理するユーザーの構成オブジェクトを使用する方法を表示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="4515c-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-108"></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="4515c-109">EWS マネージ API を使用してアプリケーション設定を作成する</span><span class="sxs-lookup"><span data-stu-id="4515c-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="4515c-110">[UserConfiguration.Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用すると、カスタム構成設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="4515c-110">You can use the [UserConfiguration.Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="4515c-111">ユーザーの構成オブジェクトは、XML を含めることができますバイナリ、データ辞書、またはこれらの 3 つのデータ型の組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="4515c-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="4515c-112">次の例では、EWS のマネージ API を使用して、[下書き] フォルダーにバイナリ データを含む ContosoDraftSettings という名前のユーザー設定のオブジェクトを保存する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="4515c-113">これは、クライアント アプリケーション内の下書きアイテムを表示する方法に関する構成情報を格納する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="4515c-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
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

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="4515c-114">EWS を使用してアプリケーション設定を作成する</span><span class="sxs-lookup"><span data-stu-id="4515c-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="4515c-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-115"></span></span>

<span data-ttu-id="4515c-116">[CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS の操作を使用すると、カスタム構成設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="4515c-116">You can use the [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting.</span></span> <span data-ttu-id="4515c-117">次の使用例は、ContosoDraftSettings という名前のユーザーの構成オブジェクトを作成するため、要求 XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="4515c-117">The following example shows the request XML for creating a user configuration object named ContosoDraftSettings.</span></span> <span data-ttu-id="4515c-118">要求は、[下書き] フォルダーのユーザーの構成オブジェクトのバイナリ ストリームを保存しようとします。</span><span class="sxs-lookup"><span data-stu-id="4515c-118">The request attempts to save a binary stream to a user configuration object on the Drafts folder.</span></span> <span data-ttu-id="4515c-119">これは、EWS のマネージ API の使用例で生成されるのと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="4515c-119">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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

<span data-ttu-id="4515c-120">[応答 XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx)は、単純な作成要求が成功したかどうか、またはエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-120">The [response XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="4515c-121">EWS マネージ API を使用してアプリケーション設定を検索する</span><span class="sxs-lookup"><span data-stu-id="4515c-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="4515c-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-122"></span></span>

<span data-ttu-id="4515c-123">関連付けのトラバーサル オプションを使用して[Folder.FindItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用するにはユーザーの構成オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="4515c-123">You can use the [Folder.FindItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="4515c-124">次のコード例では、EWS のマネージ API を使用して、[下書き] フォルダーに格納されているユーザーの構成オブジェクトを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
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

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="4515c-125">EWS を使用してアプリケーション設定を検索する</span><span class="sxs-lookup"><span data-stu-id="4515c-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="4515c-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-126"></span></span>

<span data-ttu-id="4515c-127">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS の操作を使用するにはユーザーの構成オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="4515c-127">You can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="4515c-p105">次の例は、ユーザー構成オブジェクトを検索するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="4515c-p105">The following example shows the request XML for finding user configuration objects. This is the same XML that is generated by the EWS Managed API example.</span></span>
  
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

<span data-ttu-id="4515c-p106">次の例は、ユーザー構成オブジェクトの検索が成功した場合の応答 XML を示しています。これは、EWS マネージ API の例で処理されるものと同じ XML です。この応答 XML では次の点に注意してください。 </span><span class="sxs-lookup"><span data-stu-id="4515c-p106">The following example shows the successful response XML for finding user configuration objects. This is the same XML that is processed by the EWS Managed API example. Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="4515c-133">読みやすいように識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="4515c-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="4515c-134">メッセージとしては、2 つのユーザーの構成オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="4515c-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="4515c-135">**FindItem**操作には、メッセージ アイテムとして、EWS のスキーマで定義されていないすべてのアイテムが返されるためにです。</span><span class="sxs-lookup"><span data-stu-id="4515c-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="4515c-136">[ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx)プロパティの 2 つのユーザーの構成オブジェクトは、異なります。</span><span class="sxs-lookup"><span data-stu-id="4515c-136">The [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="4515c-137">EWS を使用して、最初のユーザー設定オブジェクトが作成されました。</span><span class="sxs-lookup"><span data-stu-id="4515c-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="4515c-138">2 番目のオブジェクトは、他の API によって作成されました。</span><span class="sxs-lookup"><span data-stu-id="4515c-138">The second object was created by another API.</span></span> 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="4515c-139">EWS マネージ API を使用してアプリケーション設定を取得して更新する</span><span class="sxs-lookup"><span data-stu-id="4515c-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="4515c-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-140"></span></span>

<span data-ttu-id="4515c-141">ユーザーの構成オブジェクトを検索すると後、は、メールボックスから構成オブジェクトを取得するのに[UserConfiguration.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4515c-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="4515c-142">構成オブジェクトを取得した後は、それを更新するのに[UserConfiguration.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx)メソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4515c-142">After you get the configuration object, you can use the [UserConfiguration.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="4515c-143">次の例では、取得し、EWS のマネージ API を使用してユーザーの構成オブジェクトを更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
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

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="4515c-144">EWS を使用してアプリケーション設定を取得して更新する</span><span class="sxs-lookup"><span data-stu-id="4515c-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="4515c-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-145"></span></span>

<span data-ttu-id="4515c-146">[GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS の操作は、メールボックス、およびオブジェクトを更新するのに[UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx)から構成オブジェクトを取得するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="4515c-146">You can use the [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object.</span></span> <span data-ttu-id="4515c-147">次の使用例は、TestConfig をという名前のユーザーの構成オブジェクトを取得するため、要求の XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="4515c-147">The following example shows the request XML for getting a user configuration object named TestConfig.</span></span> <span data-ttu-id="4515c-148">要求は、すべての構成が、応答で返されることを示しています。</span><span class="sxs-lookup"><span data-stu-id="4515c-148">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="4515c-149">これは、EWS のマネージ API の使用例で生成されるのと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="4515c-149">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4515c-p111">次の例は、ユーザー構成オブジェクトの取得が成功した場合の応答 XML を示しています。応答にはデータ辞書が含まれます。これは、EWS マネージ API の例で処理されるものと同じ XML です。 </span><span class="sxs-lookup"><span data-stu-id="4515c-p111">The following example shows the successful response XML for getting a user configuration objects. The response contains a data dictionary. This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="4515c-153">次の使用例は、ユーザーの構成オブジェクトを更新する要求の XML を示しています。</span><span class="sxs-lookup"><span data-stu-id="4515c-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="4515c-154">要求は、すべての構成が、応答で返されることを示しています。</span><span class="sxs-lookup"><span data-stu-id="4515c-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="4515c-155">これは、 **UserConfiguration.Update**メソッドを呼び出し、EWS のマネージ API の使用例で生成されるのと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="4515c-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="4515c-156">更新 XML には、既存の辞書のエントリと、更新する前に追加されたその他の 1 つが含まれているを確認できます。</span><span class="sxs-lookup"><span data-stu-id="4515c-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="4515c-157">[応答 XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx)は、単純な更新が成功したかどうか、またはエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-157">The [response XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="4515c-158">EWS マネージ API を使用してアプリケーション設定を削除する</span><span class="sxs-lookup"><span data-stu-id="4515c-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="4515c-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-159"></span></span>

<span data-ttu-id="4515c-160">[UserConfiguration.Delete](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用するにはユーザーの構成オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4515c-160">You can use the [UserConfiguration.Delete](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="4515c-161">次のコード例では、EWS のマネージ API を使用して、ContosoDraftSettings のユーザー設定のオブジェクトを削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
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

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="4515c-162">EWS を使用してアプリケーション設定を削除する</span><span class="sxs-lookup"><span data-stu-id="4515c-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="4515c-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4515c-163"></span></span>

<span data-ttu-id="4515c-164">ユーザー設定オブジェクトを削除するのには、 [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx)の EWS の操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4515c-164">You can use the [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="4515c-p114">次の例は、下書きフォルダーに適用されていた ContosoDraftSettings という名前のユーザー構成オブジェクトを削除するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。</span><span class="sxs-lookup"><span data-stu-id="4515c-p114">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder. This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="4515c-167">[応答 XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx)は、単純な削除要求の成功したかどうか、またはエラーが発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4515c-167">The [response XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4515c-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="4515c-168">See also</span></span>

- [<span data-ttu-id="4515c-169">Exchange の EWS の永続的なアプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="4515c-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="4515c-170">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="4515c-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="4515c-171">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="4515c-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

