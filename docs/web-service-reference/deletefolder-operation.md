---
title: DeleteFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: DeleteFolder 操作は、メールボックスからフォルダーを削除します。
ms.openlocfilehash: e9bb9199027c2af2cbbb664ef7ad4fa70b7ef718
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455745"
---
# <a name="deletefolder-operation"></a>DeleteFolder 操作

**Deletefolder**操作は、メールボックスからフォルダーを削除します。 
  
## <a name="deletefolder-request-example"></a>DeleteFolder 要求の例

### <a name="description"></a>Description

次の**deletefolder**要求の例は、フォルダーを削除する要求を形成する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

この例では、フォルダーに対してハード削除を実行します。
  
> [!NOTE]
> フォルダー ID は読みやすくするために短縮されています。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [DeleteFolder](deletefolder.md)
    
- [FolderIds](folderids.md)
    
- [FolderId](folderid.md)
    
> [!NOTE]
> この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。 
  
**Deletefolder**操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Deletefolder](deletefolder.md)要素から開始します。 
  
## <a name="successful-deletefolder-response"></a>正常な DeleteFolder 応答

### <a name="description"></a>Description

次の例は、 **Deletefolder**要求に対する正常な応答を示しています。 
  
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
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Response 要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
**Deletefolder**操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Deletefolderresponse](deletefolderresponse.md)要素から開始します。 
  
## <a name="deletefolder-error-response"></a>DeleteFolder エラー応答

### <a name="description"></a>Description

次の例は、 **Deletefolder**要求に対するエラー応答を示しています。 このエラーは、メールボックスに存在しないフォルダーを削除する要求が原因で発生しました。 
  
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
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

**Deletefolder**操作は、識別フォルダーでは使用できません。 
  
### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteFolderResponse](deletefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteFolderResponseMessage](deletefolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
**Deletefolder**操作のエラー応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [Deletefolderresponse](deletefolderresponse.md)要素から開始します。 
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [フォルダーの削除](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

