---
title: SetTelephoneAccessFolderEmail 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: SetTelephoneAccessFolderEmail 操作は、ユニファイドメッセージングが電話でユーザーにメッセージを読み取るためのフォルダーを設定します。
ms.openlocfilehash: a2bb630f812ca811b4cbe68db1308dc18e5d3ba0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467334"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="da6ca-103">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="da6ca-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="da6ca-104">SetTelephoneAccessFolderEmail 操作は、ユニファイドメッセージングが電話でユーザーにメッセージを読み取るためのフォルダーを設定します。</span><span class="sxs-lookup"><span data-stu-id="da6ca-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="da6ca-105">SetTelephoneAccessFolderEmail 要求の例</span><span class="sxs-lookup"><span data-stu-id="da6ca-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="da6ca-106">Description</span><span class="sxs-lookup"><span data-stu-id="da6ca-106">Description</span></span>

<span data-ttu-id="da6ca-107">次の SetTelephoneAccessFolderEmail 要求の例は、ユニファイドメッセージングが電話でユーザーに返信するフォルダーを設定する要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="da6ca-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="da6ca-108">コード</span><span class="sxs-lookup"><span data-stu-id="da6ca-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="da6ca-109">Successful SetTelephoneAccessFolderEmail response の例</span><span class="sxs-lookup"><span data-stu-id="da6ca-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="da6ca-110">Description</span><span class="sxs-lookup"><span data-stu-id="da6ca-110">Description</span></span>

<span data-ttu-id="da6ca-111">SetTelephoneAccessFolderEmail response の次の例は、SetTelephoneAccessFolderEmail 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="da6ca-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="da6ca-112">コード</span><span class="sxs-lookup"><span data-stu-id="da6ca-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="da6ca-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="da6ca-113">See also</span></span>



[<span data-ttu-id="da6ca-114">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="da6ca-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="da6ca-115">SetTelephoneAccessFolderEmailResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="da6ca-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="da6ca-116">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="da6ca-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

