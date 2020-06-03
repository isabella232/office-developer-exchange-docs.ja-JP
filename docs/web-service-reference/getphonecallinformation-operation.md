---
title: GetPhoneCallInformation 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 418bd6ca-39d9-49a9-841e-7a71ede1fa51
description: GetPhoneCallInformation 操作は、指定された通話に関する情報を返します。
ms.openlocfilehash: 231b160713526f44433188e2b1e3bd98012370b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458314"
---
# <a name="getphonecallinformation-operation"></a><span data-ttu-id="fc3d2-103">GetPhoneCallInformation 操作</span><span class="sxs-lookup"><span data-stu-id="fc3d2-103">GetPhoneCallInformation operation</span></span>

<span data-ttu-id="fc3d2-104">**GetPhoneCallInformation**操作は、指定された通話に関する情報を返します。</span><span class="sxs-lookup"><span data-stu-id="fc3d2-104">The **GetPhoneCallInformation** operation returns information about the specified telephone call.</span></span> 
  
## <a name="getphonecallinformation-request-example"></a><span data-ttu-id="fc3d2-105">GetPhoneCallInformation 要求の例</span><span class="sxs-lookup"><span data-stu-id="fc3d2-105">GetPhoneCallInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="fc3d2-106">Description</span><span class="sxs-lookup"><span data-stu-id="fc3d2-106">Description</span></span>

<span data-ttu-id="fc3d2-107">次の**GetPhoneCallInformation**要求の例は、特定の電話呼び出しに関する情報を取得するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fc3d2-107">The following example of a **GetPhoneCallInformation** request shows how to form a request to get information about a specific telephone call.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fc3d2-108">コード</span><span class="sxs-lookup"><span data-stu-id="fc3d2-108">Code</span></span>

```xml
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
    <m:GetPhoneCallInformation>
      <m:PhoneCallId Id="NDDY5uY29y9t"/>
    </m:GetPhoneCallInformation>
  </soap:Body>
</soap:Envelope>
```

## <a name="getphonecallinformation-response-example"></a><span data-ttu-id="fc3d2-109">GetPhoneCallInformation response の例</span><span class="sxs-lookup"><span data-stu-id="fc3d2-109">GetPhoneCallInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="fc3d2-110">Description</span><span class="sxs-lookup"><span data-stu-id="fc3d2-110">Description</span></span>

<span data-ttu-id="fc3d2-111">次の例は、 **GetPhoneCallInformation**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fc3d2-111">The following example shows a successful response to the **GetPhoneCallInformation** request.</span></span> <span data-ttu-id="fc3d2-112">応答は、現在接続されている通話を表します。</span><span class="sxs-lookup"><span data-stu-id="fc3d2-112">The response represents a telephone call that is currently connected.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fc3d2-113">コード</span><span class="sxs-lookup"><span data-stu-id="fc3d2-113">Code</span></span>

```xml
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
    <GetPhoneCallInformationResponse ResponseClass="Success" 
                                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:PhoneCallInformation xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:PhoneCallState xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Connected</t:PhoneCallState>
        <t:ConnectionFailureCause xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">None</t:ConnectionFailureCause>
      </m:PhoneCallInformation>
    </GetPhoneCallInformationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="fc3d2-114">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc3d2-114">See also</span></span>

- [<span data-ttu-id="fc3d2-115">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="fc3d2-115">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="fc3d2-116">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fc3d2-116">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

