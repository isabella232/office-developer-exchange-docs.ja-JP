---
title: GetUMProperties 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: GetUMProperties 操作は、要求を行っているユーザーのメールボックスのすべてのユニファイドメッセージングプロパティを取得します。
ms.openlocfilehash: 42176d9cd0288af6515aeea616a4f216a419410c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462473"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="60786-103">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="60786-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="60786-104">GetUMProperties 操作は、要求を行っているユーザーのメールボックスのすべてのユニファイドメッセージングプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="60786-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="60786-105">GetUMProperties 要求の例</span><span class="sxs-lookup"><span data-stu-id="60786-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="60786-106">説明</span><span class="sxs-lookup"><span data-stu-id="60786-106">Description</span></span>

<span data-ttu-id="60786-107">次の GetUMProperties 要求の例は、メールボックスのユニファイドメッセージングのプロパティを取得するための要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="60786-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="60786-108">コード</span><span class="sxs-lookup"><span data-stu-id="60786-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="60786-109">成功した GetUMProperties 応答の例</span><span class="sxs-lookup"><span data-stu-id="60786-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="60786-110">説明</span><span class="sxs-lookup"><span data-stu-id="60786-110">Description</span></span>

<span data-ttu-id="60786-111">GetUMProperties 応答の次の例は、GetUMProperties 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="60786-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="60786-112">コード</span><span class="sxs-lookup"><span data-stu-id="60786-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="60786-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="60786-113">See also</span></span>



[<span data-ttu-id="60786-114">GetUMProperties (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="60786-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="60786-115">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="60786-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

