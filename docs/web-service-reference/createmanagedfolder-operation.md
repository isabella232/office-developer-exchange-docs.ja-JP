---
title: CreateManagedFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: CreateManagedFolder 操作は、管理フォルダーを管理ストアにExchangeします。
ms.openlocfilehash: 2b00691fbaba294950a091d5caafb8054f3e2073
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536425"
---
# <a name="createmanagedfolder-operation"></a>CreateManagedFolder 操作

CreateManagedFolder 操作は、管理フォルダーを管理ストアにExchangeします。
  
## <a name="using-the-createmanagedfolder-operation"></a>CreateManagedFolder 操作の使用

CreateManagedFolder 操作は、管理されたカスタム フォルダーをユーザーのメールボックスに追加します。 管理シェル **Get-ManagedFolder** Exchangeを使用して、追加できる管理フォルダーを検索できます。 このコマンドレットは、管理されたカスタム フォルダーと管理された既定のフォルダーの両方を返しますが、追加できるのは管理されたカスタム フォルダーのみです。 管理されたカスタム フォルダーは、ManagedCustomFolder フォルダーの種類によって識別されます。 System.DirectoryServices 名前空間には、使用可能な管理フォルダーの名前を検出するために使用できる型も含まれています。 
  
> [!NOTE]
> Web サービスをExchangeして、メールボックスに追加できる管理フォルダーの名前を検索することはできません。 
  
FindFolder 操作と GetFolder 操作を使用して、管理フォルダーにアクセスできます。 FindFolder は、指定した親フォルダー内のフォルダーを検索するために使用されます。 これは、重複する管理カスタム フォルダーを同じディレクトリに追加する前に、フォルダー内で管理フォルダーを検出するために使用できます。 GetFolder は FindFolder 操作の後で、管理されたカスタム フォルダーの詳細を取得するために使用されます。
  
## <a name="remarks"></a>注釈

メッセージング レコード管理 (MRM) ポリシーを設定する方法については、「管理フォルダー メールボックス ポリシーを作成する方法 [」を参照してください](https://go.microsoft.com/fwlink/?LinkId=100975)。
  
メールボックスから管理されたカスタム フォルダーを削除する方法については [、「Remove-ManagedFolder」を参照してください](https://go.microsoft.com/fwlink/?LinkId=100976)。
  
## <a name="createmanagedfolder-request-example"></a>CreateManagedFolder 要求の例

### <a name="description"></a>説明

CreateManagedFolder 要求の次の例は、テスト管理フォルダーという名前の管理フォルダーをメールボックスに追加する方法を示しています。
  
> [!NOTE]
> 代理アクセスを使用して管理されたカスタム フォルダーを追加することもできます。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [FolderName](foldername.md)
    
CreateManagedFolder 操作の要求メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CreateManagedFolder 要素から開始](createmanagedfolder.md)します。 
  
## <a name="successful-createmanagedfolder-response"></a>CreateManagedFolder 応答の成功

### <a name="description"></a>説明

次のコード例は、CreateManagedFolder 要求に対する正常な応答を示しています。
  
> [!NOTE]
> Id **および** **ChangeKey** 属性値は、読みやすさを維持するために短縮されました。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
CreateManagedFolder 操作の応答メッセージの他のオプションを見つけるには、スキーマ階層を確認します。 [CreateManagedFolderResponse 要素から開始](createmanagedfolderresponse.md)します。 
  
## <a name="createmanagedfolder-error-response"></a>CreateManagedFolder エラー応答

### <a name="description"></a>説明

次のコード例は、CreateManagedFolder 要求に対するエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>関連項目



[GetFolder 操作](getfolder-operation.md)
  
[FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

