---
title: GetServiceConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: 070cbfe5-325a-4955-8e4a-8230ea0459a7
description: GetServiceConfiguration 操作は、指定されたサービスの種類の構成情報を取得します。 この操作は、ユニファイドメッセージング、保護ルール、およびメールヒントサービスの構成設定を返すことができます。
ms.openlocfilehash: b8ea2cef366a52765850dddcc8c1ef1e8fa68b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460912"
---
# <a name="getserviceconfiguration-operation"></a><span data-ttu-id="f925f-104">GetServiceConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="f925f-104">GetServiceConfiguration operation</span></span>

<span data-ttu-id="f925f-105">**GetServiceConfiguration**操作は、指定されたサービスの種類の構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="f925f-105">The **GetServiceConfiguration** operation gets configuration information for the specified type of service.</span></span> <span data-ttu-id="f925f-106">この操作は、ユニファイドメッセージング、保護ルール、およびメールヒントサービスの構成設定を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="f925f-106">This operation can return configuration settings for the Unified Messaging, Protection Rules, and Mail Tips services.</span></span> 
  
## <a name="getserviceconfiguration-request-example"></a><span data-ttu-id="f925f-107">GetServiceConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="f925f-107">GetServiceConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="f925f-108">Description</span><span class="sxs-lookup"><span data-stu-id="f925f-108">Description</span></span>

<span data-ttu-id="f925f-109">次の**GetServiceConfiguration**要求の例は、ユニファイドメッセージングサービスの構成情報を取得するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f925f-109">The following example of a **GetServiceConfiguration** request shows how to form a request to get configuration information for the Unified Messaging service.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f925f-110">コード</span><span class="sxs-lookup"><span data-stu-id="f925f-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetServiceConfiguration>
      <m:RequestedConfiguration>
        <m:ConfigurationName>UnifiedMessagingConfiguration</m:ConfigurationName>
      </m:RequestedConfiguration>
    </m:GetServiceConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getserviceconfiguration-response-example"></a><span data-ttu-id="f925f-111">GetServiceConfiguration response の例</span><span class="sxs-lookup"><span data-stu-id="f925f-111">GetServiceConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="f925f-112">Description</span><span class="sxs-lookup"><span data-stu-id="f925f-112">Description</span></span>

<span data-ttu-id="f925f-113">次の例は、 **GetServiceConfiguration**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f925f-113">The following example shows a successful response to the **GetServiceConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f925f-114">コード</span><span class="sxs-lookup"><span data-stu-id="f925f-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetServiceConfigurationResponse ResponseClass="Success" 
                                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <ResponseMessages>
        <ServiceConfigurationResponseMessageType ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <m:UnifiedMessagingConfiguration xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
            <t:UmEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:UmEnabled>
            <t:PlayOnPhoneDialString xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">user@contoso.com</t:PlayOnPhoneDialString>
            <t:PlayOnPhoneEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:PlayOnPhoneEnabled>
          </m:UnifiedMessagingConfiguration>
        </ServiceConfigurationResponseMessageType>
      </ResponseMessages>
    </GetServiceConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="getserviceconfiguration-error-response-example"></a><span data-ttu-id="f925f-115">GetServiceConfiguration エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="f925f-115">GetServiceConfiguration Error response example</span></span>

### <a name="description"></a><span data-ttu-id="f925f-116">Description</span><span class="sxs-lookup"><span data-stu-id="f925f-116">Description</span></span>

<span data-ttu-id="f925f-117">次の例は、 **GetServiceConfiguration**要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f925f-117">The following example shows an error response to the **GetServiceConfiguration** request.</span></span> <span data-ttu-id="f925f-118">このエラーは、構成名が正しくないことが原因で発生しました。</span><span class="sxs-lookup"><span data-stu-id="f925f-118">This error was caused by an incorrect configuration name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f925f-119">コード</span><span class="sxs-lookup"><span data-stu-id="f925f-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: 
      The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
      is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
      datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType' 
      - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>13</t:LineNumber>
          <t:LinePosition>62</t:LinePosition>
          <t:Violation>The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
          is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
          datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType'
          - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f925f-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="f925f-120">See also</span></span>



[<span data-ttu-id="f925f-121">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="f925f-121">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="f925f-122">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f925f-122">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

