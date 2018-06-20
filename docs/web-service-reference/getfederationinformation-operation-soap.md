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
description: GetFederationInformation 操作には、対象の URI は、この組織と組織には、また他のドメインを対象とするトークンを要求するときに使用するなど、組織のフェデレーションの状態に関する情報が用意されています。連合。
ms.openlocfilehash: bf38b2f2b3db3e38b9b0157d1677efe4fc274e1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760734"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="0e0b7-103">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="0e0b7-104">**GetFederationInformation**操作には、組織のフェデレーションの状態に関する情報が用意されています、この組織では、およびその他のドメインをターゲットなどトークンを要求するときに使用する URI が対象としている組織フェデレーションがも。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="0e0b7-105">フェデレーションの組織には、予定表、連絡先、および外部ユーザーにメッセージを共有できます。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="0e0b7-106">GetFederationInformation 要求の例</span><span class="sxs-lookup"><span data-stu-id="0e0b7-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="0e0b7-107">説明</span><span class="sxs-lookup"><span data-stu-id="0e0b7-107">Description</span></span>

<span data-ttu-id="0e0b7-108">**GetFederationInformation**要求の次の使用例は、フェデレーションのユーザーの設定情報の要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="0e0b7-109">クライアントは、この要求をサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0e0b7-110">コード</span><span class="sxs-lookup"><span data-stu-id="0e0b7-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/
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
            xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="0e0b7-111">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-111">Request elements</span></span>

<span data-ttu-id="0e0b7-112">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0e0b7-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="0e0b7-114">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="0e0b7-115">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="0e0b7-116">GetFederationInformation の応答の例</span><span class="sxs-lookup"><span data-stu-id="0e0b7-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="0e0b7-117">説明</span><span class="sxs-lookup"><span data-stu-id="0e0b7-117">Description</span></span>

<span data-ttu-id="0e0b7-118">次の例では、サーバーがクライアントに送信する**GetFederationInformation**要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0e0b7-119">コード</span><span class="sxs-lookup"><span data-stu-id="0e0b7-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
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

### <a name="response-elements"></a><span data-ttu-id="0e0b7-120">応答の要素</span><span class="sxs-lookup"><span data-stu-id="0e0b7-120">Response elements</span></span>

<span data-ttu-id="0e0b7-121">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e0b7-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0e0b7-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="0e0b7-123">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="0e0b7-124">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="0e0b7-125">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="0e0b7-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="0e0b7-127">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="0e0b7-128">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="0e0b7-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e0b7-129">See also</span></span>

- [<span data-ttu-id="0e0b7-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="0e0b7-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0e0b7-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

