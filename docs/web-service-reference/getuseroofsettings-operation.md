---
title: GetUserOofSettings 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: GetUserOofSettings 操作は、メールボックス ユーザーの Office (OOF) の設定とメッセージを取得します。
ms.openlocfilehash: 75a734999842cc33c213e02dc114f23372ae51fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831691"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="bc963-103">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="bc963-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="bc963-104">**GetUserOofSettings**操作は、メールボックス ユーザーの Office (OOF) の設定とメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="bc963-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="bc963-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc963-105">SOAP Headers</span></span>

<span data-ttu-id="bc963-106">**GetUserOofSettings**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="bc963-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="bc963-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="bc963-107">**Header**</span></span>|<span data-ttu-id="bc963-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="bc963-108">**Element**</span></span>|<span data-ttu-id="bc963-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc963-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bc963-110">偽装</span><span class="sxs-lookup"><span data-stu-id="bc963-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="bc963-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="bc963-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="bc963-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="bc963-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="bc963-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="bc963-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="bc963-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bc963-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bc963-115">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="bc963-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="bc963-116">GetUserOofSettings 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="bc963-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="bc963-117">**GetUserOofSettings**操作は、ユーザーの不在時の設定へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="bc963-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="bc963-118">ユーザーは、ユーザーの電子メール アドレスで識別されます。</span><span class="sxs-lookup"><span data-stu-id="bc963-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="bc963-119">OOF メッセージが不在時が有効になっている場合は、不在時のメッセージは送信されません。</span><span class="sxs-lookup"><span data-stu-id="bc963-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="bc963-120">不在時のメッセージは、MicrosoftOfficeOutlook で設定されている場合この操作は HTML 形式で、不在時のメッセージを返します。</span><span class="sxs-lookup"><span data-stu-id="bc963-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="bc963-121">GetUserOofSettings 要求の例</span><span class="sxs-lookup"><span data-stu-id="bc963-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="bc963-122">説明</span><span class="sxs-lookup"><span data-stu-id="bc963-122">Description</span></span>

<span data-ttu-id="bc963-123">次の例では、単一のユーザーの不在時の情報を取得する**GetUserOofSettings**要求を示します。</span><span class="sxs-lookup"><span data-stu-id="bc963-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bc963-124">コード</span><span class="sxs-lookup"><span data-stu-id="bc963-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="http://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="bc963-125">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="bc963-125">Request elements</span></span>

<span data-ttu-id="bc963-126">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bc963-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="bc963-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="bc963-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="bc963-128">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="bc963-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="bc963-129">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="bc963-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="bc963-130">成功した GetUserOofSettings の応答の例</span><span class="sxs-lookup"><span data-stu-id="bc963-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="bc963-131">説明</span><span class="sxs-lookup"><span data-stu-id="bc963-131">Description</span></span>

<span data-ttu-id="bc963-132">OOF メッセージが不在時の無効な状態の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bc963-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="bc963-133">コード</span><span class="sxs-lookup"><span data-stu-id="bc963-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="bc963-134">成功した GetUserOofSettings の応答の要素</span><span class="sxs-lookup"><span data-stu-id="bc963-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="bc963-135">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bc963-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="bc963-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bc963-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bc963-137">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="bc963-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="bc963-138">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bc963-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="bc963-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bc963-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bc963-140">OofSettings</span><span class="sxs-lookup"><span data-stu-id="bc963-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="bc963-141">OofState</span><span class="sxs-lookup"><span data-stu-id="bc963-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="bc963-142">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="bc963-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="bc963-143">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="bc963-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="bc963-144">開始時刻</span><span class="sxs-lookup"><span data-stu-id="bc963-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="bc963-145">終了時刻</span><span class="sxs-lookup"><span data-stu-id="bc963-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="bc963-146">InternalReply</span><span class="sxs-lookup"><span data-stu-id="bc963-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="bc963-147">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="bc963-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="bc963-148">Message</span><span class="sxs-lookup"><span data-stu-id="bc963-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="bc963-149">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="bc963-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="bc963-150">GetUserOofSettings エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="bc963-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="bc963-151">説明</span><span class="sxs-lookup"><span data-stu-id="bc963-151">Description</span></span>

<span data-ttu-id="bc963-152">次の例では、他のユーザーの不在時の情報にアクセスしようとする原因となったエラー応答を示します。</span><span class="sxs-lookup"><span data-stu-id="bc963-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="bc963-153">コード</span><span class="sxs-lookup"><span data-stu-id="bc963-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="bc963-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc963-154">See also</span></span>



- [<span data-ttu-id="bc963-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="bc963-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

