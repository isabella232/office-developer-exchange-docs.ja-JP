---
title: Exchange で EWS を使用してアイテムを同期する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 886e7d35-9096-480b-8a8c-a7db27da06c2
description: クライアントを同期するために、EWS マネージ API または EWS を使用して、フォルダー内のすべてのアイテムの一覧、またはフォルダー内で発生した変更の一覧を取得する方法を紹介します。
ms.openlocfilehash: e75f90b2d28d782465de89000796deccdd125e25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527713"
---
# <a name="synchronize-items-by-using-ews-in-exchange"></a>Exchange で EWS を使用してアイテムを同期する

クライアントを同期するために、EWS マネージ API または EWS を使用して、フォルダー内のすべてのアイテムの一覧、またはフォルダー内で発生した変更の一覧を取得する方法を紹介します。
  
Exchange の EWS では、アイテムの同期とフォルダーの同期を使用して、クライアントとサーバー間でメールボックスのコンテンツを同期します。アイテムの同期では、フォルダーにあるアイテムの初期の一覧を取得し、その後段階的にそれらのアイテムに対して行われた変更を取得し、さらに新しいアイテムも取得します。
  
クライアントにアイテムを同期する前に、まず[フォルダー階層を同期する](how-to-synchronize-folders-by-using-ews-in-exchange.md)必要があることに注意してください。 フォルダー階層をクライアント上に適切に設定した後、EWS マネージ API を使用してアイテムの同期を実行する場合は、まず [ExchangeService.SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) メソッドを使用して、[受信トレイ内のアイテムの初期の一覧を取得します](#bk_cesyncongoingewsma)。 次に、後続の呼び出し中に _cSyncState_ パラメーターの値を更新して、受信トレイ内の変更されたアイテムの一覧を取得します。 
  
[フォルダー階層を同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)した後、EWS を使用してアイテムの同期を実行するには、[SyncFolderItems operation](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) を使用して、[受信トレイ内のアイテムの初期の一覧](#bk_ewsexamplea)を要求して、応答を解析します。その後任意の時点で[メールボックス内のアイテムへの変更を取得](#bk_ewsexamplec)して、応答を解析します。クライアントは、初期の一覧または変更されたアイテムの一覧を受信した後、[ローカルに更新を実行します](#bk_nextsteps)。後で変更を取得する方法とタイミングは、アプリケーションが使用している[同期のデザイン パターン](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) によって異なります。 
  
## <a name="get-the-list-of-all-items-or-changed-items-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してすべてのアイテムまたは変更されたアイテムの一覧を取得する
<a name="bk_cesyncongoingewsma"> </a>

次のコード例では、受信トレイ フォルダー内のすべてのアイテムの初期の一覧を取得してから、前回の同期以降に発生した受信トレイ フォルダー内のアイテムに対する変更の一覧を取得する方法を示します。 [SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) メソッドの最初の呼び出し中に、_cSyncState_ の値を null に設定します。 メソッドが完了したら、次の **SyncFolderItems** メソッド呼び出しで使用するために _cSyncState_ の値をローカルに保存します。 最初の呼び出しと後続の呼び出しの両方で、変更がなくなるまで、**SyncFolderItems** メソッドの連続呼び出しを使用して、10 回のバッチ処理でアイテムが取得されます。 
  
次の例は、_propertySet_ パラメーターを IdOnly に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。 この例では、**service** は有効な **ExchangeService** オブジェクト バインドであり、_cSyncState_ は前の **SyncFolderItems** の呼び出しによって返された同期状態を表すものとします。 
  
```cs
// Track whether there are more items available for download on the server.
bool moreChangesAvailable = false;
do
{
    // Get a list of all items in the Inbox by calling SyncFolderHierarchy repeatedly until no more changes are available.
    // The folderId parameter must be set to the root folder to synchronize,
    // and must be same folder ID as used in previous synchronization calls. 
    // The propertySet parameter is set to IdOnly to reduce calls to the Exchange database,
    // because any additional properties result in additional calls to the Exchange database. 
    // The ignoredItemIds parameter is set to null, so that no items are ignored.
    // The maxChangesReturned parameter is set to return a maximum of 10 items (512 is the maximum).
    // The syncScope parameter is set to Normal items, so that associated items will not be returned.
    // The syncState parameter is set to cSyncState, which should be null in the initial call, 
    // and should be set to the sync state returned by the 
    // previous SyncFolderItems call in subsequent calls.
    ChangeCollection<ItemChange> icc = service.SyncFolderItems(new FolderId(WellKnownFolderName.Inbox), PropertySet.IdOnly, null, 10, SyncFolderItemsScope.NormalItems, cSyncState);
    // If the count of changes is zero, there are no changes to synchronize.
    if (icc.Count == 0)
    {
        Console.WriteLine("There are no item changes to synchronize.");
    }
    // Otherwise, write all the changes included in the response 
    // to the console. 
    else
    {
        foreach (ItemChange ic in icc)
        {
            Console.WriteLine("ChangeType: " + ic.ChangeType.ToString());
            Console.WriteLine("ItemId: " + ic.ItemId);
            Console.WriteLine("===========");
        }
    }
    // Save the sync state for use in future SyncFolderContent requests.
    // The sync state is used by the server to determine what changes to report
    // to the client.
    string sSyncState = icc.SyncState;
   // Determine whether more changes are available on the server.
   moreChangesAvailable = icc.MoreChangesAvailable;
}
while (moreChangesAvailable);

```

**SyncFolderItems** メソッドは、[Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) や [Attachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) などのプロパティを返すことができないという点で [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドに似ています。 **SyncFolderItems** メソッドで返すことができないプロパティが必要な場合は、**SyncFolderItems** を呼び出す際に [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.idonly%28v=exchg.80%29.aspx) プロパティ セットを指定してから、[ExchangeService.LoadPropertiesForItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) メソッドを使用して、**SyncFolderItems** メソッドによって返されたアイテムに必要なプロパティを取得します。 
  
サーバー上の新しいアイテムまたは変更されたアイテムの一覧を取得した後、[クライアント上でアイテムを作成または更新します](#bk_nextsteps)。
  
## <a name="get-the-initial-list-of-items-by-using-ews"></a>EWS を使用してアイテムの初期のリストを取得する
<a name="bk_ewsexamplea"> </a>

次の例は、[SyncFolderItems 操作](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)を使用して、受信トレイ内のアイテムの初期の一覧を取得する XML 要求を示しています。 これは、[SyncFolderItems メソッドを使用してアイテムの一覧を取得する](#bk_cesyncongoingewsma)際に、EWS マネージ API が送信する XML 要求でもあります。 **SyncFolderItems** 操作の [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素は、これが最初の同期であるために含まれません。 次の例は、[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。
  
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
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

<a name="bk_responsesyncfolderitems"> </a>

次の例は、クライアントからの **SyncFolderItems** 操作の要求を処理した後にサーバーによって返される XML 応答を示します。最初の応答には、最初の同期中はすべてのアイテムが新しいものと見なされるため、5 つのアイテムの [Create](https://msdn.microsoft.com/library/cb5e64a2-66a5-4447-921e-7c13efb8f6bf%28Office.15%29.aspx) 要素が含まれます。読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q04QAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdC"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q07AAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdB"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="q1AwAAAA=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVdA"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc5"/>
              </t:Message>
            </t:Create>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AAMkADBh=="
                          ChangeKey="CQAAABYAAABhFfgM7MNwSYx0VZ0GoBMJAAAATVc4"/>
              </t:Message>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

サーバー上の新しいアイテムの一覧を取得した後、[クライアント上でアイテムを作成します](#bk_nextsteps)。
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>EWS を使用して前回の同期以降の変更を取得する
<a name="bk_ewsexamplec"> </a>

次の例は、[SyncFolderItems 操作](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)を使用して、受信トレイ内のアイテムに行われた変更の一覧を取得する XML 要求を示します。これは、[受信トレイに対して行われた変更の一覧を取得する](#bk_cesyncongoingewsma)際に、EWS マネージ API が送信する XML 要求でもあります。次の例では、[SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素の値を[以前の応答](#bk_responsesyncfolderitems)で返された値に設定します。またこの例では、デモ用に [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** ではなく、**AllProperties** に設定し、返される追加のプロパティを表示します。[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定することは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。**SyncState** の値は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
      <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderItems>
      <m:ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:ItemShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAAA==</m:SyncState>
      <m:MaxChangesReturned>10</m:MaxChangesReturned>
      <m:SyncScope>NormalItems</m:SyncScope>
    </m:SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

次の例は、クライアントからの **SyncFolderItems** 操作の要求を処理した後にサーバーによって返される XML 応答を示します。この応答は、以前の同期以降に、1 つのアイテムが更新され、2 つのアイテムが作成され、1 つのアイテムの読み取りのフラグが変更され、1 つのアイテムが削除されたことを示しています。読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3"
                 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAAAAEAO29B2AcSZY==</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Update>
                <t:Message>
                  <t:ItemId Id="q04QAAAA==" ChangeKey="CQAAABYAAADZGACZQpSgSpyNkexYe2b7AAAAird/" />
                  <t:ParentFolderId Id=" AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Company Soccer Team</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:22:10Z</t:DateTimeReceived>
                  <t:Size>23110</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;8e084ea1a5b64f97b95fa8a863a5869d@CH1SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:22:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:38Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>All Employees</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T16:53:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQACAi+NTh0F5Eg5YDwpJsXPE=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5V/ZICL41OHQXkSDlgPCkmxc8ZYxA3I4gAAP5UeAANHpbIAAEE+0gAABYhSAACGYTIAAA2+vgAAE81qAkhv0Eg==</t:ConversationIndex>
                  <t:ConversationTopic>Company Soccer Team</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Alfred  Welker </t:Name>
                      <t:EmailAddress>Alfred.Welker@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e5919a09c8fc4d64b6ffd3542e194fc3@BY2SR01MB609.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
            </t:Update>
            <t:Create>
              <t:Message>
                <t:ItemId Id="AQMkAD+" />
                <t:ParentFolderId Id="AQMkA==" ChangeKey="AQAAAA==" />
                <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T16:20:10Z</t:DateTimeReceived>
                  <t:Size>32515</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T16:20:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:33Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara  Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:35Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DNgAAAfKE=</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Hope Gross</t:Name>
                      <t:EmailAddress>Hope.Gross@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96@SN2SR01MB005.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>&amp;lt;2d4d7d…</t:References>
                </t:Message>
              </t:Create>
              <t:Create>
                <t:Message>
                  <t:ItemId Id="Q04AAAAA==" ChangeKey="AAAirbnd" />
                  <t:ParentFolderId Id="AgENAAAA" ChangeKey="AQAAAA==" />
                  <t:ItemClass>IPM.Note</t:ItemClass>
                  <t:Subject>RE: Review Proposal for Contoso</t:Subject>
                  <t:Sensitivity>Normal</t:Sensitivity>
                  <t:DateTimeReceived>2013-08-29T15:30:10Z</t:DateTimeReceived>
                  <t:Size>29518</t:Size>
                  <t:Importance>Normal</t:Importance>
                  <t:InReplyTo>&amp;lt;f0db3ead01db4fe087d98022149aa16f@SN2SR01MB001.namsdf01.sdf.contoso.com&amp;gt;</t:InReplyTo>
                  <t:IsSubmitted>false</t:IsSubmitted>
                  <t:IsDraft>false</t:IsDraft>
                  <t:IsFromMe>false</t:IsFromMe>
                  <t:IsResend>false</t:IsResend>
                  <t:IsUnmodified>false</t:IsUnmodified>
                  <t:DateTimeSent>2013-08-29T15:30:10Z</t:DateTimeSent>
                  <t:DateTimeCreated>2013-08-28T04:07:36Z</t:DateTimeCreated>
                  <t:DisplayCc />
                  <t:DisplayTo>Legal Team; Executives</t:DisplayTo>
                  <t:HasAttachments>false</t:HasAttachments>
                  <t:Culture>en-US</t:Culture>
                  <t:EffectiveRights>
                    <t:CreateAssociated>false</t:CreateAssociated>
                    <t:CreateContents>false</t:CreateContents>
                    <t:CreateHierarchy>false</t:CreateHierarchy>
                    <t:Delete>true</t:Delete>
                    <t:Modify>true</t:Modify>
                    <t:Read>true</t:Read>
                    <t:ViewPrivateItems>true</t:ViewPrivateItems>
                  </t:EffectiveRights>
                  <t:LastModifiedName>Mara Whitley</t:LastModifiedName>
                  <t:LastModifiedTime>2013-08-28T04:07:38Z</t:LastModifiedTime>
                  <t:IsAssociated>false</t:IsAssociated>
                  <t:WebClientReadFormQueryString>?ae=Item&amp;amp;a=Open&amp;amp;t=IPM.Note&amp;amp;id=&amp;amp;exvsurl=1</t:WebClientReadFormQueryString>
                  <t:ConversationId Id="AAQkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAQAIsBEZp25UpElByLLUQFH6Q=" />
                  <t:Sender>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:Sender>
                  <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                  <t:ConversationIndex>AQHM5WBRiwERmnblSkSUHIstRAUfpJYw9fbSgAAAdm2AAAB6koAAAHTDgAADl6+AAAbxCYAABm5PgAACSA+AANx034AAEKGQgAAAfsiAAB7m3IAABG+ngAABPZyAAASUzoAAA2DN</t:ConversationIndex>
                  <t:ConversationTopic>Review Proposal for Contoso</t:ConversationTopic>
                  <t:From>
                    <t:Mailbox>
                      <t:Name>Mack Chaves</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                      <t:MailboxType>Mailbox</t:MailboxType>
                    </t:Mailbox>
                  </t:From>
                  <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6@SN2SR01MB006.namsdf01.sdf.contoso.com&amp;gt;</t:InternetMessageId>
                  <t:IsRead>true</t:IsRead>
                  <t:References>namsdf01.sdf.contoso.com&amp;gt;</t:References>
                </t:Message>
              </t:Create>
              <t:ReadFlagChange>
                <t:ItemId Id=" q07AAAAA==" ChangeKey="CQAAAA==" />
                <t:IsRead>true</t:IsRead>
              </t:ReadFlagChange>
              <t:Delete>
                <t:ItemId Id=" q1AwAAAA==" ChangeKey="CQAAAA==" />
              </t:Delete>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderItemsResponse>
  </s:Body>
</s:Envelope>
```

**SyncFolderItems** 操作は、要素の [Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) や [Attachments](https://msdn.microsoft.com/library/b470e614-34bb-44f0-8790-7ddbdcbbd29d%28Office.15%29.aspx) などの要素を返すことができないという点で [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドに似ています。 **SyncFolderItems** 操作で返すことができないプロパティが必要な場合は、**SyncFolderItems** を呼び出す際に [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素の値を IdOnly に設定してから、[GetItem 操作](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)を使用して **SyncFolderItems** 操作によって返されたアイテムに必要なプロパティを取得します。 
  
サーバー上の変更されたアイテムの一覧を取得した後、[クライアント上でアイテムを更新します](#bk_nextsteps)。
  
## <a name="update-the-client"></a>クライアントを更新する
<a name="bk_nextsteps"> </a>

EWS マネージ API を使用している場合は、新しいアイテムまたは変更されたアイテムの一覧を取得した後、[LoadPropertiesForItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx) メソッドを使用して新しいアイテムまたは変更されたアイテムのプロパティを取得し、プロパティをローカル値と比較して、クライアント上のアイテムを更新します。 
  
EWS を使用している場合は、[GetItem 操作](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)を使用して新しいアイテムまたは変更されたアイテムのプロパティを取得し、クライアント上のアイテムを更新します。 
  
## <a name="see-also"></a>関連項目


- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用してフォルダーを同期させる](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Exchange の EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange の通知サブスクリプション、メールボックス イベント、および EWS](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    

