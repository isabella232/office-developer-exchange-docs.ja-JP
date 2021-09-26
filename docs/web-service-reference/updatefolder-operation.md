---
title: UpdateFolder 操作
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: UpdateFolder 操作は、アイテム ストア内の既存のアイテムのプロパティを変更Exchangeされます。 各 UpdateFolder 操作は、次の操作で構成されます。
ms.openlocfilehash: be8e39e13681cea34e312158c348c60a94374bec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541764"
---
# <a name="updatefolder-operation"></a>UpdateFolder 操作

UpdateFolder 操作は、アイテム ストア内の既存のアイテムのプロパティを変更Exchangeされます。 各 UpdateFolder 操作は、次の操作で構成されます。
  
- 更新 [するフォルダー](folderid.md) を指定する FolderId 要素。 
    
- フォルダー図形で指定されたフォルダー内の要素の内部パスで、更新するデータを指定します。
    
- 更新が削除ではない場合、更新されたフィールドの新しい値を含むフォルダー。
    
## <a name="remarks"></a>注釈

アイテムに対して 3 つの基本的な更新アクションを実行できます。 これらのアクションの一覧を次の表に示します。
  
|**操作**|**説明**|
|:-----|:-----|
|追加  <br/> |append アクションは、既存のプロパティにデータを追加します。 現在のデータが保持されます。 Append は、すべてのプロパティに適用できるとは言えな。  <br/> |
|Set  <br/> |set アクションは、データが含まれている場合はプロパティのデータを置き換えるか、プロパティを作成し、存在しない場合は値を設定します。 set アクションは、書き込み可能なプロパティにのみ適用されます。  <br/> |
|削除  <br/> |削除アクションは、フォルダーからプロパティを削除します。 これは、空の値に設定するのとは異なります。 完了すると、フォルダーのプロパティは存在しません。 Delete は書き込み可能なプロパティにのみ適用されます。  <br/> |
   
## <a name="updatefolder-request-example"></a>UpdateFolder 要求の例

### <a name="description"></a>説明

UpdateFolder 要求の次の例は、フォルダー表示名を更新する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

次の使用例は、フォルダーの表示名を NewFolderName に変更します。
  
> [!NOTE]
> [FolderId](folderid.md)要素 **の Id** 属性と **ChangeKey** 属性の値は、読みやすさのために短縮されています。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Updates (Folder)](updates-folder.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (string)](displayname-string.md)
    
UpdateFolder 要求の形成に使用できる追加の要素については、スキーマを参照してください。
  
> [!NOTE]
> スキーマの既定の場所は、クライアント アクセス サーバーの役割がインストールされているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="updatefolder-response-example"></a>UpdateFolder 応答の例

### <a name="description"></a>説明

次の例は、UpdateFolder 要求に対する正常な応答を示しています。 この例では、新しい変更キーが返され、フォルダーの更新された状態が反映されます。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを維持するために短縮されました。 
  
応答で返されるフォルダー ID は、更新されたフォルダーを表します。
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>UpdateFolder エラー応答の例

### <a name="description"></a>説明

次の例は、UpdateFolder 要求に対するエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

次の使用例は、要求の **ChangeKey** 属性が無効な場合に発生するエラー応答を示しています。 
  
### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

