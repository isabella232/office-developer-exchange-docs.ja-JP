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
description: GetSharingMetadata 操作は、共有への招待を識別する不透明な認証トークンを取得します。
ms.openlocfilehash: e2e04d83310e7a8a731cca655a432325574cd9e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831671"
---
# <a name="getsharingmetadata-operation"></a><span data-ttu-id="60210-103">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="60210-103">GetSharingMetadata operation</span></span>

<span data-ttu-id="60210-104">**GetSharingMetadata**操作は、共有への招待を識別する不透明な認証トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="60210-104">The **GetSharingMetadata** operation gets an opaque authentication token that identifies a sharing invitation.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="60210-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60210-105">SOAP Headers</span></span>

<span data-ttu-id="60210-106">**GetSharingMetadata**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="60210-106">The **GetSharingMetadata** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="60210-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="60210-107">**Header**</span></span>|<span data-ttu-id="60210-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="60210-108">**Element**</span></span>|<span data-ttu-id="60210-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="60210-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="60210-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="60210-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="60210-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="60210-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="60210-112">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="60210-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="60210-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="60210-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="60210-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="60210-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="60210-115">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="60210-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingmetadata-request-example"></a><span data-ttu-id="60210-116">GetSharingMetadata 要求の例</span><span class="sxs-lookup"><span data-stu-id="60210-116">GetSharingMetadata request example</span></span>

### <a name="description"></a><span data-ttu-id="60210-117">説明</span><span class="sxs-lookup"><span data-stu-id="60210-117">Description</span></span>

<span data-ttu-id="60210-118">次の例では、共有への招待を識別する不透明な認証トークンを取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="60210-118">The following example shows how to form a request to get an opaque authentication token that identifies a sharing invitation.</span></span> <span data-ttu-id="60210-119">この例では、user1@contoso.com は user1@fabikam.com と user2@test.com と[IdOfFolderToShare](idoffoldertoshare.md)の要素で指定されているフォルダーを共有しようとします。</span><span class="sxs-lookup"><span data-stu-id="60210-119">In this example, user1@contoso.com wants to share the folder that is specified by the [IdOfFolderToShare](idoffoldertoshare.md) element with user1@fabikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="60210-120">コード</span><span class="sxs-lookup"><span data-stu-id="60210-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="60210-121">コメント</span><span class="sxs-lookup"><span data-stu-id="60210-121">Comments</span></span>

<span data-ttu-id="60210-122">[受信者 (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md)の要素には、指定された共有への招待の受信者の 1 つの[SmtpAddress](smtpaddress.md)要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="60210-122">The [Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) element contains one [SmtpAddress](smtpaddress.md) element for each intended recipient of the sharing invitation.</span></span> 
  
## <a name="successful-getsharingmetadata-response"></a><span data-ttu-id="60210-123">GetSharingMetadata の正常な応答</span><span class="sxs-lookup"><span data-stu-id="60210-123">Successful GetSharingMetadata Response</span></span>

### <a name="description"></a><span data-ttu-id="60210-124">説明</span><span class="sxs-lookup"><span data-stu-id="60210-124">Description</span></span>

<span data-ttu-id="60210-125">**GetSharingMetadata**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60210-125">The following example shows a successful response to a **GetSharingMetadata** request.</span></span> <span data-ttu-id="60210-126">この例では、2 人の受信者は、対応する**GetSharingMetadata**要求で指定された: user1@fabrikam.com と user2@test.com。</span><span class="sxs-lookup"><span data-stu-id="60210-126">In this example, two recipients were specified in the corresponding **GetSharingMetadata** request: user1@fabrikam.com and user2@test.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="60210-127">コード</span><span class="sxs-lookup"><span data-stu-id="60210-127">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingMetadataResponseMessage ResponseClass="Success" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="60210-128">コメント</span><span class="sxs-lookup"><span data-stu-id="60210-128">Comments</span></span>

<span data-ttu-id="60210-129">応答には、 **GetSharingMetadata**要求で指定されている有効な受信者で表されるそれぞれの組織の 1 つの[EncryptedSharedFolderData](encryptedsharedfolderdata.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60210-129">The response contains one [EncryptedSharedFolderData](encryptedsharedfolderdata.md) element for each organization that is represented by valid recipients that are specified in the **GetSharingMetadata** request.</span></span> 
  
<span data-ttu-id="60210-130">無効な受信者が要求で指定されている場合でも、 **GetSharingMetadata**の要求は成功します。</span><span class="sxs-lookup"><span data-stu-id="60210-130">The **GetSharingMetadata** request will succeed even if invalid recipients are specified in the request.</span></span> <span data-ttu-id="60210-131">[InvalidRecipients](invalidrecipients.md)要素には、無効な受信者に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60210-131">The [InvalidRecipients](invalidrecipients.md) element contains information about invalid recipients.</span></span> <span data-ttu-id="60210-132">なぜ、受信者が無効である理由については、 [ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60210-132">For information about the reasons why a recipient might be invalid, see [ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md).</span></span>
  
<span data-ttu-id="60210-133">すべての受信者が無効である場合、 [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md)要素は空になります。</span><span class="sxs-lookup"><span data-stu-id="60210-133">If all intended recipients are invalid, the [EncryptedSharedFolderDataCollection](encryptedsharedfolderdatacollection.md) element will be empty.</span></span> 
  
## <a name="getsharingmetadata-error-response"></a><span data-ttu-id="60210-134">GetSharingMetadata エラー応答</span><span class="sxs-lookup"><span data-stu-id="60210-134">GetSharingMetadata error response</span></span>

### <a name="description"></a><span data-ttu-id="60210-135">説明</span><span class="sxs-lookup"><span data-stu-id="60210-135">Description</span></span>

<span data-ttu-id="60210-136">**GetSharingMetadata**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60210-136">The following example shows an error response to a **GetSharingMetadata** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="60210-137">コード</span><span class="sxs-lookup"><span data-stu-id="60210-137">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingMetadataResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>The SMTP address format is invalid.</MessageText>
      <m:ResponseCode>ErrorInvalidSmtpAddress</ResponseCode>
      <m:DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetSharingMetadataResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="60210-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="60210-138">See also</span></span>



[<span data-ttu-id="60210-139">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="60210-139">GetSharingMetadata</span></span>](getsharingmetadata.md)
  
[<span data-ttu-id="60210-140">GetSharingMetadataType</span><span class="sxs-lookup"><span data-stu-id="60210-140">GetSharingMetadataType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataType.aspx)
  
[<span data-ttu-id="60210-141">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="60210-141">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md)
  
[<span data-ttu-id="60210-142">GetSharingMetadataResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="60210-142">GetSharingMetadataResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingMetadataResponseMessageType.aspx)


[<span data-ttu-id="60210-143">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="60210-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="60210-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="60210-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

