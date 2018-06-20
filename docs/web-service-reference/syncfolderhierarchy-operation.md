---
title: SyncFolderHierarchy 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: SyncFolderHierarchy 操作では、Microsoft Exchange Server 2010 を実行しているコンピューターとクライアントの間でフォルダーを同期します。
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839633"
---
# <a name="syncfolderhierarchy-operation"></a>SyncFolderHierarchy 操作

SyncFolderHierarchy 操作では、Microsoft Exchange Server 2010 を実行しているコンピューターとクライアントの間でフォルダーを同期します。
  
> [!NOTE]
> SyncFolderHierarchy 操作では、 [TotalCount](totalcount.md)の[UnreadCount](unreadcount.md)プロパティが変更されたとき、フォルダーは返されません。 
  
## <a name="syncfolderhierarchy-request-example"></a>SyncFolderHierarchy 要求の例

### <a name="description"></a>説明

SyncFolderHierarchy 要求の次の使用例は、Exchange サーバーとフォルダーの階層にクライアントを同期する方法を示します。 この例では、1 つ以上の時間が既に同期されているフォルダーの階層を示します。 クライアントが Exchange サーバーと同期する最初の試みの要求では、[同期状態](syncstate-ex15websvcsotherref.md)の要素は含まれません。 最初の要求は、メールボックス内のすべてのフォルダーが返されます。 [同期状態](syncstate-ex15websvcsotherref.md)の要素は、 [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)で返されます。 SyncFolderHierarchy の後続の要求の状態を同期するのにはこの要素を使用します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[同期状態](syncstate-ex15websvcsotherref.md)の要素の base64 でエンコードされたデータは読みやすさを保持するために短縮されました。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [SyncFolderHierarchy](syncfolderhierarchy.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [同期状態](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、これらの要素を記述するスキーマがあります。 
  
## <a name="successful-syncfolderhierarchy-response"></a>SyncFolderHierarchy の正常な応答

### <a name="description"></a>説明

SyncFolderHierarchy 要求に正常な応答の例を次に示します。 この例では、新しいフォルダーが同期されています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

[同期状態](syncstate-ex15websvcsotherref.md)の要素の base64 でエンコードされたデータやフォルダーの識別子のデータは、読みやすさを保持するために短縮されています。 
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [同期状態](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
- [(階層) の変更](changes-hierarchy.md)
    
- [(集合的) を作成します。](create-foldersync.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [FolderClass](folderclass.md)
    
- [表示名 (文字列)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a>SyncFolderHierarchy エラー応答

### <a name="description"></a>説明

SyncFolderHierarchy 要求に対してエラー応答の例を次に示します。 このエラーは、無効な同期状態が原因です。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>エラー応答の要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [同期状態](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

