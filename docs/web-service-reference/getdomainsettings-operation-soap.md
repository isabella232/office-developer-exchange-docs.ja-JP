---
title: GetDomainSettings 操作 (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: GetDomainSettings 操作は、指定したユーザーのドメインの設定を取得します。 自動検出では、検出対象のドメインとそれらのドメインの指定された設定を返します。
ms.openlocfilehash: 09b1d610cd415d2d9d7d0098354521ece86f5184
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760707"
---
# <a name="getdomainsettings-operation-soap"></a><span data-ttu-id="e3926-104">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-104">GetDomainSettings operation (SOAP)</span></span>

<span data-ttu-id="e3926-105">**GetDomainSettings**操作は、指定したユーザーのドメインの設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="e3926-105">The **GetDomainSettings** operation retrieves the specified settings of the domain for the user.</span></span> <span data-ttu-id="e3926-106">自動検出では、検出対象のドメインとそれらのドメインの指定された設定を返します。</span><span class="sxs-lookup"><span data-stu-id="e3926-106">Autodiscover returns the domains that are to be discovered and the requested settings of those domains.</span></span> 
  
## <a name="getdomainsettings-request-example"></a><span data-ttu-id="e3926-107">GetDomainSettings 要求の例</span><span class="sxs-lookup"><span data-stu-id="e3926-107">GetDomainSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="e3926-108">説明</span><span class="sxs-lookup"><span data-stu-id="e3926-108">Description</span></span>

<span data-ttu-id="e3926-109">**GetDomainSettings**要求の次の使用例は、 **ExternalEWSUrl**ドメインの設定をユーザーの要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3926-109">The following example of a **GetDomainSettings** request shows a request for a user's **ExternalEWSUrl** domain settings.</span></span> <span data-ttu-id="e3926-110">クライアントは、この要求をサーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="e3926-110">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e3926-111">コード</span><span class="sxs-lookup"><span data-stu-id="e3926-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>http://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="e3926-112">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="e3926-112">Request elements</span></span>

<span data-ttu-id="e3926-113">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e3926-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e3926-114">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-114">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="e3926-115">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-115">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="e3926-116">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-116">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="e3926-117">ドメイン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-117">Domain (SOAP)</span></span>](domain-soap.md)
    
- [<span data-ttu-id="e3926-118">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-118">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="e3926-119">(SOAP) の設定</span><span class="sxs-lookup"><span data-stu-id="e3926-119">Setting (SOAP)</span></span>](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a><span data-ttu-id="e3926-120">GetDomainSettings の応答の例</span><span class="sxs-lookup"><span data-stu-id="e3926-120">GetDomainSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="e3926-121">説明</span><span class="sxs-lookup"><span data-stu-id="e3926-121">Description</span></span>

<span data-ttu-id="e3926-122">次の例では、サーバーがクライアントに送信する**GetDomainSettings**要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="e3926-122">The following example shows a successful response to the **GetDomainSettings** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e3926-123">コード</span><span class="sxs-lookup"><span data-stu-id="e3926-123">Code</span></span>

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="e3926-124">応答の要素</span><span class="sxs-lookup"><span data-stu-id="e3926-124">Response elements</span></span>

<span data-ttu-id="e3926-125">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e3926-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e3926-126">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-126">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="e3926-127">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-127">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="e3926-128">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-128">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="e3926-129">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-129">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="e3926-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md)
    
- [<span data-ttu-id="e3926-131">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-131">DomainResponse (SOAP)</span></span>](domainresponse-soap.md)
    
- [<span data-ttu-id="e3926-132">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-132">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md)
    
- [<span data-ttu-id="e3926-133">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-133">DomainSettings (SOAP)</span></span>](domainsettings-soap.md)
    
- [<span data-ttu-id="e3926-134">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-134">DomainSetting (SOAP)</span></span>](domainsetting-soap.md)
    
- [<span data-ttu-id="e3926-135">名 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-135">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="e3926-136">値 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-136">Value (SOAP)</span></span>](value-soap.md)
    
- [<span data-ttu-id="e3926-137">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-137">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="e3926-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3926-138">See also</span></span>



[<span data-ttu-id="e3926-139">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="e3926-140">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3926-140">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

