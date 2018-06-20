---
title: GetRoomLists 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomLists
api_type:
- schema
ms.assetid: 55d451f9-547f-44ac-872e-9cb220ea7b7c
description: GetRoomLists 操作は、Exchange 組織内で利用可能なルームのリストを取得します。
ms.openlocfilehash: 139a669bfc6b7c4bc9bd9c07f9f9cf52954860c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760846"
---
# <a name="getroomlists-operation"></a><span data-ttu-id="52316-103">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="52316-103">GetRoomLists operation</span></span>

<span data-ttu-id="52316-104">**GetRoomLists**操作は、Exchange 組織内で利用可能なルームのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="52316-104">The **GetRoomLists** operation gets the room lists that are available within the Exchange organization.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="52316-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52316-105">SOAP Headers</span></span>

<span data-ttu-id="52316-106">**GetRoomLists**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="52316-106">The **GetRoomLists** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="52316-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="52316-107">**Header**</span></span>|<span data-ttu-id="52316-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="52316-108">**Element**</span></span>|<span data-ttu-id="52316-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="52316-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="52316-110">偽装</span><span class="sxs-lookup"><span data-stu-id="52316-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="52316-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="52316-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="52316-112">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="52316-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="52316-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="52316-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="52316-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="52316-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="52316-115">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="52316-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="52316-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="52316-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="52316-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="52316-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="52316-118">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="52316-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="52316-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="52316-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="52316-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="52316-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="52316-121">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="52316-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getroomlists-request-example"></a><span data-ttu-id="52316-122">GetRoomLists 要求の例</span><span class="sxs-lookup"><span data-stu-id="52316-122">GetRoomLists request example</span></span>

### <a name="description"></a><span data-ttu-id="52316-123">説明</span><span class="sxs-lookup"><span data-stu-id="52316-123">Description</span></span>

<span data-ttu-id="52316-124">次に、サーバー上で利用可能なルームのリストを返す**GetRoomLists**要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="52316-124">The following is an example of a **GetRoomLists** request that returns the room lists that are available on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="52316-125">コード</span><span class="sxs-lookup"><span data-stu-id="52316-125">Code</span></span>

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
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="52316-126">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="52316-126">Request elements</span></span>

<span data-ttu-id="52316-127">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="52316-127">The following element is used in the request:</span></span>
  
- [<span data-ttu-id="52316-128">GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="52316-128">GetRoomLists</span></span>](getroomlists.md)
    
## <a name="successful-getroomlists-response-example"></a><span data-ttu-id="52316-129">成功した GetRoomLists の応答の例</span><span class="sxs-lookup"><span data-stu-id="52316-129">Successful GetRoomLists response example</span></span>

### <a name="description"></a><span data-ttu-id="52316-130">説明</span><span class="sxs-lookup"><span data-stu-id="52316-130">Description</span></span>

<span data-ttu-id="52316-131">次は、 **GetRoomLists**要求への応答の例です。</span><span class="sxs-lookup"><span data-stu-id="52316-131">The following is an example of a response to a **GetRoomLists** request.</span></span> <span data-ttu-id="52316-132">この応答は、サーバー上で 1 つの部屋の一覧を示しています。</span><span class="sxs-lookup"><span data-stu-id="52316-132">This response shows one room list on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="52316-133">コード</span><span class="sxs-lookup"><span data-stu-id="52316-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Address xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Name>Room List</t:Name>
          <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-getroomlists-response-elements"></a><span data-ttu-id="52316-134">成功した GetRoomLists の応答の要素</span><span class="sxs-lookup"><span data-stu-id="52316-134">Successful GetRoomLists response elements</span></span>

<span data-ttu-id="52316-135">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="52316-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="52316-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="52316-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="52316-137">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="52316-137">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="52316-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="52316-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="52316-139">RoomLists</span><span class="sxs-lookup"><span data-stu-id="52316-139">RoomLists</span></span>](roomlists.md)
    
- [<span data-ttu-id="52316-140">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="52316-140">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="52316-141">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="52316-141">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="52316-142">MailboxType</span><span class="sxs-lookup"><span data-stu-id="52316-142">MailboxType</span></span>](mailboxtype.md)
    
### <a name="getroomlists-error-response-example"></a><span data-ttu-id="52316-143">GetRoomLists エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="52316-143">GetRoomLists Error response example</span></span>

#### <a name="description"></a><span data-ttu-id="52316-144">説明</span><span class="sxs-lookup"><span data-stu-id="52316-144">Description</span></span>

<span data-ttu-id="52316-145">ルーム リストを定義していないサーバーからルームの一覧を取得しようとする応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52316-145">The following example shows the response to an attempt to get room lists from a server that does not have any room lists defined.</span></span>
  
#### <a name="code"></a><span data-ttu-id="52316-146">コード</span><span class="sxs-lookup"><span data-stu-id="52316-146">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"/>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

#### <a name="getroomlists-error-response-elements"></a><span data-ttu-id="52316-147">GetRoomLists エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="52316-147">GetRoomLists Error response elements</span></span>

<span data-ttu-id="52316-148">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="52316-148">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="52316-149">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="52316-149">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="52316-150">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="52316-150">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="52316-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="52316-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="52316-152">RoomLists</span><span class="sxs-lookup"><span data-stu-id="52316-152">RoomLists</span></span>](roomlists.md)
    
## <a name="see-also"></a><span data-ttu-id="52316-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="52316-153">See also</span></span>



[<span data-ttu-id="52316-154">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="52316-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="52316-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="52316-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

