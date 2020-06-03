---
title: UpdateFolder 操作
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: UpdateFolder 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。 各 UpdateFolder 操作は、次の要素で構成されます。
ms.openlocfilehash: fb894d9f42358b67f81e9fe8ae41ba61e6f46460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467362"
---
# <a name="updatefolder-operation"></a>UpdateFolder 操作

UpdateFolder 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。 各 UpdateFolder 操作は、次の要素で構成されます。
  
- 更新するフォルダーを指定する[FolderId](folderid.md)要素。 
    
- Folder 図形で指定された、フォルダー内の要素の内部パス。更新するデータを指定します。
    
- 更新が削除されていない場合は、更新されたフィールドの新しい値を含むフォルダー。
    
## <a name="remarks"></a>注釈

アイテムに対して3つの基本的な更新操作を実行できます。 これらのアクションを次の表に示します。
  
|**操作**|**説明**|
|:-----|:-----|
|追加  <br/> |Append アクションは、既存のプロパティにデータを追加します。 現在のデータは保持されます。 追加はすべてのプロパティに適用されません。  <br/> |
|Set  <br/> |Set アクションは、データが含まれている場合はプロパティのデータを置き換えます。存在しない場合は、プロパティを作成して、その値を設定します。 Set アクションは、書き込み可能なプロパティにのみ適用されます。  <br/> |
|削除  <br/> |削除アクションは、フォルダーからプロパティを削除します。 これは、空の値に設定するのとは異なります。 完了すると、フォルダーのプロパティは存在しません。 Delete は、書き込み可能なプロパティにのみ適用されます。  <br/> |
   
## <a name="updatefolder-request-example"></a>UpdateFolder 要求の例

### <a name="description"></a>Description

次の UpdateFolder 要求の例は、フォルダーの表示名を更新する方法を示しています。 
  
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
> [FolderId](folderid.md)要素の**Id**および**changekey**属性の値は、読みやすくするために短縮されています。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges 変更](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [FolderId](folderid.md)
    
- [Updates (フォルダー)](updates-folder.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [DisplayName (文字列)](displayname-string.md)
    
UpdateFolder 要求の形成に使用できるその他の要素については、スキーマを参照してください。
  
> [!NOTE]
> スキーマの既定の場所は、クライアントアクセスサーバーの役割がインストールされているコンピューター上の EWS 仮想ディレクトリにあります。 
  
## <a name="updatefolder-response-example"></a>UpdateFolder 応答の例

### <a name="description"></a>Description

次の例は、UpdateFolder 要求に対する正常な応答を示しています。 この例では、フォルダーの更新された状態を反映するために新しい変更キーが返されます。
  
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
> 読みやすくするために、フォルダー ID と変更キーが短縮されています。 
  
応答で返されるフォルダー ID は、更新されたフォルダーを表しています。
  
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

### <a name="description"></a>Description

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

この例では、要求内の無効な**Changekey**属性によって発生するエラー応答を示します。 
  
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



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

