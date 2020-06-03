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
description: GetUserOofSettings 操作は、メールボックスユーザーの不在時 (OOF) の設定とメッセージを取得します。
ms.openlocfilehash: 622faa622b0ea231a6331ff62631885d4252c1f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457698"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="8dd97-103">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="8dd97-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="8dd97-104">**Getuseroofsettings**操作は、メールボックスユーザーの不在時 (OOF) の設定とメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="8dd97-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="8dd97-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8dd97-105">SOAP Headers</span></span>

<span data-ttu-id="8dd97-106">**Getuseroofsettings**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8dd97-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="8dd97-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="8dd97-107">**Header**</span></span>|<span data-ttu-id="8dd97-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="8dd97-108">**Element**</span></span>|<span data-ttu-id="8dd97-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="8dd97-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8dd97-110">偽装</span><span class="sxs-lookup"><span data-stu-id="8dd97-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="8dd97-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="8dd97-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="8dd97-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dd97-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="8dd97-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="8dd97-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="8dd97-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8dd97-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8dd97-115">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="8dd97-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="8dd97-116">GetUserOofSettings 操作の使用</span><span class="sxs-lookup"><span data-stu-id="8dd97-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="8dd97-117">**Getuseroofsettings**操作を使用すると、ユーザーの不在時の設定にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8dd97-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="8dd97-118">ユーザーは、ユーザーの電子メールアドレスによって識別されます。</span><span class="sxs-lookup"><span data-stu-id="8dd97-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="8dd97-119">OOF メッセージが null で、OOF が有効になっている場合、不在時メッセージは送信されません。</span><span class="sxs-lookup"><span data-stu-id="8dd97-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="8dd97-120">OOF メッセージが Microsoft office outlook によって設定されている場合、この操作は OOF メッセージを HTML 形式で返します。</span><span class="sxs-lookup"><span data-stu-id="8dd97-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="8dd97-121">GetUserOofSettings 要求の例</span><span class="sxs-lookup"><span data-stu-id="8dd97-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="8dd97-122">Description</span><span class="sxs-lookup"><span data-stu-id="8dd97-122">Description</span></span>

<span data-ttu-id="8dd97-123">次の例は、1人のユーザーの OOF 情報を取得する**Getuseroofsettings**要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="8dd97-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8dd97-124">コード</span><span class="sxs-lookup"><span data-stu-id="8dd97-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="8dd97-125">Request 要素</span><span class="sxs-lookup"><span data-stu-id="8dd97-125">Request elements</span></span>

<span data-ttu-id="8dd97-126">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8dd97-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8dd97-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="8dd97-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="8dd97-128">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="8dd97-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="8dd97-129">Address (string)</span><span class="sxs-lookup"><span data-stu-id="8dd97-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="8dd97-130">Successful GetUserOofSettings response の例</span><span class="sxs-lookup"><span data-stu-id="8dd97-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="8dd97-131">Description</span><span class="sxs-lookup"><span data-stu-id="8dd97-131">Description</span></span>

<span data-ttu-id="8dd97-132">次の例は、不在時のメッセージで無効になっている OOF 状態を示しています。</span><span class="sxs-lookup"><span data-stu-id="8dd97-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="8dd97-133">コード</span><span class="sxs-lookup"><span data-stu-id="8dd97-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="8dd97-134">Successful GetUserOofSettings response 要素</span><span class="sxs-lookup"><span data-stu-id="8dd97-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="8dd97-135">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="8dd97-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8dd97-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8dd97-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8dd97-137">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="8dd97-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="8dd97-138">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8dd97-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="8dd97-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8dd97-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8dd97-140">OofSettings</span><span class="sxs-lookup"><span data-stu-id="8dd97-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="8dd97-141">OofState</span><span class="sxs-lookup"><span data-stu-id="8dd97-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="8dd97-142">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="8dd97-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="8dd97-143">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="8dd97-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="8dd97-144">StartTime</span><span class="sxs-lookup"><span data-stu-id="8dd97-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="8dd97-145">EndTime</span><span class="sxs-lookup"><span data-stu-id="8dd97-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="8dd97-146">InternalReply</span><span class="sxs-lookup"><span data-stu-id="8dd97-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="8dd97-147">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="8dd97-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="8dd97-148">Message</span><span class="sxs-lookup"><span data-stu-id="8dd97-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="8dd97-149">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="8dd97-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="8dd97-150">GetUserOofSettings エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="8dd97-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="8dd97-151">Description</span><span class="sxs-lookup"><span data-stu-id="8dd97-151">Description</span></span>

<span data-ttu-id="8dd97-152">次の例は、別のユーザーの OOF 情報にアクセスしようとした場合に発生するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="8dd97-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="8dd97-153">コード</span><span class="sxs-lookup"><span data-stu-id="8dd97-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8dd97-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="8dd97-154">See also</span></span>



- [<span data-ttu-id="8dd97-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8dd97-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

