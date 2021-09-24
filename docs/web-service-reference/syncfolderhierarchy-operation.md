---
title: SyncFolderHierarchy 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: SyncFolderHierarchy 操作では、2010 年から 2010 年まで実行されているコンピューターとクライアントMicrosoft Exchange Serverを同期します。
ms.openlocfilehash: 43182d267d4c09d4626669746ac64af9b0f890b9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513305"
---
# <a name="syncfolderhierarchy-operation"></a>SyncFolderHierarchy 操作

SyncFolderHierarchy 操作では、2010 年から 2010 年まで実行されているコンピューターとクライアントMicrosoft Exchange Serverを同期します。
  
> [!NOTE]
> SyncFolderHierarchy 操作では [、UnreadCount](unreadcount.md) プロパティまたは [TotalCount](totalcount.md) プロパティが変更された場合、フォルダーは返されません。 
  
## <a name="syncfolderhierarchy-request-example"></a>SyncFolderHierarchy 要求の例

### <a name="description"></a>説明

SyncFolderHierarchy 要求の次の例は、クライアント フォルダー階層をサーバーと同期するExchangeしています。 この例では、少なくとも 1 回は同期済みのフォルダー階層を示します。 SyncState[要素](syncstate-ex15websvcsotherref.md)は、クライアントとクライアントサーバーを同期する最初の試行の要求Exchangeされません。 最初の要求は、メールボックス内のすべてのフォルダーを返します。 [SyncState 要素](syncstate-ex15websvcsotherref.md)は[SyncFolderHierarchyResponse で返されます](syncfolderhierarchyresponse.md)。 この要素は、以降の SyncFolderHierarchy 要求の状態を同期するために使用されます。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[SyncState 要素](syncstate-ex15websvcsotherref.md)base64 でエンコードされたデータは、読みやすさを維持するために短縮されました。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [SyncFolderHierarchy](syncfolderhierarchy.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> これらの要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="successful-syncfolderhierarchy-response"></a>成功した SyncFolderHierarchy 応答

### <a name="description"></a>説明

次の例は、SyncFolderHierarchy 要求に対する正常な応答を示しています。 この例では、新しいフォルダーが同期されています。
  
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
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[SyncState 要素](syncstate-ex15websvcsotherref.md)base64 エンコード データとフォルダー識別子データは、読みやすさを維持するために短縮されました。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
- [Changes (Hierarchy)](changes-hierarchy.md)
    
- [Create (FolderSync)](create-foldersync.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [FolderClass](folderclass.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a>SyncFolderHierarchy エラー応答

### <a name="description"></a>説明

次の例は、SyncFolderHierarchy 要求に対するエラー応答を示しています。 このエラーは、無効な SyncState が原因で発生しました。
  
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
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

