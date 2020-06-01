---
title: GetDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: GetDelegate 操作は、指定したメールボックスの代理人の設定を取得します。
ms.openlocfilehash: 400bf5d1cafcbb789aaa749c62c7a908622d4ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461066"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="6b829-103">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6b829-103">GetDelegate operation</span></span>

<span data-ttu-id="6b829-104">**Getdelegate**操作は、指定したメールボックスの代理人の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="6b829-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="6b829-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b829-105">SOAP Headers</span></span>

<span data-ttu-id="6b829-106">**Getdelegate**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b829-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="6b829-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="6b829-107">**Header**</span></span>|<span data-ttu-id="6b829-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b829-108">**Element**</span></span>|<span data-ttu-id="6b829-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b829-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b829-110">偽装</span><span class="sxs-lookup"><span data-stu-id="6b829-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="6b829-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="6b829-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6b829-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6b829-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="6b829-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="6b829-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="6b829-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="6b829-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="6b829-115">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b829-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="6b829-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="6b829-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="6b829-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6b829-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6b829-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="6b829-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="6b829-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="6b829-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="6b829-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6b829-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6b829-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="6b829-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="6b829-122">GetDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="6b829-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="6b829-123">説明</span><span class="sxs-lookup"><span data-stu-id="6b829-123">Description</span></span>

<span data-ttu-id="6b829-124">次のコード例は、user3's メールボックスに設定されているすべての代理人の設定を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6b829-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="6b829-125">各ユーザーのすべてのアクセス許可が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="6b829-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="6b829-126">コード</span><span class="sxs-lookup"><span data-stu-id="6b829-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="6b829-127">コメント</span><span class="sxs-lookup"><span data-stu-id="6b829-127">Comments</span></span>

<span data-ttu-id="6b829-128">[UserId](userid.md)要素を使用して、メールボックスに対する代理人アクセスのアクセス許可を持つすべてのユーザーを返すのではなく、個々のユーザーを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="6b829-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6b829-129">Exchange Web サービス (EWS) は、グループの代理人の管理をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="6b829-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="6b829-130">セキュリティグループの代理人がいるプリンシパルに対して**Getdelegate**操作が呼び出されると、EWS はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="6b829-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="6b829-131">GetDelegate 応答の例</span><span class="sxs-lookup"><span data-stu-id="6b829-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="6b829-132">説明</span><span class="sxs-lookup"><span data-stu-id="6b829-132">Description</span></span>

<span data-ttu-id="6b829-133">**Getdelegate**応答の次の例は、 **getdelegate**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="6b829-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="6b829-134">応答には、代理人のアクセス許可、代理人が会議メッセージのコピーを受信するかどうか、および会議出席依頼を配信したユーザーを表示できるかどうかに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6b829-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6b829-135">コード</span><span class="sxs-lookup"><span data-stu-id="6b829-135">Code</span></span>

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
    <m:GetDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6b829-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b829-136">See also</span></span>



- [<span data-ttu-id="6b829-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b829-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

