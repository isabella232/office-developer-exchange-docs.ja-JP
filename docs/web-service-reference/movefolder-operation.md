---
title: MoveFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: MoveFolder 操作は、指定したフォルダーからフォルダーを移動して、別のフォルダーに保存します。
ms.openlocfilehash: 5da6929f11ce9ba74db190db6d799f25974d2192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832490"
---
# <a name="movefolder-operation"></a>MoveFolder 操作

MoveFolder 操作は、指定したフォルダーからフォルダーを移動して、別のフォルダーに保存します。
  
## <a name="remarks"></a>備考

MoveFolder 操作は、CopyFolder 操作に似ています。 識別フォルダーを移動することはできません。 コピー先のフォルダーを同時に複数のフォルダーを移動できます。
  
## <a name="movefolder-request-example"></a>MoveFolder 要求の例

### <a name="description"></a>説明

MoveFolder 要求の次の例では、[フォルダー Id](folderid.md)で識別されるフォルダーに移動し、[迷惑メールの識別フォルダーでフォルダーを配置する要求を作成する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

> [!NOTE]
> [フォルダー Id](folderid.md)要素の ID 属性の値が小さすぎると読みやすくするためです。 
  
### <a name="request-elements"></a>要素を要求します。

MoveFolder 要求には、次の要素が含まれています。
  
- [MoveFolder](movefolder.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [FolderIds](folderids.md)
    
- [フォルダー Id](folderid.md)
    
MoveFolder 要求を形成するために使用できるその他の要素のスキーマを参照してください。
  
> [!NOTE]
> スキーマの既定の場所は、クライアント アクセス サーバーの役割がインストールされているコンピューターで EWS 仮想ディレクトリには。 
  
## <a name="successful-movefolder-response-example"></a>MoveFolder 応答の成功の例

### <a name="description"></a>説明

MoveFolder 要求に正常な応答の例を次に示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。 
  
応答で返されるフォルダー Id があったフォルダーを表す新しいフォルダーの場所に移動します。
  
### <a name="response-elements"></a>応答の要素

MoveFolder の応答には、次の要素が含まれています。
  
- [MoveFolderResponse](movefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveFolderResponseMessage](movefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
## <a name="movefolder-error-response-example"></a>MoveFolder エラー応答の例

### <a name="description"></a>説明

識別フォルダーを移動しようとするときに発生するエラー応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答の要素

MoveFolder エラー応答には、次の要素が含まれています。
  
- [MoveFolderResponse](movefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveFolderResponseMessage](movefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>関連項目



[CopyFolder 操作](copyfolder-operation.md)

