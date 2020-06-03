---
title: GetSharingMetadata 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: eaf29427-ecf8-4a5e-9a54-db2e6414b35e
description: GetSharingMetadata 操作は、共有への招待を識別する非透過の認証トークンを取得します。
ms.openlocfilehash: 0390b9caa7b2e9847b1e8dcdc1b911a35e3c5864
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530184"
---
# <a name="getsharingmetadata-operation"></a>GetSharingMetadata 操作

**Getsharingmetadata**操作は、共有への招待を識別する非透過の認証トークンを取得します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**Getsharingmetadata**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
   
## <a name="getsharingmetadata-request-example"></a>GetSharingMetadata 要求の例

### <a name="description"></a>Description

次の例は、共有への招待を識別する非透過の認証トークンを取得する要求を形成する方法を示しています。 この例では、user1@contoso.com は、 [IdOfFolderToShare](idoffoldertoshare.md)要素によって指定されたフォルダーを user1@fabikam.com および user2@test.com で共有したいと考えています。 
  
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
    <m:GetSharingMetadata>
      <m:IdOfFolderToShare Id="AAMkAD=" ChangeKey="AwAAA=" />
      <m:SenderSmtpAddress>user1@contoso.com</m:SenderSmtpAddress>
      <m:Recipients>
        <t:SmtpAddress>user1@fabrikam.com</t:SmtpAddress>
        <t:SmtpAddress>user2@test.com</t:SmtpAddress>
      </m:Recipients>
    </m:GetSharingMetadata>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md)要素には、共有への招待の対象となる受信者ごとに1つの[smtpaddress](smtpaddress.md)要素が含まれています。 
  
## <a name="successful-getsharingmetadata-response"></a>正常な GetSharingMetadata 応答

### <a name="description"></a>Description

次の例は、 **Getsharingmetadata**要求に対する正常な応答を示しています。 この例では、対応する**Getsharingmetadata**要求で2人の受信者が指定されています。 user1@fabrikam.com および user2@test.com。 
  
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
    <GetSharingMetadataResponseMessage ResponseClass="Success" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</ResponseCode>
      <m:EncryptedSharedFolderDataCollection>
        <t:EncryptedSharedFolderData>
          <t:Token>
            <EncryptedData Id="Assertion0" Type="http://www.w3.org/2001/04/xmlenc#Element" xmlns="http://www.w3.org/2001/04/xmlenc#">
              <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#tripledes-cbc"></EncryptionMethod>
              <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
                <EncryptedKey>
                  <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#rsa-oaep-mgf1p"></EncryptionMethod>
                  <ds:KeyInfo Id="keyinfo">
                    <wsse:SecurityTokenReference xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd">
                      <wsse:KeyIdentifier 
                                  EncodingType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary" 
                                  ValueType="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-x509-token-profile-1.0#X509SubjectKeyIdentifier">
                        B4VEEAf=
                      </wsse:KeyIdentifier>
                    </wsse:SecurityTokenReference>
                  </ds:KeyInfo>
                  <CipherData>
                    <CipherValue>GI/Dxqvw2na==</CipherValue>
                  </CipherData>
                </EncryptedKey>
              </ds:KeyInfo>
              <CipherData>
                <CipherValue>L77I7Hr06z</CipherValue>
              </CipherData>
            </EncryptedData>
          </t:Token>
          <t:Data>
            <EncryptedData Type="http://www.w3.org/2001/04/xmlenc#Element" xmlns="http://www.w3.org/2001/04/xmlenc#">
              <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#aes256-cbc" />
              <KeyInfo xmlns="http://www.w3.org/2000/09/xmldsig#">
                <EncryptedKey xmlns="http://www.w3.org/2001/04/xmlenc#">
                  <EncryptionMethod Algorithm="http://www.w3.org/2001/04/xmlenc#kw-tripledes" />
                  <KeyInfo xmlns="http://www.w3.org/2000/09/xmldsig#">
                    <KeyName>key</KeyName>
                  </KeyInfo>
                  <CipherData>
                    <CipherValue>9UgtjrHiU</CipherValue>
                  </CipherData>
                </EncryptedKey>
              </KeyInfo>
              <CipherData>
                <CipherValue>NCNsJoGtQ==</CipherValue>
              </CipherData>
            </EncryptedData>
          </t:Data>
        </t:EncryptedSharedFolderData>
      </m:EncryptedSharedFolderDataCollection>
      <m:InvalidRecipients>
        <t:InvalidRecipient>
          <t:SmtpAddress>user2@test.com</t:SmtpAddress>
          <t:ResponseCode>RecipientOrganizationNotFederated</t:ResponseCode>
          <m:MessageText>The organization of these recipients is not federated for external sharing.</m:MessageText>
        </t:InvalidRecipient>
      </m:InvalidRecipients>
    </GetSharingMetadataResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

応答には、 **Getsharingmetadata**要求で指定されている有効な受信者によって表される各組織に対して、1つの[Encryptedsharedfolderdata](encryptedsharedfolderdata.md)要素が含まれています。 
  
**Getsharingmetadata**要求は、要求で無効な受信者が指定されていても、成功します。 [Invalidrecipients](invalidrecipients.md)要素には、無効な受信者に関する情報が含まれています。 受信者が無効である可能性がある理由については、「//」を[参照して](responsecode-invalidrecipientresponsecodetype.md)ください。
  
指定したすべての受信者が無効な場合、 [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md)要素は空になります。 
  
## <a name="getsharingmetadata-error-response"></a>GetSharingMetadata エラー応答

### <a name="description"></a>Description

次の例は、 **Getsharingmetadata**要求に対するエラー応答を示しています。 
  
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
    <GetSharingMetadataResponseMessage ResponseClass="Error" 
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>The SMTP address format is invalid.</MessageText>
      <m:ResponseCode>ErrorInvalidSmtpAddress</ResponseCode>
      <m:DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetSharingMetadataResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目



[GetSharingMetadata](getsharingmetadata.md)
  
[GetSharingMetadataType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataType.aspx)
  
[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md)
  
[GetSharingMetadataResponseMessageType](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataResponseMessageType.aspx)


[Exchange での EWS 操作](ews-operations-in-exchange.md)
  
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

