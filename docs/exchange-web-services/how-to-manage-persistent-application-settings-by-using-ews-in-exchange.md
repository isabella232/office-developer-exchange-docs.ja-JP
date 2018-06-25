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
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a>EWS を使用して Exchange 内で永続的なアプリケーションの設定を管理します。

Exchange で EWS マネージ API または EWS を使用して、永続的なアプリケーションの設定を作成、検索、取得、更新、削除する方法について説明します。  
  
ユーザー設定オブジェクトは、ほとんどのクライアント アプリケーションでの検索結果から隠されているために主に、Exchange のクライアント アプリケーションの構成設定を格納するための最適なオプション。 クライアント アプリケーション通常を非表示にこれらの設定とエンド ・ ユーザーは、それらを表示する必要があるため、ユーザーは、この情報に誤ってアクセスされないようにします。 この資料のコード例は、検索、取得、更新、およびユーザーの構成オブジェクトに格納されている永続的なアプリケーションの設定を削除、作成する方法など、永続的な設定を管理するユーザーの構成オブジェクトを使用する方法を表示します。

<a name="createconfiguration"> </a>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアプリケーション設定を作成する

[UserConfiguration.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用すると、カスタム構成設定を作成します。 ユーザーの構成オブジェクトは、XML を含めることができますバイナリ、データ辞書、またはこれらの 3 つのデータ型の組み合わせです。 次の例では、EWS のマネージ API を使用して、[下書き] フォルダーにバイナリ データを含む ContosoDraftSettings という名前のユーザー設定のオブジェクトを保存する方法を示します。 これは、クライアント アプリケーション内の下書きアイテムを表示する方法に関する構成情報を格納する場合に便利です。 
  
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

## <a name="create-an-application-setting-by-using-ews"></a>EWS を使用してアプリケーション設定を作成する
<a name="bk_createEWS"> </a>

[CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS の操作を使用すると、カスタム構成設定を作成します。 次の使用例は、ContosoDraftSettings という名前のユーザーの構成オブジェクトを作成するため、要求 XML を示しています。 要求は、[下書き] フォルダーのユーザーの構成オブジェクトのバイナリ ストリームを保存しようとします。 これは、EWS のマネージ API の使用例で生成されるのと同じ XML です。 
  
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

[応答 XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx)は、単純な作成要求が成功したかどうか、またはエラーが発生したかどうかを示します。 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアプリケーション設定を検索する
<a name="findconfiguration"> </a>

関連付けのトラバーサル オプションを使用して[Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用するにはユーザーの構成オブジェクトを検索します。 次のコード例では、EWS のマネージ API を使用して、[下書き] フォルダーに格納されているユーザーの構成オブジェクトを検索する方法を示します。 
  
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

## <a name="find-an-application-setting-by-using-ews"></a>EWS を使用してアプリケーション設定を検索する
<a name="bk_findEWS"> </a>

[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS の操作を使用するにはユーザーの構成オブジェクトを検索します。 
  
次の例は、ユーザー構成オブジェクトを検索するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。
  
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

次の例は、ユーザー構成オブジェクトの検索が成功した場合の応答 XML を示しています。これは、EWS マネージ API の例で処理されるものと同じ XML です。この応答 XML では次の点に注意してください。  
  
- 読みやすいように識別子と変更キーが短縮されています。
    
- メッセージとしては、2 つのユーザーの構成オブジェクトが返されます。 **FindItem**操作には、メッセージ アイテムとして、EWS のスキーマで定義されていないすべてのアイテムが返されるためにです。 
    
- [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx)プロパティの 2 つのユーザーの構成オブジェクトは、異なります。 EWS を使用して、最初のユーザー設定オブジェクトが作成されました。 2 番目のオブジェクトは、他の API によって作成されました。 
    
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

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアプリケーション設定を取得して更新する
<a name="getconfiguration"> </a>

ユーザーの構成オブジェクトを検索すると後、は、メールボックスから構成オブジェクトを取得するのに[UserConfiguration.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドを使用できます。 構成オブジェクトを取得した後は、それを更新するのに[UserConfiguration.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx)メソッドを使用できます。 次の例では、取得し、EWS のマネージ API を使用してユーザーの構成オブジェクトを更新する方法を示します。 
  
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

## <a name="get-and-update-application-settings-by-using-ews"></a>EWS を使用してアプリケーション設定を取得して更新する
<a name="bk_getEWS"> </a>

[GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS の操作は、メールボックス、およびオブジェクトを更新するのに[UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx)から構成オブジェクトを取得するために使用できます。 次の使用例は、TestConfig をという名前のユーザーの構成オブジェクトを取得するため、要求の XML を示しています。 要求は、すべての構成が、応答で返されることを示しています。 これは、EWS のマネージ API の使用例で生成されるのと同じ XML です。 
  
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

次の例は、ユーザー構成オブジェクトの取得が成功した場合の応答 XML を示しています。応答にはデータ辞書が含まれます。これは、EWS マネージ API の例で処理されるものと同じ XML です。  
  
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

次の使用例は、ユーザーの構成オブジェクトを更新する要求の XML を示しています。 要求は、すべての構成が、応答で返されることを示しています。 これは、 **UserConfiguration.Update**メソッドを呼び出し、EWS のマネージ API の使用例で生成されるのと同じ XML です。 更新 XML には、既存の辞書のエントリと、更新する前に追加されたその他の 1 つが含まれているを確認できます。 
  
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

[応答 XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx)は、単純な更新が成功したかどうか、またはエラーが発生したかどうかを示します。 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してアプリケーション設定を削除する
<a name="deleteconfiguration"> </a>

[UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用するにはユーザーの構成オブジェクトを削除します。 次のコード例では、EWS のマネージ API を使用して、ContosoDraftSettings のユーザー設定のオブジェクトを削除する方法を示します。 
  
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

## <a name="delete-an-application-setting-by-using-ews"></a>EWS を使用してアプリケーション設定を削除する
<a name="bk_deleteEWS"> </a>

ユーザー設定オブジェクトを削除するのには、 [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx)の EWS の操作を使用できます。 
  
次の例は、下書きフォルダーに適用されていた ContosoDraftSettings という名前のユーザー構成オブジェクトを削除するための要求 XML を示しています。これは、EWS マネージ API の例で生成されるものと同じ XML です。
  
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

[応答 XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx)は、単純な削除要求の成功したかどうか、またはエラーが発生したかどうかを示します。 
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS の永続的なアプリケーションの設定](persistent-application-settings-in-ews-in-exchange.md)
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

