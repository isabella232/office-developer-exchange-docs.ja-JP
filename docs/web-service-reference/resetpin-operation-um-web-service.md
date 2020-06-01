---
title: ResetPIN 操作 (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: ResetPIN 操作は、PIN (TUI パスワード) を新しいランダムな値に変更します。
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465493"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="5f50e-103">ResetPIN 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5f50e-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="5f50e-104">ResetPIN 操作は、PIN (TUI パスワード) を新しいランダムな値に変更します。</span><span class="sxs-lookup"><span data-stu-id="5f50e-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f50e-105">注釈</span><span class="sxs-lookup"><span data-stu-id="5f50e-105">Remarks</span></span>

<span data-ttu-id="5f50e-106">ResetPIN 操作は、PIN ポリシーに基づいて新しい PIN を作成します。</span><span class="sxs-lookup"><span data-stu-id="5f50e-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="5f50e-107">操作が成功した場合は、新しい PIN を含む電子メールメッセージがユーザーのメールボックスに送信されます。</span><span class="sxs-lookup"><span data-stu-id="5f50e-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="5f50e-108">操作が失敗した場合は、エラーに関する情報を含む例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="5f50e-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="5f50e-109">ResetPIN 要求の例</span><span class="sxs-lookup"><span data-stu-id="5f50e-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="5f50e-110">説明</span><span class="sxs-lookup"><span data-stu-id="5f50e-110">Description</span></span>

<span data-ttu-id="5f50e-111">次の ResetPIN 要求の例は、メールボックスの PIN をリセットする要求を形成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5f50e-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="5f50e-112">コード</span><span class="sxs-lookup"><span data-stu-id="5f50e-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="5f50e-113">正常な ResetPIN 応答の例</span><span class="sxs-lookup"><span data-stu-id="5f50e-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="5f50e-114">説明</span><span class="sxs-lookup"><span data-stu-id="5f50e-114">Description</span></span>

<span data-ttu-id="5f50e-115">次の ResetPIN 応答の例は、ResetPIN 要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="5f50e-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5f50e-116">コード</span><span class="sxs-lookup"><span data-stu-id="5f50e-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5f50e-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="5f50e-117">See also</span></span>



[<span data-ttu-id="5f50e-118">ResetPIN (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5f50e-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="5f50e-119">ResetPINResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="5f50e-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

