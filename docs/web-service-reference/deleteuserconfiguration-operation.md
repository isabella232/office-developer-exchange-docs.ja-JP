---
title: DeleteUserConfiguration 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 93e44690-be2d-4fdb-96a8-4ded3c193aed
description: DeleteUserConfiguration 操作は、フォルダーのユーザー構成オブジェクトを削除します。
ms.openlocfilehash: 064e1ace2c2f51783431ce42670b2a4fd8146b54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44451468"
---
# <a name="deleteuserconfiguration-operation"></a><span data-ttu-id="11a46-103">DeleteUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="11a46-103">DeleteUserConfiguration operation</span></span>

<span data-ttu-id="11a46-104">**Deleteuserconfiguration**操作は、フォルダーのユーザー構成オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="11a46-104">The **DeleteUserConfiguration** operation deletes a user configuration object on a folder.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="11a46-105">**Deleteuserconfiguration**操作は、イベント通知システムの移動イベントをトリガーします。</span><span class="sxs-lookup"><span data-stu-id="11a46-105">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="11a46-106">ユーザー構成オブジェクトは、収集に移動されます。</span><span class="sxs-lookup"><span data-stu-id="11a46-106">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="deleteuserconfiguration-request-example"></a><span data-ttu-id="11a46-107">DeleteUserConfiguration 要求の例</span><span class="sxs-lookup"><span data-stu-id="11a46-107">DeleteUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="11a46-108">説明</span><span class="sxs-lookup"><span data-stu-id="11a46-108">Description</span></span>

<span data-ttu-id="11a46-109">次の**Deleteuserconfiguration**要求の例は、下書きフォルダーのユーザー構成オブジェクトを削除するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="11a46-109">The following example of a **DeleteUserConfiguration** request shows how to form a request to delete a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="11a46-110">コード</span><span class="sxs-lookup"><span data-stu-id="11a46-110">Code</span></span>

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
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="deleteuserconfiguration-response-example"></a><span data-ttu-id="11a46-111">DeleteUserConfiguration の応答の例</span><span class="sxs-lookup"><span data-stu-id="11a46-111">DeleteUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="11a46-112">説明</span><span class="sxs-lookup"><span data-stu-id="11a46-112">Description</span></span>

<span data-ttu-id="11a46-113">次の例は、 **Deleteuserconfiguration**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="11a46-113">The following example shows a successful response to the **DeleteUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="11a46-114">コード</span><span class="sxs-lookup"><span data-stu-id="11a46-114">Code</span></span>

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
    <m:DeleteUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:DeleteUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="11a46-115">関連項目</span><span class="sxs-lookup"><span data-stu-id="11a46-115">See also</span></span>

- [<span data-ttu-id="11a46-116">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="11a46-116">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="11a46-117">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="11a46-117">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

