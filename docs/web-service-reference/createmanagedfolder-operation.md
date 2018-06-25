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
description: CreateManagedFolder 操作は、Exchange ストア内の管理フォルダーを作成します。
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759851"
---
# <a name="createmanagedfolder-operation"></a>CreateManagedFolder 操作

CreateManagedFolder 操作は、Exchange ストア内の管理フォルダーを作成します。
  
## <a name="using-the-createmanagedfolder-operation"></a>CreateManagedFolder 操作を使用します。

CreateManagedFolder 操作では、ユーザーのメールボックスに管理されたカスタム フォルダーを追加します。 **Get ManagedFolder**の Exchange 管理シェル コマンドレットを使用するには追加するのには使用可能な管理対象のフォルダーを検索します。 このコマンドレットを返します管理されたカスタム フォルダーと管理された既定フォルダーの両方、のみ管理カスタム フォルダーを追加することができます。 管理されたカスタム フォルダーは、ManagedCustomFolder フォルダーの種類によって識別されます。 System.DirectoryServices 名前空間には、利用可能な管理対象フォルダーの名前を検出するために使用する型も含まれています。 
  
> [!NOTE]
> メールボックスに追加する利用可能な管理対象のフォルダーの名前を検索するのには、Exchange Web サービスを使うことはできません。 
  
FindFolder、GetFolder の操作を使用するには管理対象のフォルダーにアクセスします。 FindFolder を使用して、指定された親フォルダー内のフォルダーを検索します。 これは、重複して同じディレクトリに、カスタム フォルダーの管理を追加する前にフォルダー内の管理フォルダーを検出できるように、使用できます。 FindFolder 操作の完了後は、GetFolder を使用して管理されたカスタム フォルダーの詳細を取得します。
  
## <a name="remarks"></a>備考

メッセージング レコード管理 (MRM) ポリシーを設定する方法の詳細については、[管理フォルダー メールボックス ポリシーを作成する方法](http://go.microsoft.com/fwlink/?LinkId=100975)を参照してください。
  
管理されたカスタム フォルダーをメールボックスから削除する方法の詳細については、[削除 ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976)を参照してください。
  
## <a name="createmanagedfolder-request-example"></a>CreateManagedFolder 要求の例

### <a name="description"></a>説明

CreateManagedFolder 要求の次の例では、テストの管理フォルダーをという名前のメールボックスに管理フォルダーを追加する方法を示します。
  
> [!NOTE]
> 管理されたカスタム フォルダーを追加するのには代理人アクセスを使用することもできます。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [表示](foldernames.md)
    
- [フォルダー名](foldername.md)
    
CreateManagedFolder 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [CreateManagedFolder](createmanagedfolder.md)要素から開始します。 
  
## <a name="successful-createmanagedfolder-response"></a>CreateManagedFolder の正常な応答

### <a name="description"></a>説明

CreateManagedFolder 要求に正常な応答を次のコード例に示します。
  
> [!NOTE]
> **Id**と**変更キー**の属性の値は、読みやすさを保持するために短縮されています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
CreateManagedFolder 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。 [CreateManagedFolderResponse](createmanagedfolderresponse.md)要素から開始します。 
  
## <a name="createmanagedfolder-error-response"></a>CreateManagedFolder エラー応答

### <a name="description"></a>説明

CreateManagedFolder 要求に対してエラー応答をコード例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>エラー応答の要素

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


[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

