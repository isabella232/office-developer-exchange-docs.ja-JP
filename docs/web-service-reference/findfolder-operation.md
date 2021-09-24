---
title: FindFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: FindFolder 操作では、Exchange Web サービスを使用して、特定のフォルダーのサブフォルダーを検索し、一連のサブフォルダーを記述するプロパティのセットを返します。
ms.openlocfilehash: 8c2776a9d60244fe77b6012a09ffbad230d86f63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518471"
---
# <a name="findfolder-operation"></a>FindFolder 操作

**FindFolder** 操作では、Exchange Web サービスを使用して、特定のフォルダーのサブフォルダーを検索し、一連のサブフォルダーを表すプロパティのセットを返します。 
  
## <a name="remarks"></a>注釈

FindFolder は、任意のストリーミング可能なプロパティの最初の 512 バイトだけを返します。Unicode の場合は、Null 終了の Unicode 文字列を使用して最初の 255 文字を返します。
  
パブリック フォルダーでは、ディープ トラバーサル クエリを実行できません。
  
制限は許可され、アイテム のプロパティではなく、フォルダー プロパティのみを使用する必要があります。 **FindFolder** 応答では並べ替え機能を使用できません。 グループ化されたクエリは **、FindFolder クエリでは** 使用できません。 
  
 **メモ****FindFolder 操作は**、管理フォルダーの検索にも使用されます。 
  
### <a name="soap-headers"></a>SOAP ヘッダー

**FindFolder 操作では**、次の表に示す SOAP ヘッダーを使用できます。 
  
|**Header**|**Element**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC3066 カルチャを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイム ゾーンを識別します。  <br/> |
   
## <a name="findfolder-request-example"></a>FindFolder 要求の例

### <a name="description"></a>説明

**FindFolder** 要求の次の例は、受信トレイ内のすべてのフォルダーを検索する要求を形成する方法を示しています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[BaseShape](baseshape.md)の既定値を使用すると、フォルダー名、フォルダー ID、サブフォルダーの数、フォルダー内に見つかった子フォルダーの数、未読アイテムの数が返されます。
  
### <a name="request-elements"></a>要求要素

この **FindFolder 要求には** 、次の要素が含まれています。 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 追加の **FindFolder 要求** 要素については、スキーマを参照してください。 
  
## <a name="findfolder-response-example"></a>FindFolder 応答の例

### <a name="description"></a>説明

次のSimple Object Access Protocol (SOAP) 本文の例は **、FindFolder** 要求に対する正常な応答を示しています。 応答には [、BaseShape](baseshape.md) の Default 値を使用するときに返される要素が含まれます。 
  
> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを維持するために短縮されました。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>応答要素

応答で返されるプロパティは [、BaseShape](baseshape.md) と [AdditionalProperties](additionalproperties.md) が使用されている場合に決定されます。 **FindFolder 応答の成功には**、次の要素が含まれます。 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>コメント

 **AllProperties** 応答図形を持つ要求に対する **FindFolder** 応答は、パブリック フォルダー検索の [TotalCount](totalcount.md) 要素と [UnreadCount](unreadcount.md) 要素を返すことはありません。 
  
## <a name="findfolder-error-response-example"></a>FindFolder エラー応答の例

### <a name="description"></a>説明

次の SOAP 本文の例は、形式が正しいフォルダー識別子によって識別されるフォルダーを検索するときに発生するエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

**FindFolder エラー応答** には、次の要素が含まれます。 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>その他の情報

- フォルダー [DisplayName (string)](displayname-string.md) 要素は、常に既定の図形に含まれます。 
    
- [UnreadCount 要素](unreadcount.md)は、[タスク] フォルダーと [メモ] フォルダーに含まれています。 
    
- **ExtendedFieldURI** 要素を使用0x672D管理フォルダーを識別するには、**プロパティ** の種類が Integer のプロパティ プロパティの [PropertyTag 値を使用](extendedfielduri.md)します。 
    
## <a name="see-also"></a>関連項目



[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

