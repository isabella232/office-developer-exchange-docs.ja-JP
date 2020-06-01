---
title: FindFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: FindFolder 操作は、Exchange Web サービスを使用して、識別されたフォルダーのサブフォルダーを検索し、一連のサブフォルダーを記述する一連のプロパティを返します。
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462585"
---
# <a name="findfolder-operation"></a>FindFolder 操作

**Findfolder**操作は、Exchange Web サービスを使用して、識別されたフォルダーのサブフォルダーを検索し、一連のサブフォルダーを記述する一連のプロパティを返します。 
  
## <a name="remarks"></a>注釈

FindFolder は、任意のストリーミング可能なプロパティの最初の 512 バイトだけを返します。 Unicode の場合は、Null 終了の Unicode 文字列を使用して最初の 255 文字を返します。
  
ディープトラバースクエリは、パブリックフォルダーでは実行できません。
  
制限は許可され、アイテムのプロパティではなく、フォルダーのプロパティのみを使用する必要があります。 **Findfolder**応答では、並べ替え機能を使用できません。 グループ化されたクエリは、 **Findfolder**クエリでは使用できません。 
  
 **メモ****Findfolder**操作は、管理フォルダーを検索するためにも使用されます。 
  
### <a name="soap-headers"></a>SOAP ヘッダー

**Findfolder**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイムゾーンを指定します。  <br/> |
   
## <a name="findfolder-request-example"></a>FindFolder 要求の例

### <a name="description"></a>説明

**Findfolder**要求の次の例は、受信トレイ内のすべてのフォルダーを検索するための要求を形成する方法を示しています。 
  
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

[Baseshape](baseshape.md)の既定値を使用すると、応答はフォルダー名、フォルダー ID、サブフォルダー数、フォルダー内で見つかった子フォルダーの数、未読アイテムの数を返します。
  
### <a name="request-elements"></a>Request 要素

この**Findfolder**要求には、次の要素が含まれています。 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 **Findfolder**要求の追加要素については、スキーマを参照してください。 
  
## <a name="findfolder-response-example"></a>FindFolder 応答の例

### <a name="description"></a>説明

次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、 **Findfolder**要求に対する正常な応答を示しています。 応答には、 [Baseshape](baseshape.md)の既定値が使用されたときに返される要素が含まれています。 
  
> [!NOTE]
> 読みやすくするために、フォルダー ID と変更キーが短縮されています。 
  
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

### <a name="response-elements"></a>Response 要素

応答で返されるプロパティは、使用されている場合は[Baseshape](baseshape.md)および[additionalproperties](additionalproperties.md)によって決まります。 正常な**Findfolder**応答には、次の要素が含まれています。 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (文字列)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>コメント

 **Allproperties**応答図形を使用した要求に対する**findfolder**応答では、パブリックフォルダー検索の[totalcount](totalcount.md)要素と[UnreadCount](unreadcount.md)要素は返されません。 
  
## <a name="findfolder-error-response-example"></a>FindFolder エラー応答の例

### <a name="description"></a>説明

次の SOAP 本文の例は、無効なフォルダーの識別子によって識別されるフォルダーを検索すると発生するエラー応答を示しています。
  
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

**Findfolder**エラー応答には、次の要素が含まれています。 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>追加情報

- Folder [DisplayName (string)](displayname-string.md)要素は、常に既定の図形に含まれています。 
    
- [UnreadCount](unreadcount.md)要素は、タスクフォルダーとメモフォルダーに含まれています。 
    
- [ExtendedFieldURI](extendedfielduri.md)要素を使用して、管理フォルダーを識別するには、プロパティの種類が**Integer**の**Propertytag**の値0x672d を使用します。 
    
## <a name="see-also"></a>関連項目



[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

