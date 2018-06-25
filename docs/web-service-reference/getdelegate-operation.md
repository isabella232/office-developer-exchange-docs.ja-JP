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
description: GetDelegate 操作は、指定されたメールボックスの代理人の設定を取得します。
ms.openlocfilehash: bd1a0add54ee5fd1c23b4ba09a921a9061afa394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760684"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="86886-103">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="86886-103">GetDelegate operation</span></span>

<span data-ttu-id="86886-104">**GetDelegate**操作は、指定されたメールボックスの代理人の設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="86886-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="86886-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86886-105">SOAP Headers</span></span>

<span data-ttu-id="86886-106">**GetDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="86886-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="86886-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="86886-107">**Header**</span></span>|<span data-ttu-id="86886-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="86886-108">**Element**</span></span>|<span data-ttu-id="86886-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="86886-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="86886-110">偽装</span><span class="sxs-lookup"><span data-stu-id="86886-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="86886-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="86886-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="86886-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="86886-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="86886-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="86886-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="86886-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="86886-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="86886-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="86886-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="86886-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="86886-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="86886-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="86886-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="86886-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="86886-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="86886-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="86886-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="86886-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="86886-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="86886-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="86886-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="86886-122">GetDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="86886-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="86886-123">説明</span><span class="sxs-lookup"><span data-stu-id="86886-123">Description</span></span>

<span data-ttu-id="86886-124">User3 のメールボックスに設定されているすべての代理人の代理人の設定を取得する方法を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="86886-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="86886-125">ユーザーごとにすべてのアクセス許可は、応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="86886-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="86886-126">コード</span><span class="sxs-lookup"><span data-stu-id="86886-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="86886-127">コメント</span><span class="sxs-lookup"><span data-stu-id="86886-127">Comments</span></span>

<span data-ttu-id="86886-128">[ユーザー Id](userid.md)要素を使用するには、メールボックスの代理人アクセス権限を持っているすべてのユーザーを返すのではなく個々 のユーザーを指定します。</span><span class="sxs-lookup"><span data-stu-id="86886-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="86886-129">Exchange Web サービス (EWS) は、管理グループの代理人をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="86886-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="86886-130">セキュリティ グループの代理人がいる主体の**GetDelegate**操作が呼び出された場合、EWS はエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="86886-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="86886-131">GetDelegate の応答の例</span><span class="sxs-lookup"><span data-stu-id="86886-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="86886-132">説明</span><span class="sxs-lookup"><span data-stu-id="86886-132">Description</span></span>

<span data-ttu-id="86886-133">**GetDelegate**要求に正常な応答を**GetDelegate**の応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86886-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="86886-134">応答には、代理人アクセスのアクセス許可に関する情報が含まれている、要求が配信されたか、代理人が代理人にコピーし、メッセージ、会議の出席の会議の対象にするかどうか、プライベートなアイテムを表示できます。</span><span class="sxs-lookup"><span data-stu-id="86886-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="86886-135">コード</span><span class="sxs-lookup"><span data-stu-id="86886-135">Code</span></span>

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
    <m:GetDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a><span data-ttu-id="86886-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="86886-136">See also</span></span>



- [<span data-ttu-id="86886-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="86886-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

