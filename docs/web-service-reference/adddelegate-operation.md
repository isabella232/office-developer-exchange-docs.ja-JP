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
description: AddDelegate 操作では、1 つまたは複数主体のメールボックスを委任し、特定のアクセス許可の設定を追加します。
ms.openlocfilehash: 28d4ded2625efc3d6eade44f5fafc06c2ffca7ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759275"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="d68fc-103">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="d68fc-103">AddDelegate operation</span></span>

<span data-ttu-id="d68fc-104">**AddDelegate**操作では、1 つまたは複数主体のメールボックスを委任し、特定のアクセス許可の設定を追加します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="d68fc-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d68fc-105">SOAP headers</span></span>

<span data-ttu-id="d68fc-106">**AddDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d68fc-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="d68fc-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="d68fc-107">**Header**</span></span>|<span data-ttu-id="d68fc-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="d68fc-108">**Element**</span></span>|<span data-ttu-id="d68fc-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="d68fc-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d68fc-110">偽装</span><span class="sxs-lookup"><span data-stu-id="d68fc-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="d68fc-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d68fc-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d68fc-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="d68fc-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d68fc-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="d68fc-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d68fc-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d68fc-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="d68fc-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="d68fc-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="d68fc-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d68fc-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d68fc-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="d68fc-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="d68fc-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="d68fc-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d68fc-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d68fc-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="d68fc-122">AddDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="d68fc-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="d68fc-123">説明</span><span class="sxs-lookup"><span data-stu-id="d68fc-123">Description</span></span>

<span data-ttu-id="d68fc-124">**AddDelegate**要求の次の使用例は、user2 が所有するフォルダーに user1 のアクセス許可の委任を付与する試みを示しています。</span><span class="sxs-lookup"><span data-stu-id="d68fc-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="d68fc-125">User1 には、user2 の予定表フォルダーと user2 の連絡先フォルダーに参照者レベルのアクセス許可を作成者レベルのアクセス許可が与えられます。</span><span class="sxs-lookup"><span data-stu-id="d68fc-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="d68fc-126">User1 は会議のメッセージのコピーを受信しませんし、user2 のメールボックスにプライベート アイテムを表示することはできません。</span><span class="sxs-lookup"><span data-stu-id="d68fc-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="d68fc-127">User1 と user2 の両方に会議出席依頼が送信されます。</span><span class="sxs-lookup"><span data-stu-id="d68fc-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d68fc-128">コード</span><span class="sxs-lookup"><span data-stu-id="d68fc-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="adddelegate-response-example"></a><span data-ttu-id="d68fc-129">AddDelegate 応答の例</span><span class="sxs-lookup"><span data-stu-id="d68fc-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="d68fc-130">説明</span><span class="sxs-lookup"><span data-stu-id="d68fc-130">Description</span></span>

<span data-ttu-id="d68fc-131">**AddDelegate**要求に正常な応答を**AddDelegate**応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d68fc-132">コード</span><span class="sxs-lookup"><span data-stu-id="d68fc-132">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="d68fc-133">AddDelegate エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="d68fc-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="d68fc-134">説明</span><span class="sxs-lookup"><span data-stu-id="d68fc-134">Description</span></span>

<span data-ttu-id="d68fc-135">主体のメールボックスに既に追加されているデリゲートを追加する要求への応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="d68fc-136">コード</span><span class="sxs-lookup"><span data-stu-id="d68fc-136">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="d68fc-137">コメント</span><span class="sxs-lookup"><span data-stu-id="d68fc-137">Comments</span></span>

<span data-ttu-id="d68fc-138">デリゲートを追加しようとすると ErrorDelegateAlreadyExists の応答コードが返された場合は、 [GetDelegate 操作](getdelegate-operation.md)を使用して、現在のすべての権限を代理人を取得し、 [UpdateDelegate 操作](updatedelegate-operation.md)を使用して新しいアクセス許可を設定するのには。</span><span class="sxs-lookup"><span data-stu-id="d68fc-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d68fc-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="d68fc-139">See also</span></span>

- [<span data-ttu-id="d68fc-140">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="d68fc-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

