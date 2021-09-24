---
title: EmptyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: EmptyFolder 操作では、メールボックス内のフォルダーが空になります。 必要に応じて、この操作を使用すると、指定したフォルダーのサブフォルダーを削除できます。 サブフォルダーを削除すると、サブフォルダーとサブフォルダー内のメッセージが削除されます。
ms.openlocfilehash: 8191dc7ecea7038a6d885f30d08fe561a59c4ed2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519668"
---
# <a name="emptyfolder-operation"></a>EmptyFolder 操作

**EmptyFolder 操作では**、メールボックス内のフォルダーが空になります。 必要に応じて、この操作を使用すると、指定したフォルダーのサブフォルダーを削除できます。 サブフォルダーを削除すると、サブフォルダーとサブフォルダー内のメッセージが削除されます。 
  
## <a name="emptyfolder-request-example"></a>EmptyFolder 要求の例

### <a name="description"></a>説明

次の **EmptyFolder 要求の例** は、フォルダーを空にする要求を形成する方法を示しています。 次の使用例は、識別されたフォルダーのすべてのサブフォルダーを削除します。 
  
> [!NOTE]
> [FolderId](folderid.md)要素 **の Id** 属性と **ChangeKey** 属性の値は、読みやすさのために短縮されています。 
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>コメント

この例では、フォルダーに対してハード削除を実行します。
  
フォルダーは[、FolderIds](folderids.md)要素で使用するために[、DistinguishedFolderId](distinguishedfolderid.md)要素または[FolderId](folderid.md)要素のいずれかによって識別できます。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [EmptyFolder](emptyfolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="successful-emptyfolder-response"></a>EmptyFolder 応答の成功

### <a name="description"></a>説明

次の例は **、EmptyFolder** 要求に対する正常な応答を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [EmptyFolderResponse](emptyfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [EmptyFolderResponseMessage](emptyfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="emptyfolder-error-response"></a>EmptyFolder エラー応答

### <a name="description"></a>説明

次の例は、Emptyfolder 要求に対する **エラー応答を示** しています。 エラーが作成されたのは、操作で、フォルダーストアに見つからなかったフォルダーをExchangeしました。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetFolderResponse](getfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetFolderResponseMessage](getfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

