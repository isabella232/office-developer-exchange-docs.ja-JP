---
title: GetFederationInformation 操作 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: GetFederationInformation 操作は、組織のフェデレーションの状態 (この組織を対象としたトークンを要求するときに使用されるターゲット URI、および組織がフェデレーションを行うその他のドメイン) についての情報を提供します。
ms.openlocfilehash: 533b2f6d282e3287f4945df56b169f5bc93ff445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455626"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="4cd90-103">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="4cd90-104">**GetFederationInformation**操作は、組織のフェデレーションの状態 (この組織を対象としたトークンを要求するときに使用されるターゲット URI、および組織がフェデレーションを行うその他のドメイン) についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4cd90-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="4cd90-105">外部ユーザーに予定表、連絡先、メッセージを共有できるのは、フェデレーション組織のみです。</span><span class="sxs-lookup"><span data-stu-id="4cd90-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="4cd90-106">GetFederationInformation 要求の例</span><span class="sxs-lookup"><span data-stu-id="4cd90-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="4cd90-107">説明</span><span class="sxs-lookup"><span data-stu-id="4cd90-107">Description</span></span>

<span data-ttu-id="4cd90-108">**GetFederationInformation**要求の次の例は、ユーザーのフェデレーション情報の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="4cd90-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="4cd90-109">クライアントは、この要求をサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="4cd90-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4cd90-110">コード</span><span class="sxs-lookup"><span data-stu-id="4cd90-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="4cd90-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="4cd90-111">Request elements</span></span>

<span data-ttu-id="4cd90-112">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4cd90-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4cd90-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="4cd90-114">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="4cd90-115">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="4cd90-116">GetFederationInformation response の例</span><span class="sxs-lookup"><span data-stu-id="4cd90-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="4cd90-117">説明</span><span class="sxs-lookup"><span data-stu-id="4cd90-117">Description</span></span>

<span data-ttu-id="4cd90-118">次の例は、サーバーがクライアントに送信する**GetFederationInformation**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="4cd90-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4cd90-119">コード</span><span class="sxs-lookup"><span data-stu-id="4cd90-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="4cd90-120">Response 要素</span><span class="sxs-lookup"><span data-stu-id="4cd90-120">Response elements</span></span>

<span data-ttu-id="4cd90-121">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4cd90-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4cd90-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="4cd90-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="4cd90-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="4cd90-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="4cd90-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="4cd90-127">Domains (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="4cd90-128">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="4cd90-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4cd90-129">See also</span></span>

- [<span data-ttu-id="4cd90-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="4cd90-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4cd90-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

