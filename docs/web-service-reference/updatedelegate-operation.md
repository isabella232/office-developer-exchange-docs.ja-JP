---
title: UpdateDelegate 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: 03f618ac-ad1a-4772-9b81-c5bb0f12d6ab
description: UpdateDelegate 操作は、プリンシパルのメールボックスの代理アクセス許可を更新します。
ms.openlocfilehash: b7cf5325d925f8d6588115a8657a2077e940f9d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468559"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="18cc5-103">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="18cc5-103">UpdateDelegate operation</span></span>

<span data-ttu-id="18cc5-104">**Updatedelegate**操作は、プリンシパルのメールボックスの代理アクセス許可を更新します。</span><span class="sxs-lookup"><span data-stu-id="18cc5-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="18cc5-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18cc5-105">SOAP Headers</span></span>

<span data-ttu-id="18cc5-106">**Updatedelegate**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="18cc5-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="18cc5-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="18cc5-107">**Header**</span></span>|<span data-ttu-id="18cc5-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="18cc5-108">**Element**</span></span>|<span data-ttu-id="18cc5-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="18cc5-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18cc5-110">偽装</span><span class="sxs-lookup"><span data-stu-id="18cc5-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="18cc5-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="18cc5-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="18cc5-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="18cc5-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="18cc5-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="18cc5-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="18cc5-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="18cc5-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="18cc5-115">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="18cc5-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="18cc5-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="18cc5-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="18cc5-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="18cc5-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="18cc5-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="18cc5-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="18cc5-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="18cc5-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="18cc5-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="18cc5-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="18cc5-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="18cc5-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="18cc5-122">UpdateDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="18cc5-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="18cc5-123">説明</span><span class="sxs-lookup"><span data-stu-id="18cc5-123">Description</span></span>

<span data-ttu-id="18cc5-124">次の**updatedelegate**要求の例は、user1 アカウントの代理アクセス許可を更新する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="18cc5-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="18cc5-125">User2 には、タスクフォルダーの [なし] アクセス許可レベルが与えられており、プライベートアイテムを表示するためのアクセス許可が付与されています。</span><span class="sxs-lookup"><span data-stu-id="18cc5-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="18cc5-126">User3 には、ジャーナルフォルダーに対するレビュー担当者のアクセス許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="18cc5-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="18cc5-127">会議出席依頼は代理人に送信され、要求に関する情報は User1 に送信されます。</span><span class="sxs-lookup"><span data-stu-id="18cc5-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="18cc5-128">コード</span><span class="sxs-lookup"><span data-stu-id="18cc5-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ViewPrivateItems>true</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user3@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:JournalFolderPermissionLevel>Reviewer</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndSendInformationToMe</DeliverMeetingRequests>
    </UpdateDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="18cc5-129">コメント</span><span class="sxs-lookup"><span data-stu-id="18cc5-129">Comments</span></span>

<span data-ttu-id="18cc5-130">[Updatedelegate](updatedelegate.md)要求では、更新が代理人に適用される必要はありません。</span><span class="sxs-lookup"><span data-stu-id="18cc5-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="18cc5-131">クライアントは、 **DeliverMeetingMessage**設定のみを変更できます。</span><span class="sxs-lookup"><span data-stu-id="18cc5-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="18cc5-132">UpdateDelegate 応答の例</span><span class="sxs-lookup"><span data-stu-id="18cc5-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="18cc5-133">説明</span><span class="sxs-lookup"><span data-stu-id="18cc5-133">Description</span></span>

<span data-ttu-id="18cc5-134">次の例は、 **Updatedelegate**操作に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="18cc5-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="18cc5-135">コード</span><span class="sxs-lookup"><span data-stu-id="18cc5-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1117</t:SID>
              <t:PrimarySmtpAddress>User2@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User2</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>true</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
              <t:PrimarySmtpAddress>User3@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User3</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="18cc5-136">UpdateDelegate エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="18cc5-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="18cc5-137">説明</span><span class="sxs-lookup"><span data-stu-id="18cc5-137">Description</span></span>

<span data-ttu-id="18cc5-138">次の例は、 **Updatedelegate**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="18cc5-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="18cc5-139">代理人がプリンシパルの委任リストに存在しないため、エラーが生成されました。</span><span class="sxs-lookup"><span data-stu-id="18cc5-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="18cc5-140">コード</span><span class="sxs-lookup"><span data-stu-id="18cc5-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="18cc5-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="18cc5-141">See also</span></span>



- [<span data-ttu-id="18cc5-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="18cc5-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

