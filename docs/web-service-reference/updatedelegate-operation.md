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
description: UpdateDelegate 操作では、プリンシパルのメールボックスに代理アクセス権を更新します。
ms.openlocfilehash: 9f69d784617d10d8902a260bbf6639703dd33b6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839829"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="a27ca-103">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="a27ca-103">UpdateDelegate operation</span></span>

<span data-ttu-id="a27ca-104">**UpdateDelegate**操作では、プリンシパルのメールボックスに代理アクセス権を更新します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="a27ca-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a27ca-105">SOAP Headers</span></span>

<span data-ttu-id="a27ca-106">**UpdateDelegate**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a27ca-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a27ca-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="a27ca-107">**Header**</span></span>|<span data-ttu-id="a27ca-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="a27ca-108">**Element**</span></span>|<span data-ttu-id="a27ca-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="a27ca-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a27ca-110">偽装</span><span class="sxs-lookup"><span data-stu-id="a27ca-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="a27ca-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a27ca-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a27ca-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="a27ca-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a27ca-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="a27ca-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a27ca-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a27ca-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a27ca-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="a27ca-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="a27ca-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a27ca-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a27ca-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="a27ca-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="a27ca-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a27ca-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a27ca-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a27ca-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="a27ca-122">UpdateDelegate 要求の例</span><span class="sxs-lookup"><span data-stu-id="a27ca-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="a27ca-123">説明</span><span class="sxs-lookup"><span data-stu-id="a27ca-123">Description</span></span>

<span data-ttu-id="a27ca-124">**UpdateDelegate**要求の次の例では、user1 のアカウントのアクセス許可の委任を更新する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="a27ca-125">User2 は、[なし] アクセス許可は、[仕事] フォルダーのレベルし、プライベートなアイテムを表示するのには許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="a27ca-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="a27ca-126">User3 には、履歴フォルダーの参照者アクセス許可が与えられます。</span><span class="sxs-lookup"><span data-stu-id="a27ca-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="a27ca-127">、代理人に会議出席依頼が送信され、要求に関する情報は、User1 に送信されます。</span><span class="sxs-lookup"><span data-stu-id="a27ca-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a27ca-128">コード</span><span class="sxs-lookup"><span data-stu-id="a27ca-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="a27ca-129">コメント</span><span class="sxs-lookup"><span data-stu-id="a27ca-129">Comments</span></span>

<span data-ttu-id="a27ca-130">[UpdateDelegate](updatedelegate.md)要求では、代理人に、更新プログラムを適用することは不要です。</span><span class="sxs-lookup"><span data-stu-id="a27ca-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="a27ca-131">クライアントは、 **DeliverMeetingMessage**の設定だけを変更できます。</span><span class="sxs-lookup"><span data-stu-id="a27ca-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="a27ca-132">UpdateDelegate の応答の例</span><span class="sxs-lookup"><span data-stu-id="a27ca-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="a27ca-133">説明</span><span class="sxs-lookup"><span data-stu-id="a27ca-133">Description</span></span>

<span data-ttu-id="a27ca-134">**UpdateDelegate**操作を正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a27ca-135">コード</span><span class="sxs-lookup"><span data-stu-id="a27ca-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="a27ca-136">UpdateDelegate エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="a27ca-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="a27ca-137">説明</span><span class="sxs-lookup"><span data-stu-id="a27ca-137">Description</span></span>

<span data-ttu-id="a27ca-138">**UpdateDelegate**要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a27ca-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="a27ca-139">主体の代理人] ボックスの一覧で代理人が存在しないために、エラーが生成されました。</span><span class="sxs-lookup"><span data-stu-id="a27ca-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a27ca-140">コード</span><span class="sxs-lookup"><span data-stu-id="a27ca-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a27ca-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="a27ca-141">See also</span></span>



- [<span data-ttu-id="a27ca-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a27ca-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

