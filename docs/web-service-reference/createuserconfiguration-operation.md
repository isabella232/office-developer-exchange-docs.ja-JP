---
title: CreateUserConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: eb5b8ab6-9743-481c-aac9-f9aa889bd353
description: CreateUserConfiguration 操作は、ユーザー構成オブジェクトをフォルダーに作成します。
ms.openlocfilehash: 0c9233146d21c7014be15896426b968106485200
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463784"
---
# <a name="createuserconfiguration-operation"></a><span data-ttu-id="0ae66-103">CreateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="0ae66-103">CreateUserConfiguration operation</span></span>

<span data-ttu-id="0ae66-104">**CreateUserConfiguration**操作は、ユーザー構成オブジェクトをフォルダーに作成します。</span><span class="sxs-lookup"><span data-stu-id="0ae66-104">The **CreateUserConfiguration** operation creates a user configuration object on a folder.</span></span> 
  
## <a name="createuserconfiguration-request-example"></a><span data-ttu-id="0ae66-105">CreateUserConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="0ae66-105">CreateUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="0ae66-106">Description</span><span class="sxs-lookup"><span data-stu-id="0ae66-106">Description</span></span>

<span data-ttu-id="0ae66-107">次の**CreateUserConfiguration**要求の例は、下書きフォルダーでユーザー構成オブジェクトを作成するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0ae66-107">The following example of a **CreateUserConfiguration** request shows how to form a request to create a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0ae66-108">コード</span><span class="sxs-lookup"><span data-stu-id="0ae66-108">Code</span></span>

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
    <m:CreateUserConfiguration>
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
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="createuserconfiguration-response-example"></a><span data-ttu-id="0ae66-109">CreateUserConfiguration response の例</span><span class="sxs-lookup"><span data-stu-id="0ae66-109">CreateUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="0ae66-110">Description</span><span class="sxs-lookup"><span data-stu-id="0ae66-110">Description</span></span>

<span data-ttu-id="0ae66-111">次の例は、 **CreateUserConfiguration**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0ae66-111">The following example shows a successful response to the **CreateUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0ae66-112">コード</span><span class="sxs-lookup"><span data-stu-id="0ae66-112">Code</span></span>

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
    <m:CreateUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:CreateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:CreateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="0ae66-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ae66-113">See also</span></span>



[<span data-ttu-id="0ae66-114">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="0ae66-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="0ae66-115">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0ae66-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

