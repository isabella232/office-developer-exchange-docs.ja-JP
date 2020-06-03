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
# <a name="getsharingmetadata-operation"></a><span data-ttu-id="8bcc4-103">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="8bcc4-103">GetSharingMetadata operation</span></span>

<span data-ttu-id="8bcc4-104">**Getsharingmetadata**操作は、共有への招待を識別する非透過の認証トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-104">The **GetSharingMetadata** operation gets an opaque authentication token that identifies a sharing invitation.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="8bcc4-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bcc4-105">SOAP Headers</span></span>

<span data-ttu-id="8bcc4-106">**Getsharingmetadata**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-106">The **GetSharingMetadata** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="8bcc4-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="8bcc4-107">**Header**</span></span>|<span data-ttu-id="8bcc4-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="8bcc4-108">**Element**</span></span>|<span data-ttu-id="8bcc4-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="8bcc4-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8bcc4-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="8bcc4-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="8bcc4-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8bcc4-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8bcc4-112">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="8bcc4-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="8bcc4-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="8bcc4-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8bcc4-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8bcc4-115">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingmetadata-request-example"></a><span data-ttu-id="8bcc4-116">GetSharingMetadata 要求の例</span><span class="sxs-lookup"><span data-stu-id="8bcc4-116">GetSharingMetadata request example</span></span>

### <a name="description"></a><span data-ttu-id="8bcc4-117">Description</span><span class="sxs-lookup"><span data-stu-id="8bcc4-117">Description</span></span>

<span data-ttu-id="8bcc4-118">次の例は、共有への招待を識別する非透過の認証トークンを取得する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-118">The following example shows how to form a request to get an opaque authentication token that identifies a sharing invitation.</span></span> <span data-ttu-id="8bcc4-119">この例では、user1@contoso.com は、 [IdOfFolderToShare](idoffoldertoshare.md)要素によって指定されたフォルダーを user1@fabikam.com および user2@test.com で共有したいと考えています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-119">In this example, user1@contoso.com wants to share the folder that is specified by the [IdOfFolderToShare](idoffoldertoshare.md) element with user1@fabikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8bcc4-120">コード</span><span class="sxs-lookup"><span data-stu-id="8bcc4-120">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="8bcc4-121">コメント</span><span class="sxs-lookup"><span data-stu-id="8bcc4-121">Comments</span></span>

<span data-ttu-id="8bcc4-122">[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md)要素には、共有への招待の対象となる受信者ごとに1つの[smtpaddress](smtpaddress.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-122">The [Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) element contains one [SmtpAddress](smtpaddress.md) element for each intended recipient of the sharing invitation.</span></span> 
  
## <a name="successful-getsharingmetadata-response"></a><span data-ttu-id="8bcc4-123">正常な GetSharingMetadata 応答</span><span class="sxs-lookup"><span data-stu-id="8bcc4-123">Successful GetSharingMetadata Response</span></span>

### <a name="description"></a><span data-ttu-id="8bcc4-124">Description</span><span class="sxs-lookup"><span data-stu-id="8bcc4-124">Description</span></span>

<span data-ttu-id="8bcc4-125">次の例は、 **Getsharingmetadata**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-125">The following example shows a successful response to a **GetSharingMetadata** request.</span></span> <span data-ttu-id="8bcc4-126">この例では、対応する**Getsharingmetadata**要求で2人の受信者が指定されています。 user1@fabrikam.com および user2@test.com。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-126">In this example, two recipients were specified in the corresponding **GetSharingMetadata** request: user1@fabrikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8bcc4-127">コード</span><span class="sxs-lookup"><span data-stu-id="8bcc4-127">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="8bcc4-128">コメント</span><span class="sxs-lookup"><span data-stu-id="8bcc4-128">Comments</span></span>

<span data-ttu-id="8bcc4-129">応答には、 **Getsharingmetadata**要求で指定されている有効な受信者によって表される各組織に対して、1つの[Encryptedsharedfolderdata](encryptedsharedfolderdata.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-129">The response contains one [EncryptedSharedFolderData](encryptedsharedfolderdata.md) element for each organization that is represented by valid recipients that are specified in the **GetSharingMetadata** request.</span></span> 
  
<span data-ttu-id="8bcc4-130">**Getsharingmetadata**要求は、要求で無効な受信者が指定されていても、成功します。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-130">The **GetSharingMetadata** request will succeed even if invalid recipients are specified in the request.</span></span> <span data-ttu-id="8bcc4-131">[Invalidrecipients](invalidrecipients.md)要素には、無効な受信者に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-131">The [InvalidRecipients](invalidrecipients.md) element contains information about invalid recipients.</span></span> <span data-ttu-id="8bcc4-132">受信者が無効である可能性がある理由については、「//」を[参照して](responsecode-invalidrecipientresponsecodetype.md)ください。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-132">For information about the reasons why a recipient might be invalid, see [ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md).</span></span>
  
<span data-ttu-id="8bcc4-133">指定したすべての受信者が無効な場合、 [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md)要素は空になります。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-133">If all intended recipients are invalid, the [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) element will be empty.</span></span> 
  
## <a name="getsharingmetadata-error-response"></a><span data-ttu-id="8bcc4-134">GetSharingMetadata エラー応答</span><span class="sxs-lookup"><span data-stu-id="8bcc4-134">GetSharingMetadata error response</span></span>

### <a name="description"></a><span data-ttu-id="8bcc4-135">Description</span><span class="sxs-lookup"><span data-stu-id="8bcc4-135">Description</span></span>

<span data-ttu-id="8bcc4-136">次の例は、 **Getsharingmetadata**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8bcc4-136">The following example shows an error response to a **GetSharingMetadata** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8bcc4-137">コード</span><span class="sxs-lookup"><span data-stu-id="8bcc4-137">Code</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8bcc4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="8bcc4-138">See also</span></span>



[<span data-ttu-id="8bcc4-139">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="8bcc4-139">GetSharingMetadata</span></span>](getsharingmetadata.md)
  
[<span data-ttu-id="8bcc4-140">GetSharingMetadataType</span><span class="sxs-lookup"><span data-stu-id="8bcc4-140">GetSharingMetadataType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataType.aspx)
  
[<span data-ttu-id="8bcc4-141">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8bcc4-141">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md)
  
[<span data-ttu-id="8bcc4-142">GetSharingMetadataResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="8bcc4-142">GetSharingMetadataResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataResponseMessageType.aspx)


[<span data-ttu-id="8bcc4-143">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="8bcc4-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="8bcc4-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8bcc4-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

