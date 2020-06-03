---
title: GetUserConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 71d50e3c-92bd-435f-8118-b28bb85f8138
description: GetUserConfiguration 操作は、フォルダーからユーザー構成オブジェクトを取得します。
ms.openlocfilehash: fb28e88d1a47b0ea8f63ed33b1efacae8538e1c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458209"
---
# <a name="getuserconfiguration-operation"></a><span data-ttu-id="34c2c-103">GetUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="34c2c-103">GetUserConfiguration operation</span></span>

<span data-ttu-id="34c2c-104">**Getuserconfiguration**操作は、フォルダーからユーザー構成オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="34c2c-104">The **GetUserConfiguration** operation gets a user configuration object from a folder.</span></span> 
  
## <a name="getuserconfiguration-request-example"></a><span data-ttu-id="34c2c-105">GetUserConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="34c2c-105">GetUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="34c2c-106">Description</span><span class="sxs-lookup"><span data-stu-id="34c2c-106">Description</span></span>

<span data-ttu-id="34c2c-107">次の**Getuserconfiguration**要求の例は、下書きフォルダーでユーザー構成オブジェクトを取得する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="34c2c-107">The following example of a **GetUserConfiguration** request shows how to form a request to get a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="34c2c-108">コード</span><span class="sxs-lookup"><span data-stu-id="34c2c-108">Code</span></span>

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
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>Dictionary</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getuserconfiguration-response-example"></a><span data-ttu-id="34c2c-109">GetUserConfiguration 応答の例</span><span class="sxs-lookup"><span data-stu-id="34c2c-109">GetUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="34c2c-110">Description</span><span class="sxs-lookup"><span data-stu-id="34c2c-110">Description</span></span>

<span data-ttu-id="34c2c-111">次の例は、 **Getuserconfiguration**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="34c2c-111">The following example shows a successful response to the **GetUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="34c2c-112">コード</span><span class="sxs-lookup"><span data-stu-id="34c2c-112">Code</span></span>

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
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts">
              </t:DistinguishedFolderId>
            </t:UserConfigurationName>
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="34c2c-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="34c2c-113">See also</span></span>



[<span data-ttu-id="34c2c-114">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="34c2c-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="34c2c-115">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="34c2c-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

