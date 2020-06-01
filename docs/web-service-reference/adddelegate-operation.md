---
title: AddDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: AddDelegate 操作は、1つ以上の代理人をプリンシパルのメールボックスに追加し、特定のアクセス許可を設定します。
ms.openlocfilehash: 80adbe71d69be1025dc9593c6a9002bc68fdcb76
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466515"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="29ebb-103">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="29ebb-103">AddDelegate operation</span></span>

<span data-ttu-id="29ebb-104">**Adddelegate**操作は、1つ以上の代理人をプリンシパルのメールボックスに追加し、特定のアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="29ebb-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29ebb-105">SOAP headers</span></span>

<span data-ttu-id="29ebb-106">**Adddelegate**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="29ebb-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="29ebb-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="29ebb-107">**Header**</span></span>|<span data-ttu-id="29ebb-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="29ebb-108">**Element**</span></span>|<span data-ttu-id="29ebb-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="29ebb-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="29ebb-110">偽装</span><span class="sxs-lookup"><span data-stu-id="29ebb-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="29ebb-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="29ebb-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="29ebb-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="29ebb-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="29ebb-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="29ebb-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="29ebb-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="29ebb-115">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="29ebb-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="29ebb-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="29ebb-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="29ebb-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="29ebb-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="29ebb-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="29ebb-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="29ebb-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="29ebb-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="29ebb-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="29ebb-122">AddDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="29ebb-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="29ebb-123">説明</span><span class="sxs-lookup"><span data-stu-id="29ebb-123">Description</span></span>

<span data-ttu-id="29ebb-124">次の**Adddelegate**要求の例では、user2 によって所有されているフォルダーに user1 の代理人アクセス許可を付与しようとしています。</span><span class="sxs-lookup"><span data-stu-id="29ebb-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="29ebb-125">User1 には、user2's の予定表フォルダーとレビューアーレベルのアクセス許可を user2's の連絡先フォルダーに付与するための、作成者レベルのアクセス許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="29ebb-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="29ebb-126">User1 は会議メッセージのコピーを受信せず、user2's メールボックス内のプライベートアイテムを表示することができません。</span><span class="sxs-lookup"><span data-stu-id="29ebb-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="29ebb-127">会議出席依頼は user1 と user2 の両方に送信されます。</span><span class="sxs-lookup"><span data-stu-id="29ebb-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="29ebb-128">コード</span><span class="sxs-lookup"><span data-stu-id="29ebb-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <AddDelegate>
      <Mailbox>
        <t:EmailAddress>user2@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user1@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndMe</DeliverMeetingRequests>
    </AddDelegate>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-response-example"></a><span data-ttu-id="29ebb-129">AddDelegate 応答の例</span><span class="sxs-lookup"><span data-stu-id="29ebb-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="29ebb-130">説明</span><span class="sxs-lookup"><span data-stu-id="29ebb-130">Description</span></span>

<span data-ttu-id="29ebb-131">Adddelegate 応答の次**AddDelegate**の例は、 **adddelegate**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="29ebb-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="29ebb-132">コード</span><span class="sxs-lookup"><span data-stu-id="29ebb-132">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="29ebb-133">AddDelegate エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="29ebb-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="29ebb-134">説明</span><span class="sxs-lookup"><span data-stu-id="29ebb-134">Description</span></span>

<span data-ttu-id="29ebb-135">次の例は、既にプリンシパルのメールボックスに追加されている代理人を追加する要求に対する応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="29ebb-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="29ebb-136">コード</span><span class="sxs-lookup"><span data-stu-id="29ebb-136">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="29ebb-137">コメント</span><span class="sxs-lookup"><span data-stu-id="29ebb-137">Comments</span></span>

<span data-ttu-id="29ebb-138">代理人を追加しようとしたときに ErrorDelegateAlreadyExists 応答コードが返された場合は、 [Getdelegate 操作](getdelegate-operation.md)を使用して代理人に対する現在のアクセス許可をすべて取得した後、 [updatedelegate 操作](updatedelegate-operation.md)を使用して新しいアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="29ebb-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="29ebb-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="29ebb-139">See also</span></span>

- [<span data-ttu-id="29ebb-140">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="29ebb-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

