---
title: CopyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: CopyFolder 操作は、メールボックス内のフォルダーをコピーします。
ms.openlocfilehash: 1f9a7a3f3ede2d3cf8f9d41677d8ce0487266f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468895"
---
# <a name="copyfolder-operation"></a>CopyFolder 操作

CopyFolder 操作は、メールボックス内のフォルダーをコピーします。
  
## <a name="using-the-copyfolder-operation"></a>CopyFolder 操作の使用

CopyFolder 操作は、 [movefolder 操作](movefolder-operation.md)に似ています。 識別されたフォルダーをコピーし、コピーしたフォルダーの**Id**および**changekey**を返します。 
  
## <a name="copyfolder-request-example"></a>CopyFolder 要求の例

### <a name="description"></a>説明

次の CopyFolder 要求の例は、フォルダーを受信トレイフォルダーにコピーする方法を示しています。
  
> [!NOTE]
> [FolderId](folderid.md)要素の**Id**属性の値は、読みやすくするために短縮されています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

フォルダーは、 [ToFolderId](tofolderid.md)または[FolderIds](folderids.md)要素で使用するために、 [DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderId](folderid.md)要素のいずれかで識別できます。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [CopyFolder](copyfolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
CopyFolder 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Copyfolder](copyfolder.md)要素から開始します。 
  
## <a name="successful-copyfolder-response"></a>成功した CopyFolder 応答

### <a name="description"></a>説明

次の例は、CopyFolder 要求に対する正常な応答を示しています。 
  
> [!NOTE]
> 読みやすくするために、フォルダー ID と変更キーが短縮されています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>コメント

応答で返される[FolderId](folderid.md)要素は、新しいフォルダーの場所にコピーされたフォルダーを表します。 
  
### <a name="response-elements"></a>Response 要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
CopyFolder 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Copyfolderresponse](copyfolderresponse.md)要素から開始します。 
  
## <a name="copyfolder-error-response"></a>CopyFolder エラー応答

### <a name="description"></a>説明

次の例は、CopyFolder 要求に対するエラー応答を示しています。 同じ表示名のフォルダーが既に存在するため、エラーが発生しました。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
CopyFolder 操作のエラー応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Copyfolderresponse](copyfolderresponse.md)要素から開始します。 
  
## <a name="see-also"></a>関連項目

- [MoveFolder 操作](movefolder-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

