---
title: Exchange で EWS を使用して、代理人として連絡先にアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。
ms.openlocfilehash: 06faf7dd7459b14792abbea21761e909c8eb9fb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455346"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、代理人として連絡先にアクセスする

Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。
  
EWS マネージ API または EWS を使用して、ユーザーにメールボックス所有者の連絡先フォルダーへのアクセス権を付与できます。代理人は、メールボックス所有者の代わりに連絡先を作成し、アクセス許可に応じて、メールボックス所有者の連絡先フォルダーから連絡先を取得、更新、および削除することができます。
  
代理人として、同じメソッドと操作を使用して、自分の連絡先フォルダーへのアクセスに使用する、メールボックス所有者の連絡先フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して連絡先アイテムを検索または作成する必要がある点です。アイテム ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、または削除できます。 
  
**表 1. 代理人として連絡先にアクセスするための EWS マネージ API メソッドと EWS 操作**

|**目的**|**使用する EWS マネージ API メソッド…**|**使用する EWS 操作…**|
|:-----|:-----|:-----|
|代理人として連絡先を作成する  <br/> |[Item.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx): [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の連絡先フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) を提供する場合  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合  <br/> |
|代理人として複数の連絡先を作成する  <br/> |[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合  <br/> |
|代理人として連絡先を解決する  <br/> |[ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx): [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の連絡先フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合  <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合  <br/> |
|代理人として連絡先を検索する  <br/> |[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合  <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合  <br/> |
|代理人として連絡先を取得する  <br/> |[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|代理人として連絡先を更新する  <br/> |[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) の後に [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) を使用する <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|代理人として連絡先を削除する  <br/> |[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) の後に [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) 使用する <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> この記事のコード例では、primary@contoso.com がメールボックス所有者です。 

<a name="bk_prereq"> </a>

## <a name="prerequisite-tasks"></a>事前に必要なタスク

ユーザーは、代理人としてメールボックス所有者の連絡先フォルダーにアクセスできるようにするために、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)メールボックス所有者の連絡先フォルダーに追加される必要があります。 

<a name="bk_createewsma"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人として連絡先を作成する

EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先を作成することができます。 この例は、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。 
  
この例では、**service** が代理人の有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、代理人にメールボックス所有者の連絡先フォルダーの適切なアクセス許可が付与されていることを前提にしています。 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

アイテムの保存時には、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッド呼び出しでメールボックス所有者の連絡先フォルダーを識別する必要があることにご注意ください。 メールボックス所有者の連絡先フォルダーを指定しない場合、会議出席依頼はメールボックス所有者の連絡先フォルダーではなく、代理人の連絡先フォルダーに保存されます。 メールボックス所有者の連絡先フォルダーは、2 つの方法で **Save** メソッド呼び出しに含めることができます。 メールボックス所有者の [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) と SMTP アドレスを使用して、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) オブジェクトの新しいインスタンスをインスタンス化することをお勧めします。 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

ただし、最初に連絡先フォルダーへの [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) を使用してから、 **Save** メソッド呼び出しでフォルダーの ID を使用することもできます。 ただし、これにより追加の EWS 呼び出しが作成されることにご注意ください。 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<a name="bk_createews"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a>EWS を使用して、代理人として連絡先を作成する

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先アイテムを作成することができます。この例では、[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) を使用して連絡先を作成する方法を示します。 
  
これは、[連絡先の作成](#bk_createewsma)に **Save** メソッドを使用する場合、EWS マネージ API が送信する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、[CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージを含む **CreateItem** 要求に応答します。このメッセージには、連絡先が正常に作成されたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。また、応答には新しく作成された連絡先のアイテム ID も含まれます。

<a name="bk_resolveewsma"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人として連絡先を解決する

場合によって、あいまいな名前または語句に基づいて連絡先を検索するには、メールボックス所有者の連絡先フォルダーを指定するようにするため、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) を含む [ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) メソッドのいずれかを使用する必要があります。 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

**ResolveNames** メソッドの呼び出しが ID と共に応答を返すと、ID と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;を使用して[連絡先を取得、更新または削除](#bk_getewsma)できます。メールボックス所有者の SMTP アドレスを指定する必要はありません。 

<a name="bk_resolveews"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a>EWS を使用して、代理人として連絡先を解決する

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先内の部分的な名前を解決できます。この例では、[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作を使用して、"johnson" という単語が含まれるメールボックス所有者の連絡先フォルダー内で会議を検索する方法を示します。  
  
これは、[連絡先の解決](#bk_resolveewsma)に **ResolvName** メソッドを使用する場合、EWS マネージ API が送信する XML 要求でもあります。
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**ResolveNames** 要求に対して[ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) メッセージで応答します。このメッセージには、操作が正常に完了され、結果が 1 つだけ検出されたことを示す **NoError** と、複数の結果が検出された場合は **ErrorNameResolutionMultipleResults** という [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値が含まれます。これは、連絡先 (「[EWS マネージ API を使用して、代理人として連絡先を作成する](#bk_createewsma)」) に基づく 3 番目のコード例で示されています。 応答には各結果の [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) も含まれます。 
  
**ItemId** 要素の値は読みやすいよう短縮されています。 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

あいまいな名前と一致する連絡先の **ItemId** がわかると、**ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;を使用して、[EWS を使用して、代理人として連絡先アイテムを取得、更新、または削除する](#bk_getews)ことができます。メールボックス所有者の SMTP アドレスを指定する必要はありません。 

<a name="bk_getewsma"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人として連絡先アイテムを取得、更新、または削除する

EWS マネージ API を使用すると、代理人アクセスを使用していない場合に取得、更新、または削除のアクションを実行するのと同じ方法で、連絡先アイテムを取得、更新、または削除することができます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。**Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の連絡先フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 2. 代理人として連絡先を操作する EWS マネージ API メソッド**

|**タスク**|**EWS マネージ API メソッド**|**コード例**|
|:-----|:-----|:-----|
|連絡先を取得する  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|連絡先を更新する  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを更新する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|連絡先を削除する  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<a name="bk_getews"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a>EWS を使用して、代理人として連絡先アイテムを取得、更新、または削除する

EWS を使用すると、代理人アクセスを使用していない場合に取得、更新、または削除のアクションを実行するのと同じ方法で、連絡先アイテムを取得、更新、または削除することができます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) 要求に含まれるアイテム ID は、メールボックス所有者の連絡先フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 3. 代理人として連絡先を操作するための EWS 操作**

|**タスク**|**EWS 操作**|**サンプル**|
|:-----|:-----|:-----|
|連絡先を取得する  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[EWS を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|連絡先を更新する  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) を使用する <br/> |[EWS を使用してアイテムを更新する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|連絡先を削除する  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) を使用する <br/> |[EWS を使用してアイテムを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)
- [Exchange で EWS を使用して代理人を追加および削除する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)
- [Exchange 2013 の EWS を使用して、あいまいな名前を解決する](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

