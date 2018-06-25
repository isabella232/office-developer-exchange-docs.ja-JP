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
description: SetTelephoneAccessFolderEmail 操作では、ユニファイド メッセージングはの読み取り元メッセージのユーザーに電話でフォルダーを設定します。
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="d7dce-103">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d7dce-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="d7dce-104">SetTelephoneAccessFolderEmail 操作では、ユニファイド メッセージングはの読み取り元メッセージのユーザーに電話でフォルダーを設定します。</span><span class="sxs-lookup"><span data-stu-id="d7dce-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="d7dce-105">SetTelephoneAccessFolderEmail 要求の例</span><span class="sxs-lookup"><span data-stu-id="d7dce-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="d7dce-106">説明</span><span class="sxs-lookup"><span data-stu-id="d7dce-106">Description</span></span>

<span data-ttu-id="d7dce-107">SetTelephoneAccessFolderEmail 要求の次の例では、ユニファイド メッセージングはの読み取り元のユーザーに電話でフォルダーを設定する要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d7dce-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="d7dce-108">コード</span><span class="sxs-lookup"><span data-stu-id="d7dce-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="d7dce-109">成功した SetTelephoneAccessFolderEmail の応答の例</span><span class="sxs-lookup"><span data-stu-id="d7dce-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="d7dce-110">説明</span><span class="sxs-lookup"><span data-stu-id="d7dce-110">Description</span></span>

<span data-ttu-id="d7dce-111">SetTelephoneAccessFolderEmail 要求への応答を SetTelephoneAccessFolderEmail の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7dce-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d7dce-112">コード</span><span class="sxs-lookup"><span data-stu-id="d7dce-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="d7dce-113">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7dce-113">See also</span></span>



[<span data-ttu-id="d7dce-114">SetTelephoneAccessFolderEmail (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d7dce-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="d7dce-115">SetTelephoneAccessFolderEmailResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d7dce-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="d7dce-116">base64FolderId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="d7dce-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

