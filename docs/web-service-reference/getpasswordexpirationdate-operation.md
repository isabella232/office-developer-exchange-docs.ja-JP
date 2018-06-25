---
title: GetPasswordExpirationDate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: GetPasswordExpirationDate 操作では、現在のユーザーの電子メール アカウントのパスワード有効期限の日付を提供します。
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760816"
---
# <a name="getpasswordexpirationdate-operation"></a><span data-ttu-id="70a9e-103">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="70a9e-103">GetPasswordExpirationDate operation</span></span>

<span data-ttu-id="70a9e-104">**GetPasswordExpirationDate**操作では、現在のユーザーの電子メール アカウントのパスワード有効期限の日付を提供します。</span><span class="sxs-lookup"><span data-stu-id="70a9e-104">The **GetPasswordExpirationDate** operation provides the email account password expiration date for the current user.</span></span> 
  
<span data-ttu-id="70a9e-105">この操作は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="70a9e-105">This operation was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a><span data-ttu-id="70a9e-106">GetPasswordExpirationDate 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70a9e-106">GetPasswordExpirationDate operation SOAP headers</span></span>

<span data-ttu-id="70a9e-107">**GetPasswordExpirationDate**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-107">The **GetPasswordExpirationDate** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="70a9e-108">**Header**</span><span class="sxs-lookup"><span data-stu-id="70a9e-108">**Header**</span></span>|<span data-ttu-id="70a9e-109">**要素**</span><span class="sxs-lookup"><span data-stu-id="70a9e-109">**Element**</span></span>|<span data-ttu-id="70a9e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="70a9e-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70a9e-111">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="70a9e-111">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="70a9e-112">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="70a9e-112">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="70a9e-113">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="70a9e-113">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="70a9e-114">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-114">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="70a9e-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="70a9e-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="70a9e-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="70a9e-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="70a9e-117">操作要求のスキーマを識別します。</span><span class="sxs-lookup"><span data-stu-id="70a9e-117">Identifies the schema for the operation request.</span></span> <span data-ttu-id="70a9e-118">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-118">This is applicable to a request.</span></span> <span data-ttu-id="70a9e-119">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-119">This is applicable to a request.</span></span>  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a><span data-ttu-id="70a9e-120">GetPasswordExpirationDate 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="70a9e-120">GetPasswordExpirationDate operation request example</span></span>

### <a name="description"></a><span data-ttu-id="70a9e-121">説明</span><span class="sxs-lookup"><span data-stu-id="70a9e-121">Description</span></span>

<span data-ttu-id="70a9e-122">**GetPasswordExpirationDate**操作要求の次の例では、電子メール アカウントのパスワードの有効期限の日付を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="70a9e-122">The following example of a **GetPasswordExpirationDate** operation request shows how to get the password expiration date for an email account.</span></span> 
  
### <a name="code"></a><span data-ttu-id="70a9e-123">コード</span><span class="sxs-lookup"><span data-stu-id="70a9e-123">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="70a9e-124">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="70a9e-124">Request elements</span></span>

<span data-ttu-id="70a9e-125">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="70a9e-126">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="70a9e-126">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md)
    
- [<span data-ttu-id="70a9e-127">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="70a9e-127">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a><span data-ttu-id="70a9e-128">GetPasswordExpirationDate 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="70a9e-128">Successful GetPasswordExpirationDate operation response</span></span>

<span data-ttu-id="70a9e-129">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="70a9e-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="70a9e-130">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="70a9e-130">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
    
- [<span data-ttu-id="70a9e-131">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="70a9e-131">PasswordExpirationDate</span></span>](passwordexpirationdate.md)
    

