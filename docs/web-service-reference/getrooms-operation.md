---
title: GetRooms 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 5501ddc0-3bfa-4da6-8e15-4223ca5499a3
description: GetRooms 操作では、部屋の指定されたリスト内で 2 つの部屋を取得します。
ms.openlocfilehash: 3718c476881ae8aa538646464e7c61845d849562
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760850"
---
# <a name="getrooms-operation"></a><span data-ttu-id="c0a7a-103">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="c0a7a-103">GetRooms operation</span></span>

<span data-ttu-id="c0a7a-104">**GetRooms**操作では、部屋の指定されたリスト内で 2 つの部屋を取得します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="c0a7a-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0a7a-105">SOAP Headers</span></span>

<span data-ttu-id="c0a7a-106">**GetRooms**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="c0a7a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="c0a7a-107">**Header**</span></span>|<span data-ttu-id="c0a7a-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0a7a-108">**Element**</span></span>|<span data-ttu-id="c0a7a-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0a7a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c0a7a-110">偽装</span><span class="sxs-lookup"><span data-stu-id="c0a7a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="c0a7a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c0a7a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c0a7a-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="c0a7a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c0a7a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="c0a7a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c0a7a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c0a7a-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="c0a7a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="c0a7a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="c0a7a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c0a7a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c0a7a-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="c0a7a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="c0a7a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="c0a7a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c0a7a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c0a7a-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="c0a7a-122">GetRooms 要求の例</span><span class="sxs-lookup"><span data-stu-id="c0a7a-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="c0a7a-123">説明</span><span class="sxs-lookup"><span data-stu-id="c0a7a-123">Description</span></span>

<span data-ttu-id="c0a7a-124">次に、会議室の一覧に関連付けられている 2 つの部屋を取得する**GetRooms**要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c0a7a-125">コード</span><span class="sxs-lookup"><span data-stu-id="c0a7a-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>

```

### <a name="request-elements"></a><span data-ttu-id="c0a7a-126">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-126">Request elements</span></span>

<span data-ttu-id="c0a7a-127">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c0a7a-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c0a7a-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="c0a7a-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="c0a7a-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="c0a7a-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="c0a7a-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="c0a7a-131">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c0a7a-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="c0a7a-132">成功した GetRooms の応答の例</span><span class="sxs-lookup"><span data-stu-id="c0a7a-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="c0a7a-133">説明</span><span class="sxs-lookup"><span data-stu-id="c0a7a-133">Description</span></span>

<span data-ttu-id="c0a7a-134">次の応答では、ルーム リストに関連付けられている会議室の電子メール アドレス情報を示します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="c0a7a-135">コード</span><span class="sxs-lookup"><span data-stu-id="c0a7a-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room02</t:Name>
            <t:EmailAddress>Room02@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="c0a7a-136">成功した GetRooms の応答の要素</span><span class="sxs-lookup"><span data-stu-id="c0a7a-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="c0a7a-137">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c0a7a-138">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c0a7a-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c0a7a-139">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="c0a7a-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="c0a7a-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0a7a-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c0a7a-141">ルーム</span><span class="sxs-lookup"><span data-stu-id="c0a7a-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="c0a7a-142">ルーム</span><span class="sxs-lookup"><span data-stu-id="c0a7a-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="c0a7a-143">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c0a7a-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="c0a7a-144">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c0a7a-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="c0a7a-145">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c0a7a-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="c0a7a-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="c0a7a-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="c0a7a-147">GetRooms エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="c0a7a-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c0a7a-148">説明</span><span class="sxs-lookup"><span data-stu-id="c0a7a-148">Description</span></span>

<span data-ttu-id="c0a7a-149">存在しない会議室の一覧の領域情報を取得しようとする原因となったエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="c0a7a-150">コード</span><span class="sxs-lookup"><span data-stu-id="c0a7a-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="c0a7a-151">GetRooms エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="c0a7a-151">GetRooms Error response elements</span></span>

<span data-ttu-id="c0a7a-152">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c0a7a-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c0a7a-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c0a7a-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c0a7a-154">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="c0a7a-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="c0a7a-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="c0a7a-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c0a7a-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0a7a-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c0a7a-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c0a7a-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="c0a7a-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0a7a-158">See also</span></span>

- [<span data-ttu-id="c0a7a-159">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="c0a7a-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="c0a7a-160">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c0a7a-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

