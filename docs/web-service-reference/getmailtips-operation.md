---
title: GetMailTips ヒント操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: GetMailTips ヒント操作は、指定されたメールボックスのメールヒント情報を取得します。
ms.openlocfilehash: 41a4bb99ee7ae4e416ec8a106968bb7869e60345
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458657"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="ab215-103">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="ab215-103">GetMailTips operation</span></span>

<span data-ttu-id="ab215-104">**Getmailtips**ヒント操作は、指定されたメールボックスのメールヒント情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="ab215-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="ab215-105">GetMailTips ヒント要求の例</span><span class="sxs-lookup"><span data-stu-id="ab215-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="ab215-106">説明</span><span class="sxs-lookup"><span data-stu-id="ab215-106">Description</span></span>

<span data-ttu-id="ab215-107">クライアントは、要求 XML を構築し、サーバーに送信します。</span><span class="sxs-lookup"><span data-stu-id="ab215-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="ab215-108">要求は、クライアントが送信しているユーザー、メールヒントを取得するメールボックス、および要求されているメールヒントを識別します。</span><span class="sxs-lookup"><span data-stu-id="ab215-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="ab215-109">この例では、クライアントは、選択したメールボックスのすべてのメールヒントを返すように要求します。</span><span class="sxs-lookup"><span data-stu-id="ab215-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="ab215-110">コード</span><span class="sxs-lookup"><span data-stu-id="ab215-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="ab215-111">Request 要素</span><span class="sxs-lookup"><span data-stu-id="ab215-111">Request elements</span></span>

<span data-ttu-id="ab215-112">要求には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab215-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="ab215-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="ab215-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="ab215-114">SendingAs</span><span class="sxs-lookup"><span data-stu-id="ab215-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="ab215-115">受信者 (Arrayof受信者 Stype)</span><span class="sxs-lookup"><span data-stu-id="ab215-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="ab215-116">Mailヒント要求</span><span class="sxs-lookup"><span data-stu-id="ab215-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="ab215-117">成功した GetMailTips ヒントの応答の例</span><span class="sxs-lookup"><span data-stu-id="ab215-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="ab215-118">説明</span><span class="sxs-lookup"><span data-stu-id="ab215-118">Description</span></span>

<span data-ttu-id="ab215-119">次の簡易オブジェクトアクセスプロトコル (SOAP) 本文の例は、 **Getmailtips ヒント**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ab215-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab215-120">コード</span><span class="sxs-lookup"><span data-stu-id="ab215-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="ab215-121">Response 要素</span><span class="sxs-lookup"><span data-stu-id="ab215-121">Response elements</span></span>

<span data-ttu-id="ab215-122">応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ab215-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="ab215-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab215-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ab215-124">メールヒント</span><span class="sxs-lookup"><span data-stu-id="ab215-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="ab215-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="ab215-125">See also</span></span>



[<span data-ttu-id="ab215-126">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="ab215-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="ab215-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ab215-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

