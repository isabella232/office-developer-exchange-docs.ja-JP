---
title: GetPasswordExpirationDate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: GetPasswordExpirationDate 操作は、現在のユーザーの電子メールアカウントパスワードの有効期限日を提供します。
ms.openlocfilehash: 4184092cf98161e4c2f74446cef5439722ae71a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457894"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="81c76-103">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="81c76-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="81c76-104">**GetPasswordExpirationDate**操作は、現在のユーザーの電子メールアカウントパスワードの有効期限日を提供します。</span><span class="sxs-lookup"><span data-stu-id="81c76-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="81c76-105">この操作は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="81c76-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="81c76-106">GetPasswordExpirationDate 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81c76-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="81c76-107">**GetPasswordExpirationDate**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="81c76-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="81c76-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="81c76-108">**Header**</span></span>|<span data-ttu-id="81c76-109">**要素**</span><span class="sxs-lookup"><span data-stu-id="81c76-109">**Element**</span></span>|<span data-ttu-id="81c76-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="81c76-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="81c76-111">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="81c76-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="81c76-112">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="81c76-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="81c76-113">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="81c76-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="81c76-114">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="81c76-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="81c76-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="81c76-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="81c76-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="81c76-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="81c76-117">操作要求のスキーマを識別します。</span><span class="sxs-lookup"><span data-stu-id="81c76-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="81c76-118">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="81c76-118">This is applicable to a request.</span></span> <span data-ttu-id="81c76-119">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="81c76-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="81c76-120">GetPasswordExpirationDate 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="81c76-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="81c76-121">Description</span><span class="sxs-lookup"><span data-stu-id="81c76-121">Description</span></span>

<span data-ttu-id="81c76-122">次の**GetPasswordExpirationDate**操作要求の例は、電子メールアカウントのパスワードの有効期限を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="81c76-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="81c76-123">コード</span><span class="sxs-lookup"><span data-stu-id="81c76-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="81c76-124">Request 要素</span><span class="sxs-lookup"><span data-stu-id="81c76-124">Request elements</span></span>

<span data-ttu-id="81c76-125">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="81c76-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="81c76-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="81c76-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="81c76-127">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="81c76-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="81c76-128">成功した GetPasswordExpirationDate 操作の応答</span><span class="sxs-lookup"><span data-stu-id="81c76-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="81c76-129">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="81c76-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="81c76-130">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="81c76-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="81c76-131">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="81c76-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

