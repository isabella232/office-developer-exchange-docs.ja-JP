---
title: GetSharingFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: GetSharingFolder 操作は、指定された共有フォルダーのローカルフォルダー識別子を取得します。
ms.openlocfilehash: cf66eb390b0287e89bb8402f26a2e728868a2b18
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460513"
---
# <a name="getsharingfolder-operation"></a>GetSharingFolder 操作

**Getsharingfolder**操作は、指定された共有フォルダーのローカルフォルダー識別子を取得します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**Getsharingfolder**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
   
## <a name="getsharingfolder-request-example"></a>GetSharingFolder 要求の例

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a>共有するフォルダーの SharedFolderId 要素を指定して、ローカルフォルダーの識別子を取得する

次のコード例は、共有されているフォルダーに対応するローカルフォルダーの識別子を取得する要求を形成する方法を示しています。 共有されているフォルダーは、共有されるフォルダーが含まれているメールボックスの SMTP アドレスと、そのフォルダーの識別子を表す[SharedFolderId](sharedfolderid.md)要素によって識別されます。 この例では、共有されているフォルダーが user1@contoso.com によって所有されています。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a>共有するフォルダーの DataType 要素を指定してローカルフォルダーの識別子を取得する

次のコード例は、共有されているフォルダーに対応するローカルフォルダーの識別子を取得する要求を形成する方法を示しています。 共有されているフォルダーは、共有されるフォルダーが含まれているメールボックスの SMTP アドレスと、そのフォルダー内のデータの種類を表す[DataType](datatype.md)要素によって識別されます。 この例では、共有されているフォルダーは、user1@contoso.com によって所有されている連絡先フォルダーです。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

**Datatype**要素に指定できる値の詳細については、「 [datatype](datatype.md)」を参照してください。
  
## <a name="successful-getsharingfolder-response"></a>成功した GetSharingFolder 応答

### <a name="description"></a>説明

次の例は、 **Getsharingfolder**要求に対する正常な応答を示しています。 [SharingFolderId](sharingfolderid.md)要素の**Id**属性は、共有関係のローカルフォルダーの識別子を表します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a>GetSharingFolder エラー応答

### <a name="description"></a>説明

次の例は、 **Getsharingfolder**要求に対するエラー応答を示しています。 この例では、要求で[SharingFolderId](sharingfolderid.md)要素と[DataType](datatype.md)要素の両方が指定されているため、エラーが発生しました。 これら2つの要素のどちらか一方のみを指定できますが、両方を指定することはできません。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[GetSharingFolder](getsharingfolder.md)
  
[GetSharingFolderType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md)
  
[GetSharingFolderResponseMessageType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[Exchange での EWS 操作](ews-operations-in-exchange.md)
  
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

