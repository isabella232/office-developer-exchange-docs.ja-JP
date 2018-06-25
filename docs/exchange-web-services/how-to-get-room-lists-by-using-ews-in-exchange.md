---
title: Exchange EWS を使用して、ルームの一覧を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 15980e4a-e41c-4194-829a-cadbdf365bf1
description: EWS マネージ API または EWS を使用して、Exchange サーバーから組織内の会議室一覧のすべて、または個室の会議室の一覧を取得する方法について説明します。
ms.openlocfilehash: 404a31fb6c8d98bdbba4c79ed6912c333a44d04b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758953"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a><span data-ttu-id="b33e7-103">Exchange EWS を使用して、ルームの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-103">Get room lists by using EWS in Exchange</span></span>

<span data-ttu-id="b33e7-104">EWS マネージ API または EWS を使用して、Exchange サーバーから組織内の会議室一覧のすべて、または個室の会議室の一覧を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-104">Learn how to get a list of all the room lists in your organization or a single room list from an Exchange server by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="b33e7-105">EWS のマネージ API または EWS を使用するには、部屋と部屋が組織内でグループ化する方法に関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-105">You can use the EWS Managed API or EWS to get information about rooms and how the rooms are grouped in your organization.</span></span> <span data-ttu-id="b33e7-106">ルームの一覧は、既定では存在しません。管理者は、作成し、それらを整理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b33e7-106">Room lists don't exist by default; your administrator needs to create and organize them.</span></span> <span data-ttu-id="b33e7-107">通常、次の例のようにに拠点や部門で整理しています。</span><span class="sxs-lookup"><span data-stu-id="b33e7-107">Typically, they're organized by location or department, as shown in the following example.</span></span>
  
<span data-ttu-id="b33e7-108">**Contoso ルームの一覧の名前と電子メール アドレス**</span><span class="sxs-lookup"><span data-stu-id="b33e7-108">**Contoso room list names and email addresses**</span></span>

|<span data-ttu-id="b33e7-109">**ルーム リストの名前**</span><span class="sxs-lookup"><span data-stu-id="b33e7-109">**Name of room list**</span></span>|<span data-ttu-id="b33e7-110">**ルーム リストの電子メール アドレス**</span><span class="sxs-lookup"><span data-stu-id="b33e7-110">**Email address of room list**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b33e7-111">11号棟の会議室一覧</span><span class="sxs-lookup"><span data-stu-id="b33e7-111">Building 11 room list</span></span>  <br/> |<span data-ttu-id="b33e7-112">Bldg11rooms@contoso.com</span><span class="sxs-lookup"><span data-stu-id="b33e7-112">Bldg11rooms@contoso.com</span></span>  <br/> |
|<span data-ttu-id="b33e7-113">ヘルス サイエンス棟の会議室一覧</span><span class="sxs-lookup"><span data-stu-id="b33e7-113">Health Science Building Conference Room List</span></span>  <br/> |<span data-ttu-id="b33e7-114">HSbldgrooms@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="b33e7-114">HSbldgrooms@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="b33e7-115">経理フロアの会議室</span><span class="sxs-lookup"><span data-stu-id="b33e7-115">Accounting Floor Meeting Rooms</span></span>  <br/> |<span data-ttu-id="b33e7-116">Acctfloor300@contoso.com</span><span class="sxs-lookup"><span data-stu-id="b33e7-116">Acctfloor300@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="b33e7-117">会議室一覧の各会議室には、それに関連する名前と電子メール アドレスがあります。</span><span class="sxs-lookup"><span data-stu-id="b33e7-117">Each room in a room list has a name and email address associated with it.</span></span>
  
<span data-ttu-id="b33e7-118">**Contoso の部屋の名前と電子メール アドレス**</span><span class="sxs-lookup"><span data-stu-id="b33e7-118">**Contoso room names and email addresses**</span></span>

|<span data-ttu-id="b33e7-119">**ルームの名前**</span><span class="sxs-lookup"><span data-stu-id="b33e7-119">**Name of room**</span></span>|<span data-ttu-id="b33e7-120">**ルームの電子メール アドレス**</span><span class="sxs-lookup"><span data-stu-id="b33e7-120">**Email address of room**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b33e7-121">会議室 11/101 (8) AV</span><span class="sxs-lookup"><span data-stu-id="b33e7-121">Conf Room 11/101 (8) AV</span></span>  <br/> |<span data-ttu-id="b33e7-122">Cf11101@contoso.com</span><span class="sxs-lookup"><span data-stu-id="b33e7-122">Cf11101@contoso.com</span></span>  <br/> |
|<span data-ttu-id="b33e7-123">HS デモンストレーション ラボ (100)</span><span class="sxs-lookup"><span data-stu-id="b33e7-123">HS Demonstration Lab (100)</span></span>  <br/> |<span data-ttu-id="b33e7-124">Hs101@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="b33e7-124">Hs101@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="b33e7-125">経理 305 WB</span><span class="sxs-lookup"><span data-stu-id="b33e7-125">Accounting 305 WB</span></span>  <br/> |<span data-ttu-id="b33e7-126">Acct305@contoso.com</span><span class="sxs-lookup"><span data-stu-id="b33e7-126">Acct305@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="b33e7-127">[ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx)の EWS の操作のいずれかを使用して、ルームのすべてのリストを含む一覧を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="b33e7-127">You can get a list that contains all room lists by using either the [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="b33e7-128">[GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx)の EWS の操作を使用して、電子メール アドレスを指定することにより、場所または部門のすべての会議室を含む 1 つの会議室の一覧を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="b33e7-128">You can retrieve a single room list that contains all the rooms for a location or department by supplying its email address by using the [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="b33e7-129">会議室の一覧に関連付けられている部屋のコレクションがある場合、室や、会議室を識別する電子メール アドレス、または"AV"、または「ラボ」など、名前のキーワードを調べることによってコレクションを検索できます。</span><span class="sxs-lookup"><span data-stu-id="b33e7-129">When you have a collection of rooms associated with a room list, you can then search through the collection to identify the room or rooms you want, either by email address, or by looking for key words in the name, such as "AV", or "Lab".</span></span> 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a><span data-ttu-id="b33e7-130">EWS マネージ API を使用して、全会議室一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="b33e7-130">Get all room lists by using the EWS Managed API</span></span>
<span data-ttu-id="b33e7-131"><a name="bk_GetRoomListewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b33e7-131"></span></span>

<span data-ttu-id="b33e7-132">次の例では、 [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx)メソッドを使用して、組織内のすべてのルーム一覧を含むリストを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-132">The following example shows how to get a list that contains all the room lists in your organization by using the [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) method.</span></span> 
  
<span data-ttu-id="b33e7-133">次の使用例は、認証済み Exchange サーバーおよび**サービス**をという名前の[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトを取得することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="b33e7-133">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
// Return all the room lists in the organization.
// This method call results in a GetRoomLists call to EWS.
EmailAddressCollection myRoomLists = service.GetRoomLists();
// Display the room lists.
foreach (EmailAddress address in myRoomLists)
{
    Console.WriteLine("Email Address: {0} Mailbox Type: {1}", address.Address, address.MailboxType);
}

```

## <a name="get-all-room-lists-by-using-ews"></a><span data-ttu-id="b33e7-134">EWS を使用して、全会議室一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="b33e7-134">Get all room lists by using EWS</span></span>
<span data-ttu-id="b33e7-135"><a name="bk_GetRoomListews"> </a></span><span class="sxs-lookup"><span data-stu-id="b33e7-135"></span></span>

<span data-ttu-id="b33e7-136">次の例では、 [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx)操作を使用して、組織内のすべての[RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx)のコレクションを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-136">The following example shows how to get a collection of all your organization's [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) by using the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="b33e7-137">[ルームのすべてのリストを取得](#bk_GetRoomListewsma)するのには EWS のマネージ API を使用する場合、EWS のマネージ API を送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="b33e7-137">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all room lists](#bk_GetRoomListewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b33e7-138">サーバーは、組織の部屋のリストが含まれている[GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx)メッセージに[GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx)要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-138">The server responds to the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) request with a [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) message that contains the room lists for your organization.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="868" MinorBuildNumber="8" Version="V2_9" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomListsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:RoomLists>
        <t:Address>
          <t:Name>Contoso Building 1 Room List</t:Name>
          <t:EmailAddress>bldg1rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 2 Room List</t:Name>
          <t:EmailAddress>bldg2rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 3 Room List</t:Name>
          <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </m:GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a><span data-ttu-id="b33e7-139">EWS マネージ API を使用して、会議室一覧の会議室すべてを取得する</span><span class="sxs-lookup"><span data-stu-id="b33e7-139">Get all the rooms in a room list by using the EWS Managed API</span></span>
<span data-ttu-id="b33e7-140"><a name="bk_FindRoomewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b33e7-140"></span></span>

<span data-ttu-id="b33e7-141">次の例では、 [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx)メソッドを使用して会議室の一覧でルームのコレクションを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-141">The following example shows how to get a collection of rooms in a room list by using the [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) method.</span></span> 
  
```cs
EmailAddress myRoomList = "bldg3rooms@contoso.com";
// This method call results in a GetRooms call to EWS.
System.Collections.ObjectModel.Collection<EmailAddress> myRoomAddresses = service.GetRooms(myRoomList);
// Display the individual rooms.
foreach (EmailAddress address in myRoomAddresses)
{
    Console.WriteLine("Email Address: {0}", address.Address);
}

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a><span data-ttu-id="b33e7-142">EWS を使用して、会議室一覧の会議室すべてを取得する</span><span class="sxs-lookup"><span data-stu-id="b33e7-142">Get all the rooms in a room list by using EWS</span></span>
<span data-ttu-id="b33e7-143"><a name="bk_FindRoomews"> </a></span><span class="sxs-lookup"><span data-stu-id="b33e7-143"></span></span>

<span data-ttu-id="b33e7-144">次の例では、 [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx)操作を使用して、 [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) [ルーム](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx)の一覧を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-144">The following example shows how to get a list of [rooms](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) in a [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) by using the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="b33e7-145">EWS のマネージ API が[会議室の一覧内のすべての会議室を取得](#bk_FindRoomewsma)するのには EWS のマネージ API を使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="b33e7-145">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all the rooms in a room list](#bk_FindRoomewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b33e7-146">サーバーは、ルーム リストで 2 つの部屋が含まれている[GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx)メッセージの[GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx)の要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-146">The server responds to the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) request with a [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) message that contains the rooms in the room list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" 
                         Version="V2_9" xmlns:h="http://scemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://scemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Rooms>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/101 (16) AV</t:Name>
            <t:EmailAddress>cf3101@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/102 (8) AV</t:Name>
            <t:EmailAddress>cf3102@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/103 (14) AV RoundTable</t:Name>
            <t:EmailAddress>cf3103@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </m:GetRoomsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="b33e7-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="b33e7-147">See also</span></span>


- [<span data-ttu-id="b33e7-148">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="b33e7-148">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="b33e7-149">Exchange EWS を使用して空き時間情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="b33e7-149">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="b33e7-150">作成し、ルームのメールボックスの管理</span><span class="sxs-lookup"><span data-stu-id="b33e7-150">Create and Manage Room Mailboxes</span></span>](http://technet.microsoft.com/en-us/library/jj215781%28v=exchg.150%29.aspx)
    

