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
description: GetPhoneCallInformation 操作は、指定した電話の呼び出しに関する情報を返します。
ms.openlocfilehash: 8f98ca5dd304eadffc307fa47620b7db6401c782
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760836"
---
# <a name="getphonecallinformation-operation"></a><span data-ttu-id="30087-103">GetPhoneCallInformation 操作</span><span class="sxs-lookup"><span data-stu-id="30087-103">GetPhoneCallInformation operation</span></span>

<span data-ttu-id="30087-104">**GetPhoneCallInformation**操作は、指定した電話の呼び出しに関する情報を返します。</span><span class="sxs-lookup"><span data-stu-id="30087-104">The **GetPhoneCallInformation** operation returns information about the specified telephone call.</span></span> 
  
## <a name="getphonecallinformation-request-example"></a><span data-ttu-id="30087-105">GetPhoneCallInformation 要求の例</span><span class="sxs-lookup"><span data-stu-id="30087-105">GetPhoneCallInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="30087-106">説明</span><span class="sxs-lookup"><span data-stu-id="30087-106">Description</span></span>

<span data-ttu-id="30087-107">**GetPhoneCallInformation**要求の次の例では、特定の電話の呼び出しに関する情報を取得する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="30087-107">The following example of a **GetPhoneCallInformation** request shows how to form a request to get information about a specific telephone call.</span></span> 
  
### <a name="code"></a><span data-ttu-id="30087-108">コード</span><span class="sxs-lookup"><span data-stu-id="30087-108">Code</span></span>

```xml
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
    <m:GetPhoneCallInformation>
      <m:PhoneCallId Id="NDDY5uY29y9t"/>
    </m:GetPhoneCallInformation>
  </soap:Body>
</soap:Envelope>
```

## <a name="getphonecallinformation-response-example"></a><span data-ttu-id="30087-109">GetPhoneCallInformation の応答の例</span><span class="sxs-lookup"><span data-stu-id="30087-109">GetPhoneCallInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="30087-110">説明</span><span class="sxs-lookup"><span data-stu-id="30087-110">Description</span></span>

<span data-ttu-id="30087-111">**GetPhoneCallInformation**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30087-111">The following example shows a successful response to the **GetPhoneCallInformation** request.</span></span> <span data-ttu-id="30087-112">応答は、現在接続されている電話の呼び出しを表します。</span><span class="sxs-lookup"><span data-stu-id="30087-112">The response represents a telephone call that is currently connected.</span></span> 
  
### <a name="code"></a><span data-ttu-id="30087-113">コード</span><span class="sxs-lookup"><span data-stu-id="30087-113">Code</span></span>

```xml
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
    <GetPhoneCallInformationResponse ResponseClass="Success" 
                                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:PhoneCallInformation xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:PhoneCallState xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">Connected</t:PhoneCallState>
        <t:ConnectionFailureCause xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">None</t:ConnectionFailureCause>
      </m:PhoneCallInformation>
    </GetPhoneCallInformationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="30087-114">関連項目</span><span class="sxs-lookup"><span data-stu-id="30087-114">See also</span></span>

- [<span data-ttu-id="30087-115">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="30087-115">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="30087-116">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="30087-116">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

