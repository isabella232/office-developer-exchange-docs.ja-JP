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
description: GetRooms 操作は、指定した会議室リスト内のルームを取得します。
ms.openlocfilehash: 4cb124b96637b9fcdca15595faebb2ce4d304de0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460548"
---
# <a name="getrooms-operation"></a><span data-ttu-id="f37df-103">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="f37df-103">GetRooms operation</span></span>

<span data-ttu-id="f37df-104">**Getrooms**操作は、指定した会議室リスト内のルームを取得します。</span><span class="sxs-lookup"><span data-stu-id="f37df-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="f37df-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f37df-105">SOAP Headers</span></span>

<span data-ttu-id="f37df-106">**Getrooms**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f37df-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="f37df-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="f37df-107">**Header**</span></span>|<span data-ttu-id="f37df-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="f37df-108">**Element**</span></span>|<span data-ttu-id="f37df-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="f37df-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f37df-110">偽装</span><span class="sxs-lookup"><span data-stu-id="f37df-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="f37df-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f37df-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f37df-112">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f37df-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="f37df-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f37df-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="f37df-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f37df-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f37df-115">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="f37df-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="f37df-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="f37df-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="f37df-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f37df-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f37df-118">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="f37df-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="f37df-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="f37df-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="f37df-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f37df-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f37df-121">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="f37df-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="f37df-122">GetRooms 要求の例</span><span class="sxs-lookup"><span data-stu-id="f37df-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="f37df-123">Description</span><span class="sxs-lookup"><span data-stu-id="f37df-123">Description</span></span>

<span data-ttu-id="f37df-124">ルームリストに関連付けられているルームを取得する**getrooms**要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f37df-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f37df-125">コード</span><span class="sxs-lookup"><span data-stu-id="f37df-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="f37df-126">Request 要素</span><span class="sxs-lookup"><span data-stu-id="f37df-126">Request elements</span></span>

<span data-ttu-id="f37df-127">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f37df-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f37df-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f37df-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="f37df-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="f37df-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="f37df-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="f37df-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="f37df-131">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="f37df-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="f37df-132">正常な GetRooms 応答の例</span><span class="sxs-lookup"><span data-stu-id="f37df-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="f37df-133">Description</span><span class="sxs-lookup"><span data-stu-id="f37df-133">Description</span></span>

<span data-ttu-id="f37df-134">次の応答は、会議室リストに関連付けられているルームの電子メールアドレス情報を示しています。</span><span class="sxs-lookup"><span data-stu-id="f37df-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="f37df-135">コード</span><span class="sxs-lookup"><span data-stu-id="f37df-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="f37df-136">正常な GetRooms 応答要素</span><span class="sxs-lookup"><span data-stu-id="f37df-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="f37df-137">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f37df-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f37df-138">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f37df-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f37df-139">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="f37df-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="f37df-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f37df-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f37df-141">ルーム</span><span class="sxs-lookup"><span data-stu-id="f37df-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="f37df-142">作る</span><span class="sxs-lookup"><span data-stu-id="f37df-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="f37df-143">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f37df-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="f37df-144">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="f37df-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="f37df-145">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f37df-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="f37df-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="f37df-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="f37df-147">GetRooms エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="f37df-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="f37df-148">Description</span><span class="sxs-lookup"><span data-stu-id="f37df-148">Description</span></span>

<span data-ttu-id="f37df-149">次の例は、存在しない会議室一覧の会議室情報を取得しようとしたときに発生するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f37df-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="f37df-150">コード</span><span class="sxs-lookup"><span data-stu-id="f37df-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="f37df-151">GetRooms エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="f37df-151">GetRooms Error response elements</span></span>

<span data-ttu-id="f37df-152">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f37df-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f37df-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f37df-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f37df-154">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="f37df-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="f37df-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="f37df-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f37df-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f37df-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f37df-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f37df-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="f37df-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="f37df-158">See also</span></span>

- [<span data-ttu-id="f37df-159">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="f37df-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="f37df-160">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f37df-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

