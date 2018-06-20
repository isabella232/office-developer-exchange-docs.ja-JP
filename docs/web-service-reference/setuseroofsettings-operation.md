---
title: SetUserOofSettings 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettings
api_type:
- schema
ms.assetid: 36277ef0-18ee-4b35-9e6e-8c321d8f5433
description: SetUserOofSettings Web メソッドは、メールボックス ユーザーの Office (OOF) の設定とメッセージを設定します。
ms.openlocfilehash: 51c2f9488f38a4adb0e291c11adc2ebfe3426f25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833469"
---
# <a name="setuseroofsettings-operation"></a><span data-ttu-id="23de7-103">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="23de7-103">SetUserOofSettings operation</span></span>

<span data-ttu-id="23de7-104">**SetUserOofSettings** Web メソッドは、メールボックス ユーザーの Office (OOF) の設定とメッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="23de7-104">The **SetUserOofSettings** Web method sets a mailbox user's Out of Office (OOF) settings and message.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="23de7-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23de7-105">SOAP Headers</span></span>

<span data-ttu-id="23de7-106">**SetUserOofSettings**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="23de7-106">The **SetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="23de7-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="23de7-107">**Header**</span></span>|<span data-ttu-id="23de7-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="23de7-108">**Element**</span></span>|<span data-ttu-id="23de7-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="23de7-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="23de7-110">偽装</span><span class="sxs-lookup"><span data-stu-id="23de7-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="23de7-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="23de7-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="23de7-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="23de7-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="23de7-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="23de7-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="23de7-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="23de7-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="23de7-115">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="23de7-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="setuseroofsettings-request-example"></a><span data-ttu-id="23de7-116">SetUserOofSettings 要求の例</span><span class="sxs-lookup"><span data-stu-id="23de7-116">SetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="23de7-117">説明</span><span class="sxs-lookup"><span data-stu-id="23de7-117">Description</span></span>

<span data-ttu-id="23de7-118">**SetUserOofSettings**要求の次の例では、10 日間、不在時の設定を設定します。</span><span class="sxs-lookup"><span data-stu-id="23de7-118">The following example of a **SetUserOofSettings** request sets an OOF setting for 10 days.</span></span> 
  
### <a name="code"></a><span data-ttu-id="23de7-119">コード</span><span class="sxs-lookup"><span data-stu-id="23de7-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-10-05T00:00:00</StartTime>
          <EndTime>2006-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="23de7-120">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="23de7-120">Request elements</span></span>

<span data-ttu-id="23de7-121">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="23de7-121">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="23de7-122">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="23de7-122">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
    
- [<span data-ttu-id="23de7-123">メールボックス (可用性)</span><span class="sxs-lookup"><span data-stu-id="23de7-123">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="23de7-124">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="23de7-124">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="23de7-125">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="23de7-125">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="23de7-126">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="23de7-126">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="23de7-127">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="23de7-127">UserOofSettings</span></span>](useroofsettings.md)
    
- [<span data-ttu-id="23de7-128">OofState</span><span class="sxs-lookup"><span data-stu-id="23de7-128">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="23de7-129">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="23de7-129">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="23de7-130">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="23de7-130">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="23de7-131">開始時刻</span><span class="sxs-lookup"><span data-stu-id="23de7-131">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="23de7-132">終了時刻</span><span class="sxs-lookup"><span data-stu-id="23de7-132">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="23de7-133">InternalReply</span><span class="sxs-lookup"><span data-stu-id="23de7-133">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="23de7-134">メッセージ (可用性)</span><span class="sxs-lookup"><span data-stu-id="23de7-134">Message (Availability)</span></span>](message-availability.md)
    
- [<span data-ttu-id="23de7-135">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="23de7-135">ExternalReply</span></span>](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a><span data-ttu-id="23de7-136">成功した SetUserOofSettings の応答の例</span><span class="sxs-lookup"><span data-stu-id="23de7-136">Successful SetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="23de7-137">説明</span><span class="sxs-lookup"><span data-stu-id="23de7-137">Description</span></span>

<span data-ttu-id="23de7-138">**SetUserOofSettings**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="23de7-138">The following example shows a successful response to the **SetUserOofSettings** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="23de7-139">コード</span><span class="sxs-lookup"><span data-stu-id="23de7-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="23de7-140">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="23de7-140">Successful response elements</span></span>

<span data-ttu-id="23de7-141">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="23de7-141">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="23de7-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="23de7-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="23de7-143">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="23de7-143">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md)
    
- [<span data-ttu-id="23de7-144">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="23de7-144">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="23de7-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="23de7-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="23de7-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="23de7-146">See also</span></span>



- [<span data-ttu-id="23de7-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="23de7-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

