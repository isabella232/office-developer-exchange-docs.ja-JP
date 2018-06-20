---
title: RemoveDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: 1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a
description: RemoveDelegate 操作は、ユーザーのメールボックスから、1 つまたは複数のデリゲートを削除します。
ms.openlocfilehash: 6f3371d19bd8a7fd967d4959d85037ae6b51f6aa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833088"
---
# <a name="removedelegate-operation"></a><span data-ttu-id="ff9e8-103">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="ff9e8-103">RemoveDelegate operation</span></span>

<span data-ttu-id="ff9e8-104">**RemoveDelegate**操作は、ユーザーのメールボックスから、1 つまたは複数のデリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-104">The **RemoveDelegate** operation removes one or more delegates from a user's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="ff9e8-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff9e8-105">SOAP Headers</span></span>

<span data-ttu-id="ff9e8-106">**RemoveDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-106">The **RemoveDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ff9e8-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="ff9e8-107">**Header**</span></span>|<span data-ttu-id="ff9e8-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff9e8-108">**Element**</span></span>|<span data-ttu-id="ff9e8-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff9e8-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ff9e8-110">偽装</span><span class="sxs-lookup"><span data-stu-id="ff9e8-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="ff9e8-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ff9e8-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ff9e8-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ff9e8-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ff9e8-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="ff9e8-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ff9e8-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ff9e8-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ff9e8-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ff9e8-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ff9e8-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ff9e8-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ff9e8-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ff9e8-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ff9e8-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ff9e8-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ff9e8-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ff9e8-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="removedelegate-request-example"></a><span data-ttu-id="ff9e8-122">RemoveDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="ff9e8-122">RemoveDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="ff9e8-123">説明</span><span class="sxs-lookup"><span data-stu-id="ff9e8-123">Description</span></span>

<span data-ttu-id="ff9e8-124">次のコード例は、user1 のメールボックスからの 2 つのデリゲートを削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-124">The following code example shows how to remove two delegates from user1's mailbox.</span></span> <span data-ttu-id="ff9e8-125">この例では、代理人のプライマリ SMTP アドレスを使用して 1 つのデリゲートが削除され、代理人のセキュリティ識別子 (SID) を使用して、もう 1 つが削除されます。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-125">In this example, one delegate is removed by using the delegate's primary SMTP address, and the other one is removed by using the delegate's security identifier (SID).</span></span>
  
### <a name="code"></a><span data-ttu-id="ff9e8-126">コード</span><span class="sxs-lookup"><span data-stu-id="ff9e8-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
        </t:UserId>
      </UserIds>
    </RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ff9e8-127">コメント</span><span class="sxs-lookup"><span data-stu-id="ff9e8-127">Comments</span></span>

<span data-ttu-id="ff9e8-128">**RemoveDelegate**操作では、指定した代理ユーザーのメールボックスを持つまたは Active Directory ディレクトリ サービスに存在するは必要はありません。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-128">The **RemoveDelegate** operation does not require the specified delegate user to have a mailbox or to exist in the Active Directory directory service.</span></span> <span data-ttu-id="ff9e8-129">代理エントリが孤立した場合は、 **RemoveDelegate**操作が成功します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-129">The **RemoveDelegate** operation will succeed if the delegate entry is orphaned.</span></span> 
  
## <a name="removedelegate-response-example"></a><span data-ttu-id="ff9e8-130">RemoveDelegate の応答の例</span><span class="sxs-lookup"><span data-stu-id="ff9e8-130">RemoveDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="ff9e8-131">説明</span><span class="sxs-lookup"><span data-stu-id="ff9e8-131">Description</span></span>

<span data-ttu-id="ff9e8-132">**RemoveDelegate**要求に正常な応答を**RemoveDelegate**の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-132">The following example of a **RemoveDelegate** response shows a successful response to a **RemoveDelegate** request.</span></span> <span data-ttu-id="ff9e8-133">応答には、各メールボックスから削除されるデリゲートの**DelegateUserResponseMessageType**要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-133">The response contains a **DelegateUserResponseMessageType** element for each delegate that is removed from the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ff9e8-134">コード</span><span class="sxs-lookup"><span data-stu-id="ff9e8-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="removedelegate-error-response-example"></a><span data-ttu-id="ff9e8-135">RemoveDelegate エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="ff9e8-135">RemoveDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ff9e8-136">説明</span><span class="sxs-lookup"><span data-stu-id="ff9e8-136">Description</span></span>

<span data-ttu-id="ff9e8-137">**RemoveDelegate**エラー応答の次の使用例は、存在しないデリゲートを削除する要求の結果を示しています。</span><span class="sxs-lookup"><span data-stu-id="ff9e8-137">The following example of a **RemoveDelegate** error response shows the results of a request to remove a delegate that does not exist.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ff9e8-138">コード</span><span class="sxs-lookup"><span data-stu-id="ff9e8-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ff9e8-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff9e8-139">See also</span></span>



- [<span data-ttu-id="ff9e8-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff9e8-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

