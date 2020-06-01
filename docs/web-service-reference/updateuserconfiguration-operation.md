---
title: UpdateUserConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfiguration
api_type:
- schema
ms.assetid: eda73b62-6a3a-43ae-8fd9-f30892811f27
description: UpdateUserConfiguration 操作は、フォルダーのユーザー構成オブジェクトを更新します。
ms.openlocfilehash: 95fe6518fa30104463ec7f0aec8f786183eb513b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468545"
---
# <a name="updateuserconfiguration-operation"></a><span data-ttu-id="cfa45-103">UpdateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="cfa45-103">UpdateUserConfiguration operation</span></span>

<span data-ttu-id="cfa45-104">**Updateuserconfiguration**操作は、フォルダーのユーザー構成オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfa45-104">The **UpdateUserConfiguration** operation updates a user configuration object on a folder.</span></span> 
  
## <a name="updateuserconfiguration-request-example"></a><span data-ttu-id="cfa45-105">UpdateUserConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="cfa45-105">UpdateUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="cfa45-106">説明</span><span class="sxs-lookup"><span data-stu-id="cfa45-106">Description</span></span>

<span data-ttu-id="cfa45-107">次の**Updateuserconfiguration**要求の例は、下書きフォルダーのユーザー構成オブジェクトを更新する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cfa45-107">The following example of an **UpdateUserConfiguration** request shows how to form a request to update a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cfa45-108">コード</span><span class="sxs-lookup"><span data-stu-id="cfa45-108">Code</span></span>

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
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts"/>
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>111-111-5555</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="updateuserconfiguration-response-example"></a><span data-ttu-id="cfa45-109">UpdateUserConfiguration 応答の例</span><span class="sxs-lookup"><span data-stu-id="cfa45-109">UpdateUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="cfa45-110">説明</span><span class="sxs-lookup"><span data-stu-id="cfa45-110">Description</span></span>

<span data-ttu-id="cfa45-111">次の例は、 **Updateuserconfiguration**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cfa45-111">The following example shows a successful response to the **UpdateUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cfa45-112">コード</span><span class="sxs-lookup"><span data-stu-id="cfa45-112">Code</span></span>

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
    <m:UpdateUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UpdateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:UpdateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="cfa45-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="cfa45-113">See also</span></span>



[<span data-ttu-id="cfa45-114">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="cfa45-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="cfa45-115">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cfa45-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

