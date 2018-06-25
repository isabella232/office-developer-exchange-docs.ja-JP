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
description: ResetPIN 操作では、暗証番号 (pin) (TUI パスワード) を新しいランダムな値に変更します。
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833146"
---
# <a name="resetpin-operation-um-web-service"></a><span data-ttu-id="6809c-103">ResetPIN 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6809c-103">ResetPIN operation (UM web service)</span></span>

<span data-ttu-id="6809c-104">ResetPIN 操作では、暗証番号 (pin) (TUI パスワード) を新しいランダムな値に変更します。</span><span class="sxs-lookup"><span data-stu-id="6809c-104">The ResetPIN operation changes the PIN (TUI password) to a new random value.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6809c-105">備考</span><span class="sxs-lookup"><span data-stu-id="6809c-105">Remarks</span></span>

<span data-ttu-id="6809c-106">ResetPIN 操作では、暗証番号 (pin) のポリシーに基づき、新しい PIN を作成します。</span><span class="sxs-lookup"><span data-stu-id="6809c-106">The ResetPIN operation creates a new PIN based on the PIN policies.</span></span> <span data-ttu-id="6809c-107">操作が成功した場合、新しい暗証番号 (pin) を含む電子メール メッセージがユーザーのメールボックスに送信されます。</span><span class="sxs-lookup"><span data-stu-id="6809c-107">If the operation is successful, an e-mail message that contains the new PIN is sent to the mailbox of the user.</span></span> <span data-ttu-id="6809c-108">操作が失敗した場合、エラーに関する情報が含まれている例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="6809c-108">If the operation fails, it will throw an exception that contains information about the failure.</span></span>
  
## <a name="resetpin-request-example"></a><span data-ttu-id="6809c-109">ResetPIN 要求の例</span><span class="sxs-lookup"><span data-stu-id="6809c-109">ResetPIN request example</span></span>

### <a name="description"></a><span data-ttu-id="6809c-110">説明</span><span class="sxs-lookup"><span data-stu-id="6809c-110">Description</span></span>

<span data-ttu-id="6809c-111">ResetPIN 要求の次の例では、メールボックスの PIN をリセットする要求を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="6809c-111">The following example of a ResetPIN request shows how to form a request to reset the PIN for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="6809c-112">コード</span><span class="sxs-lookup"><span data-stu-id="6809c-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a><span data-ttu-id="6809c-113">ResetPIN 応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="6809c-113">Successful ResetPIN response example</span></span>

### <a name="description"></a><span data-ttu-id="6809c-114">説明</span><span class="sxs-lookup"><span data-stu-id="6809c-114">Description</span></span>

<span data-ttu-id="6809c-115">ResetPIN 要求への応答を ResetPIN 応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6809c-115">The following example of a ResetPIN response shows a response to the ResetPIN request.</span></span>
  
### <a name="code"></a><span data-ttu-id="6809c-116">コード</span><span class="sxs-lookup"><span data-stu-id="6809c-116">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6809c-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="6809c-117">See also</span></span>



[<span data-ttu-id="6809c-118">ResetPIN (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6809c-118">ResetPIN (UM web service)</span></span>](resetpin-um-web-service.md)
  
[<span data-ttu-id="6809c-119">ResetPINResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="6809c-119">ResetPINResponse (UM web service)</span></span>](resetpinresponse-um-web-service.md)

