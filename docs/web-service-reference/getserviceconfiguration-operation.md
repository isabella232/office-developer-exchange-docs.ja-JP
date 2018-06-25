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
description: GetServiceConfiguration 操作は、指定した型のサービスの構成情報を取得します。 この操作は、ユニファイド メッセージング、保護ルール、およびヒントのメール サービスの構成設定を返すことができます。
ms.openlocfilehash: 7fdc4d8defac3d6d352c121483bf8a4c735d9629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831667"
---
# <a name="getserviceconfiguration-operation"></a><span data-ttu-id="9c977-104">GetServiceConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="9c977-104">GetServiceConfiguration operation</span></span>

<span data-ttu-id="9c977-105">**GetServiceConfiguration**操作は、指定した型のサービスの構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="9c977-105">The **GetServiceConfiguration** operation gets configuration information for the specified type of service.</span></span> <span data-ttu-id="9c977-106">この操作は、ユニファイド メッセージング、保護ルール、およびヒントのメール サービスの構成設定を返すことができます。</span><span class="sxs-lookup"><span data-stu-id="9c977-106">This operation can return configuration settings for the Unified Messaging, Protection Rules, and Mail Tips services.</span></span> 
  
## <a name="getserviceconfiguration-request-example"></a><span data-ttu-id="9c977-107">GetServiceConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="9c977-107">GetServiceConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="9c977-108">説明</span><span class="sxs-lookup"><span data-stu-id="9c977-108">Description</span></span>

<span data-ttu-id="9c977-109">**GetServiceConfiguration**要求の次の例では、ユニファイド メッセージング サービスの構成情報を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="9c977-109">The following example of a **GetServiceConfiguration** request shows how to form a request to get configuration information for the Unified Messaging service.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9c977-110">コード</span><span class="sxs-lookup"><span data-stu-id="9c977-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

## <a name="getserviceconfiguration-response-example"></a><span data-ttu-id="9c977-111">GetServiceConfiguration の応答の例</span><span class="sxs-lookup"><span data-stu-id="9c977-111">GetServiceConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="9c977-112">説明</span><span class="sxs-lookup"><span data-stu-id="9c977-112">Description</span></span>

<span data-ttu-id="9c977-113">**GetServiceConfiguration**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9c977-113">The following example shows a successful response to the **GetServiceConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9c977-114">コード</span><span class="sxs-lookup"><span data-stu-id="9c977-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetServiceConfigurationResponse ResponseClass="Success" 
                                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <ResponseMessages>
        <ServiceConfigurationResponseMessageType ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <m:UnifiedMessagingConfiguration xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
            <t:UmEnabled xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">true</t:UmEnabled>
            <t:PlayOnPhoneDialString xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">user@contoso.com</t:PlayOnPhoneDialString>
            <t:PlayOnPhoneEnabled xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">true</t:PlayOnPhoneEnabled>
          </m:UnifiedMessagingConfiguration>
        </ServiceConfigurationResponseMessageType>
      </ResponseMessages>
    </GetServiceConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="getserviceconfiguration-error-response-example"></a><span data-ttu-id="9c977-115">GetServiceConfiguration エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="9c977-115">GetServiceConfiguration Error response example</span></span>

### <a name="description"></a><span data-ttu-id="9c977-116">説明</span><span class="sxs-lookup"><span data-stu-id="9c977-116">Description</span></span>

<span data-ttu-id="9c977-117">**GetServiceConfiguration**要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9c977-117">The following example shows an error response to the **GetServiceConfiguration** request.</span></span> <span data-ttu-id="9c977-118">構成が正しくない名前で、このエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="9c977-118">This error was caused by an incorrect configuration name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9c977-119">コード</span><span class="sxs-lookup"><span data-stu-id="9c977-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: 
      The 'http://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
      is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
      datatype 'http://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType' 
      - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>13</t:LineNumber>
          <t:LinePosition>62</t:LinePosition>
          <t:Violation>The 'http://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
          is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
          datatype 'http://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType'
          - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="9c977-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c977-120">See also</span></span>



[<span data-ttu-id="9c977-121">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="9c977-121">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="9c977-122">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9c977-122">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

