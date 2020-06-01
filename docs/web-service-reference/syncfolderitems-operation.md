---
title: SyncFolderItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: SyncFolderItems 操作は、Exchange サーバーとクライアントの間でアイテムを同期します。
ms.openlocfilehash: 1a28d895eda11dd43f77ec2662a60a426cfc463c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468146"
---
# <a name="syncfolderitems-operation"></a>SyncFolderItems 操作

SyncFolderItems 操作は、Exchange サーバーとクライアントの間でアイテムを同期します。
  
## <a name="remarks"></a>注釈

SyncFolderItems 操作は、最大512の変更を返します。 追加の変更を取得するには、以降の SyncFolderItems 要求を実行する必要があります。 
  
SyncFolderItems は FindItem 操作に似ていますが、本文や添付ファイルなどのプロパティを返すことはできません。 SyncFolderItems 操作が必要なプロパティを返さない場合は、 [GetItem 操作](getitem-operation.md)を使用して、syncfolderitems から返された各アイテムの特定のプロパティセットを取得できます。 
  
## <a name="syncfolderitems-request-example"></a>SyncFolderItems 要求の例

### <a name="description"></a>説明

次の SyncFolderItems 要求の例は、フォルダー内のアイテムを同期する方法を示しています。 この例では、[送信済みアイテム] フォルダーに対して行われた最初の同期ではないフォルダーアイテムの同期を示します。 クライアントと Exchange サーバーの同期を最初に試行する要求には、 [Syncstate](syncstate-ex15websvcsotherref.md)要素は含まれていません。 フォルダー階層内のアイテムを最初に同期しようとすると、そのメールボックス内のすべてのアイテムが返されます。[無視](ignore.md)要素で識別されるアイテムは除きます。 この SyncFolderItems 要求は、前回の同期以降のフォルダーアイテムへのすべての変更を同期しようとします。 この要求は、 [ignore](ignore.md)要素で識別される1つのアイテムを同期しようとする試行を無視します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすくするために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータと[ItemId](itemid.md)要素**Id**属性は短縮されています。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [SyncFolderItems](syncfolderitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncFolderId](syncfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [無視](ignore.md)
    
- [ItemId](itemid.md)
    
- [Maxの戻り値](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a>正常な SyncFolderItems 応答

### <a name="description"></a>説明

次の例は、SyncFolderItems 要求に対する正常な応答を示しています。 この例では、[送信済みアイテム] フォルダーから会議出席依頼が同期されます。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすくするために、 [Syncstate](syncstate-ex15websvcsotherref.md)要素の base64 でエンコードされたデータと[ItemId](itemid.md)要素**Id**属性は短縮されています。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
- [変更 (アイテム)](changes-items.md)
    
- [Create (ItemSync)](create-itemsync.md)
    
- [MeetingRequest](meetingrequest.md)
    
- [ItemId](itemid.md)
    
- [[件名]](subject.md)
    
- [Sensitivity](sensitivity.md)
    
- [IsOutOfDate](isoutofdate.md)
    
- [Hasが処理されました](hasbeenprocessed.md)
    
- [ResponseType](responsetype.md)
    
- [IntendedFreeBusyStatus](intendedfreebusystatus.md)
    
- [開始](start.md)
    
- [終わり](end-ex15websvcsotherref.md)
    
- [場所](location.md)
    
- [Organizer](organizer.md)
    
- [メールボックス](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (非 Emptystringtype)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a>SyncFolderItems エラー応答

### <a name="description"></a>説明

次の例は、SyncFolderItems 要求に対するエラー応答を示しています。 このエラーは、無効な SyncState が原因で発生しました。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

