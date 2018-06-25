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
description: UpdateFolder 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。 各 UpdateFolder 操作は、次ので構成されます。
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839836"
---
# <a name="updatefolder-operation"></a>UpdateFolder 操作

UpdateFolder 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。 各 UpdateFolder 操作は、次ので構成されます。
  
- [フォルダー Id](folderid.md)の要素で、更新するフォルダーを指定します。 
    
- 更新するデータを指定するフォルダーの図形で指定したフォルダー内の要素の内部のパスです。
    
- 更新プログラムが削除できない場合、更新されたフィールドの新しい値を格納するフォルダーです。
    
## <a name="remarks"></a>備考

アイテムには、3 つの更新プログラムの基本的な操作を実行できます。 これらのアクションは、次の表に表示されます。
  
|**アクション**|**説明**|
|:-----|:-----|
|追加  <br/> |追加操作では、既存のプロパティにデータを追加します。 そこにある現在のデータが保持されます。 追加のすべてのプロパティには適用できません。  <br/> |
|設定  <br/> |設定のアクションでは、データが含まれていますまたはプロパティが作成され、存在しない場合、その値を設定する場合、プロパティのデータが置き換えられます。 アクションのセットは、書き込み可能なプロパティに適用できるのみです。  <br/> |
|削除  <br/> |削除操作では、フォルダーからプロパティを削除します。 これは、空の値を設定することとは異なります。 完了すると、フォルダーのプロパティが存在しません。 削除は、書き込み可能なプロパティに該当する場合のみです。  <br/> |
   
## <a name="updatefolder-request-example"></a>UpdateFolder 要求の例

### <a name="description"></a>説明

UpdateFolder 要求の次の使用例は、フォルダーの表示名を更新する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

NewFolderName] にフォルダーの表示名を変更します。
  
> [!NOTE]
> [フォルダー Id](folderid.md)要素の属性を**変更キー**と**Id**の値は、読みやすさに短縮されています。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [UpdateFolder](updatefolder.md)
    
- [FolderChanges](folderchanges.md)
    
- [FolderChange](folderchange.md)
    
- [フォルダー Id](folderid.md)
    
- [更新 (アイテム)](updates-item.md)
    
- [SetFolderField](setfolderfield.md)
    
- [FieldURI](fielduri.md)
    
- [Folder](folder.md)
    
- [表示名 (文字列)](displayname-string.md)
    
UpdateFolder 要求を形成するために使用できるその他の要素のスキーマを参照してください。
  
> [!NOTE]
> スキーマの既定の場所は、クライアント アクセス サーバーの役割がインストールされているコンピューターで EWS 仮想ディレクトリには。 
  
## <a name="updatefolder-response-example"></a>UpdateFolder 応答の例

### <a name="description"></a>説明

UpdateFolder 要求に正常な応答の例を次に示します。 この例では、フォルダーの更新されたステータスを反映するために新しいキーの変更が返されます。
  
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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。 
  
応答で返されたフォルダー ID は、更新されたフォルダーを表します。
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateFolderResponse](updatefolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateFolderResponseMessage](updatefolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
## <a name="updatefolder-error-response-example"></a>UpdateFolder エラー応答の例

### <a name="description"></a>説明

UpdateFolder 要求に対するエラー応答の例を次に示します。
  
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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

この例では、要求に無効な**変更キー**属性が原因で発生するエラー応答を使用します。 
  
### <a name="error-response-elements"></a>エラー応答の要素

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



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

