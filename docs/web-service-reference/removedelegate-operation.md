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
description: RemoveDelegate 操作は、ユーザーのメールボックスから1つ以上の代理人を削除します。
ms.openlocfilehash: b2e342225e7e79c44dcd86b76b4b7d47b16b860b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466599"
---
# <a name="removedelegate-operation"></a><span data-ttu-id="7a905-103">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="7a905-103">RemoveDelegate operation</span></span>

<span data-ttu-id="7a905-104">**Removedelegate**操作は、ユーザーのメールボックスから1つ以上の代理人を削除します。</span><span class="sxs-lookup"><span data-stu-id="7a905-104">The **RemoveDelegate** operation removes one or more delegates from a user's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="7a905-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a905-105">SOAP Headers</span></span>

<span data-ttu-id="7a905-106">**Removedelegate**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7a905-106">The **RemoveDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="7a905-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="7a905-107">**Header**</span></span>|<span data-ttu-id="7a905-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a905-108">**Element**</span></span>|<span data-ttu-id="7a905-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a905-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7a905-110">偽装</span><span class="sxs-lookup"><span data-stu-id="7a905-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="7a905-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7a905-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7a905-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a905-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="7a905-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7a905-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="7a905-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7a905-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="7a905-115">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="7a905-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="7a905-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="7a905-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="7a905-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7a905-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7a905-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a905-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="7a905-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="7a905-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="7a905-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7a905-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7a905-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a905-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="removedelegate-request-example"></a><span data-ttu-id="7a905-122">RemoveDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="7a905-122">RemoveDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="7a905-123">Description</span><span class="sxs-lookup"><span data-stu-id="7a905-123">Description</span></span>

<span data-ttu-id="7a905-124">次のコード例は、user1 メールボックスから2つの代理人を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a905-124">The following code example shows how to remove two delegates from user1's mailbox.</span></span> <span data-ttu-id="7a905-125">この例では、代理人のプライマリ SMTP アドレスを使用して1つの委任が削除され、もう1つのデリゲートは代理人のセキュリティ識別子 (SID) を使用して削除されます。</span><span class="sxs-lookup"><span data-stu-id="7a905-125">In this example, one delegate is removed by using the delegate's primary SMTP address, and the other one is removed by using the delegate's security identifier (SID).</span></span>
  
### <a name="code"></a><span data-ttu-id="7a905-126">コード</span><span class="sxs-lookup"><span data-stu-id="7a905-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="7a905-127">コメント</span><span class="sxs-lookup"><span data-stu-id="7a905-127">Comments</span></span>

<span data-ttu-id="7a905-128">**Removedelegate**操作では、指定された代理ユーザーがメールボックスを持っていたり、Active directory ディレクトリサービスに存在していたりする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="7a905-128">The **RemoveDelegate** operation does not require the specified delegate user to have a mailbox or to exist in the Active Directory directory service.</span></span> <span data-ttu-id="7a905-129">委任エントリが孤立している場合、 **removedelegate**操作は成功します。</span><span class="sxs-lookup"><span data-stu-id="7a905-129">The **RemoveDelegate** operation will succeed if the delegate entry is orphaned.</span></span> 
  
## <a name="removedelegate-response-example"></a><span data-ttu-id="7a905-130">RemoveDelegate 応答の例</span><span class="sxs-lookup"><span data-stu-id="7a905-130">RemoveDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="7a905-131">Description</span><span class="sxs-lookup"><span data-stu-id="7a905-131">Description</span></span>

<span data-ttu-id="7a905-132">**Removedelegate**応答の次の例は、 **removedelegate**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a905-132">The following example of a **RemoveDelegate** response shows a successful response to a **RemoveDelegate** request.</span></span> <span data-ttu-id="7a905-133">応答には、メールボックスから削除された各代理人の**DelegateUserResponseMessageType**要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a905-133">The response contains a **DelegateUserResponseMessageType** element for each delegate that is removed from the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7a905-134">コード</span><span class="sxs-lookup"><span data-stu-id="7a905-134">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="removedelegate-error-response-example"></a><span data-ttu-id="7a905-135">RemoveDelegate エラーの応答の例</span><span class="sxs-lookup"><span data-stu-id="7a905-135">RemoveDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="7a905-136">Description</span><span class="sxs-lookup"><span data-stu-id="7a905-136">Description</span></span>

<span data-ttu-id="7a905-137">次に示す**Removedelegate**エラー応答の例は、存在しない代理人を削除する要求の結果を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a905-137">The following example of a **RemoveDelegate** error response shows the results of a request to remove a delegate that does not exist.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7a905-138">コード</span><span class="sxs-lookup"><span data-stu-id="7a905-138">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a><span data-ttu-id="7a905-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a905-139">See also</span></span>



- [<span data-ttu-id="7a905-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a905-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

