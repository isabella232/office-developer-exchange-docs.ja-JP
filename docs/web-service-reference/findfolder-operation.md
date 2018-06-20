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
description: FindFolder 操作は、Exchange Web サービスを使用して識別されたフォルダーのサブフォルダーを検索し、サブフォルダーの設定を記述するプロパティのセットを返します。
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760502"
---
# <a name="findfolder-operation"></a>FindFolder 操作

**FindFolder**操作は、Exchange Web サービスを使用して識別されたフォルダーのサブフォルダーを検索し、サブフォルダーの設定を記述するプロパティのセットを返します。 
  
## <a name="remarks"></a>備考

FindFolder は、ストリーム再生可能なプロパティの最初の 512 バイトのみを返します。 Unicode では、null で終わる Unicode 文字列を使用して、最初の 255 文字を返します。
  
パブリック フォルダーの深い階層にわたるクエリを実行できません。
  
制限は、許可およびのみ、フォルダーのプロパティ、項目のプロパティではなくを使用する必要があります。 並べ替え機能では、 **FindFolder**応答を使用できません。 **FindFolder**クエリのクエリをグループ化することはできません。 
  
 **メモ****FindFolder**操作は、管理対象のフォルダーを検索するのにも使用されます。 
  
### <a name="soap-headers"></a>SOAP ヘッダー

**FindFolder**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|偽装  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |サーバーからのすべての応答に使用するタイム ゾーンを識別します。  <br/> |
   
## <a name="findfolder-request-example"></a>FindFolder 要求の例

### <a name="description"></a>説明

**FindFolder**要求の次の例では、受信トレイ内にあるすべてのフォルダーを検索する要求を作成する方法を示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

[BaseShape](baseshape.md)の既定値を使用して、応答は、フォルダー名、フォルダー ID では、サブフォルダー、フォルダー、および未読アイテム数内の子フォルダーの数の数を返します。
  
### <a name="request-elements"></a>要素を要求します。

**FindFolder**要求には、次の要素が含まれています。 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 **FindFolder**要求の追加の要素は、スキーマを参照してください。 
  
## <a name="findfolder-response-example"></a>FindFolder 応答の例

### <a name="description"></a>説明

**FindFolder**要求に正常な応答を Simple Object Access Protocol (SOAP) 本文の例を次に示します。 応答には、 [BaseShape](baseshape.md)の既定値が使用されるときに返される要素が含まれています。 
  
> [!NOTE]
> フォルダー ID と変更キーは、読みやすさを保持するために短縮されています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a>応答の要素

応答で返されるプロパティは、使用される場合に、 [BaseShape](baseshape.md)と[AdditionalProperties](additionalproperties.md)によって決定されます。 **FindFolder**の正常な応答には、次の要素が含まれています。 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [フォルダー](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [フォルダー Id](folderid.md)
    
- [表示名 (文字列)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>コメント

 [TotalCount](totalcount.md)とパブリック フォルダーの検索の[UnreadCount](unreadcount.md)要素、 **FindFolder** **AllProperties**応答の形をした要求の応答は返されません。 
  
## <a name="findfolder-error-response-example"></a>FindFolder エラー応答の例

### <a name="description"></a>説明

不正なフォルダー id で識別されているフォルダーを検索するときに発生するエラー応答を SOAP 本文の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>エラー応答の要素

**FindFolder**エラー応答には、次の要素が含まれています。 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>その他の情報

- フォルダーの[表示名 (文字列)](displayname-string.md)の要素は常に既定の図形に含まれます。 
    
- 仕事リストとメモのフォルダーの[UnreadCount](unreadcount.md)要素が含まれます。 
    
- [ExtendedFieldURI](extendedfielduri.md)要素を使用して管理対象のフォルダーを識別するのに**整数**のプロパティの種類と 0x672D の**PropertyTag**値を使用します。 
    
## <a name="see-also"></a>関連項目



[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

