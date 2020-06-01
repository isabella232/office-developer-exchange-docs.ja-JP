---
title: CreateManagedFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: CreateManagedFolder 操作は、Exchange ストアに管理フォルダーを作成します。
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44444594"
---
# <a name="createmanagedfolder-operation"></a>CreateManagedFolder 操作

CreateManagedFolder 操作は、Exchange ストアに管理フォルダーを作成します。
  
## <a name="using-the-createmanagedfolder-operation"></a>CreateManagedFolder 操作の使用

CreateManagedFolder 操作は、管理されたカスタムフォルダーをユーザーのメールボックスに追加します。 Exchange 管理シェルの**Get-ManagedFolder**コマンドレットを使用して、追加できる利用可能な管理フォルダーを見つけることができます。 このコマンドレットは、管理されたカスタムフォルダーと管理された既定のフォルダーの両方を返しますが、管理されたカスタムフォルダーのみを追加できます。 管理されたカスタムフォルダーは、ManagedCustomFolder フォルダーの種類によって識別されます。 System.directoryservices 名前空間には、使用可能な管理フォルダーの名前を検出するために使用できる型も含まれています。 
  
> [!NOTE]
> Exchange Web サービスを使用して、メールボックスに追加する使用可能な管理フォルダーの名前を検索することはできません。 
  
FindFolder および GetFolder 操作を使用して、管理フォルダーにアクセスできます。 FindFolder は、指定された親フォルダー内のフォルダーを検索するために使用されます。 これは、同じディレクトリに重複した管理されたカスタムフォルダーを追加しようとする前に、フォルダーで管理フォルダーを検出できるようにするために使用できます。 GetFolder は、FindFolder 操作の後に使用され、管理されたカスタムフォルダーに関する詳細情報を取得します。
  
## <a name="remarks"></a>注釈

メッセージングレコード管理 (MRM) ポリシーを設定する方法については、「 [how To Create a Managed Folder Mailbox policy](https://go.microsoft.com/fwlink/?LinkId=100975)」を参照してください。
  
管理されたカスタムフォルダーをメールボックスから削除する方法については、「[削除-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976)」を参照してください。
  
## <a name="createmanagedfolder-request-example"></a>CreateManagedFolder 要求の例

### <a name="description"></a>説明

次の CreateManagedFolder 要求の例は、Test 管理フォルダーという名前の管理フォルダーをメールボックスに追加する方法を示しています。
  
> [!NOTE]
> 代理人アクセスを使用して、管理されたカスタムフォルダーを追加することもできます。 
  
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

### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [FolderName](foldername.md)
    
CreateManagedFolder 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [CreateManagedFolder](createmanagedfolder.md)要素から開始します。 
  
## <a name="successful-createmanagedfolder-response"></a>成功した CreateManagedFolder 応答

### <a name="description"></a>説明

次のコード例は、CreateManagedFolder 要求に対する正常な応答を示しています。
  
> [!NOTE]
> **Id**および**changekey**属性の値は、読みやすくするために短縮されています。 
  
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
    
CreateManagedFolder 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。 [CreateManagedFolderResponse](createmanagedfolderresponse.md)要素から開始します。 
  
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

