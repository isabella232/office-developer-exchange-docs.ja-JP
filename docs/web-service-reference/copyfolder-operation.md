---
title: CopyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: CopyFolder 操作は、メールボックス内のフォルダーをコピーします。
ms.openlocfilehash: 7bfe9c85f3782f751e23b79afe193c9369a4720c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510337"
---
# <a name="copyfolder-operation"></a>CopyFolder 操作

CopyFolder 操作は、メールボックス内のフォルダーをコピーします。
  
## <a name="using-the-copyfolder-operation"></a>CopyFolder 操作の使用

CopyFolder 操作は [MoveFolder 操作に似ています](movefolder-operation.md)。 識別されたフォルダーをコピーし、コピーされたフォルダー **の Id** と **ChangeKey** を返します。 
  
## <a name="copyfolder-request-example"></a>CopyFolder 要求の例

### <a name="description"></a>説明

CopyFolder 要求の次の例は、フォルダーを受信トレイ フォルダーにコピーする方法を示しています。
  
> [!NOTE]
> [FolderId](folderid.md)要素 **の Id** 属性の値が、読みやすさのために短縮されました。 
  
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

フォルダーは[、ToFolderId](tofolderid.md)要素または[FolderIds](folderids.md)要素で使用するために[、DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderId](folderid.md)要素のいずれかによって識別できます。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CopyFolder](copyfolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
CopyFolder 操作の要求メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CopyFolder 要素から開始](copyfolder.md)します。 
  
## <a name="successful-copyfolder-response"></a>CopyFolder 応答の成功

### <a name="description"></a>説明

次の例は、CopyFolder 要求に対する正常な応答を示しています。 
  
> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを維持するために短縮されました。 
  
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

応答 [で返される FolderId](folderid.md) 要素は、新しいフォルダーの場所にコピーされたフォルダーを表します。 
  
### <a name="response-elements"></a>応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyFolderResponse](copyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyFolderResponseMessage](copyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
CopyFolder 操作の応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CopyFolderResponse 要素から開始](copyfolderresponse.md)します。 
  
## <a name="copyfolder-error-response"></a>CopyFolder エラー応答

### <a name="description"></a>説明

次の例は、CopyFolder 要求に対するエラー応答を示しています。 同じ表示名を持つフォルダーが既に存在していたため、エラーが発生しました。
  
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
    
CopyFolder 操作のエラー応答メッセージの他のオプションを見つけるには、スキーマ階層を参照してください。 [CopyFolderResponse 要素から開始](copyfolderresponse.md)します。 
  
## <a name="see-also"></a>関連項目

- [MoveFolder 操作](movefolder-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

