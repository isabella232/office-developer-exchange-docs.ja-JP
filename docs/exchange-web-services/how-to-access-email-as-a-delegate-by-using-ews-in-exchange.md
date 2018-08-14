---
title: Exchange で EWS を使用して、代理人としてメールにアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。
ms.openlocfilehash: 23dd35f95b1303ff643e3760aa408e308725cb12
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354037"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、代理人としてメールにアクセスする

Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。
  
EWS マネージ API または EWS を使用して、ユーザーにメーボックス所有者の受信トレイ フォルダーへの代理人アクセス権を付与できます。代理人は、メールボックス所有者の代わりに会議出席依頼を作成し、アクセス許可に応じて、メールボックス所有者の受信トレイ フォルダーのメールの検索、取得、更新、削除を行うことができます。
  
代理人として、代理人アクセス権なしで受信トレイ フォルダーへのアクセスに使用するのと同じメソッドと操作を使用して、メールボックス所有者の受信トレイ フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用してメール アイテムを検索または作成する必要がある点です。アイテム ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、削除できます。 
  
**表 1. 代理人としてメールにアクセスするための EWS マネージ API メソッドと EWS 操作**

|**目的**|**使用する EWS マネージ API メソッド…**|**使用する EWS 操作…**|
|:-----|:-----|:-----|
|代理人としてメールを作成して送信する  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx): [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の下書きフォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx): [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の送信済みアイテム フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> [SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|代理人として複数のメール メッセージを作成する  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|代理人としてメールを検索する  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する  <br/> |
|代理人としてメールを取得  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|代理人としてメールを更新する  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [EmailMessage.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|代理人としてメールを削除する  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [EmailMessage.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
代理人としてメールを操作する場合、次の点に注意してください。
  
- 代理人が行う必要がある操作が会議出席依頼と出欠の返答だけである場合、受信トレイ フォルダーへのアクセスは必要ありません。詳しくは、「[代理人として予定表にアクセスするために事前に必要なタスク](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq)」をご覧ください。
    
- メールボックス所有者の代理として送信したメッセージを受信者が受信すると、送信者は「*メールボックス所有者*の*代理人*」として表示されます。 
    
> [!NOTE]
> この記事のコード例では、primary@contoso.com は、メールボックス所有者です。 
  
## <a name="prerequisite-tasks"></a>事前に必要なタスク
<a name="bk_prereq"> </a>

ユーザーは、代理人としてメールボックス所有者の受信トレイ フォルダーにアクセスできるようにするために、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)メールボックス所有者の受信トレイ フォルダーに追加される必要があります。  
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人としてメールを作成および送信する
<a name="bk_createewsma"> </a>

EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の代わりにメールを作成および送信することができます。 次の例は、[Save](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx) メソッドを使用してメールボックス所有者の下書きフォルダーにメッセージを保存し、[SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx) メソッドを使用してそのメールを送信してそのメッセージをメールボックス所有者の送信済みアイテム フォルダーに保存する方法を示しています。 
  
この例は、**service** が代理人の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、代理人に[メールボックス所有者の受信トレイ、下書き、送信済みアイテムの各フォルダーの適切なアクセス許可](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)が付与されていることを前提にしています。
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a>EWS を使用して代理人としてメールを作成して送信する
<a name="bk_createews"> </a>

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の代わりにメールを作成および送信することができます。次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用してメールを作成し、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作によって送信してメールボックス所有者の送信済みアイテム フォルダーに保存する方法を示しています。 
  
またこれは、[メールの作成と送信](#bk_createewsma)に **Save** メソッドを使用する際に、EWS マネージ API が送信する最初の XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、メールが正常に作成および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。また、この応答には新しく作成されたメールのアイテム ID も含まれます。
  
**ItemId** 値は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

次に、**SendItem** 操作を使用してメールボックス所有者の代理としてメッセージを送信し、メールボックス所有者の送信済みアイテム フォルダーに保存します。 
  
**ItemId** 値は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**SendItem** 要求に [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) メッセージで応答します。このメッセージには、メールがメールボックス所有者の送信済みアイテム フォルダーに正常に送信および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人としてメールを検索する
<a name="bk_searchewsma"> </a>

メールを検索するには、[FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターが含まれるいずれかの [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドを使用し、メールボックス所有者の受信トレイ フォルダーを指定する必要があります。 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

**FindItems** 呼び出しが ID と共に応答を返すと、ID と[暗黙的アクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して対象のメールを取得、更新、削除できます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a>EWS を使用して代理人としてメールを検索する
<a name="bk_searchews"> </a>

EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、一連の検索条件に一致するメールを検索できます。次の例は、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、件名に「soccer」という語が含まれる、所有者の受信トレイ フォルダー内のメッセージを検索する方法を示しています。 
  
また、これは、[メールを検索する](#bk_searchewsma)際に、EWS マネージ API が送信する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**FindItem** 要求に [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) メッセージで応答します。このメッセージには、検索が正常に完了したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。この応答には、検索条件と一致するすべての [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素が含まれます。この例では、1 つのメールのみが検出されました。 
  
[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

この時点で、条件と一致するメールの **ItemId** がわかったので **ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してメールの取得、更新、削除を行えます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、代理人としてメール アイテムを取得、更新、削除する
<a name="bk_geteswma"> </a>

EWS マネージ API を使用すると、代理人アクセスを使用していない場合と同じように、メール アイテムを取得、更新、削除できます。唯一の違いは、**ExchangeService** オブジェクトが代理ユーザーを対象にしている点です。**Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の受信トレイ フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 2. 代理人としてメールを操作する EWS マネージ API メソッド**

|**タスク**|**EWS マネージ API メソッド**|**コード例**|
|:-----|:-----|:-----|
|メールを取得する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|メールを更新する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを更新する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|メールを削除する  <br/> |[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[EWS マネージ API を使用してアイテムを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a>EWS を使用して、代理人としてメール アイテムを取得、更新、削除する
<a name="bk_getews"> </a>

EWS マネージ API を使用すると、代理人アクセスを使用していない場合と同じように、メール アイテムを取得、更新、削除できます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。**GetItem** 要求に含まれるアイテム ID は、メールボックス所有者の受信トレイ フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。 
  
**表 3. 代理人としてメールを操作するための EWS 操作**

|**タスク**|**EWS 操作**|**コード例**|
|:-----|:-----|:-----|
|メールを取得する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[EWS を使用してアイテムを取得する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|メールを更新する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[EWS を使用してアイテムを更新する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|メールを削除する  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[EWS を使用してアイテムを削除する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)    
- [Exchange で EWS を使用して代理人を追加および削除する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [Exchange の予定表と EWS](calendars-and-ews-in-exchange.md)
    

