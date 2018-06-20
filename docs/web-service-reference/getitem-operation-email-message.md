---
title: GetItem 操作 (電子メール)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e8492e3b-1c8d-4b14-8070-9530f8306edd
description: GetItem 操作は、電子メール メッセージに関する情報にアクセスできます。
ms.openlocfilehash: 133a893ec7cd0c206d9db573f8b952eb3c2286df
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760775"
---
# <a name="getitem-operation-email-message"></a><span data-ttu-id="2cabb-103">GetItem 操作 (電子メール)</span><span class="sxs-lookup"><span data-stu-id="2cabb-103">GetItem operation (email message)</span></span>

<span data-ttu-id="2cabb-104">GetItem 操作は、電子メール メッセージに関する情報にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2cabb-104">The GetItem operation allows the user to access information about e-mail messages.</span></span>
  
## <a name="using-the-getitem-operation-for-messages"></a><span data-ttu-id="2cabb-105">メッセージの GetItem 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="2cabb-105">Using the GetItem Operation for Messages</span></span>

<span data-ttu-id="2cabb-106">GetItem 要求は、次の情報を用意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cabb-106">The GetItem request must have the following information:</span></span>
  
- <span data-ttu-id="2cabb-107">返される項目の情報を識別するのには[アイテム Id](itemid.md)の要素です。</span><span class="sxs-lookup"><span data-stu-id="2cabb-107">The [ItemId](itemid.md) element to identify the item information to return.</span></span> 
    
- <span data-ttu-id="2cabb-108">返す項目のプロパティを識別する[ItemShape](itemshape.md)要素です。</span><span class="sxs-lookup"><span data-stu-id="2cabb-108">The [ItemShape](itemshape.md) element to identify the item properties to return.</span></span> 
    
## <a name="getitem-request-example"></a><span data-ttu-id="2cabb-109">GetItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="2cabb-109">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="2cabb-110">説明</span><span class="sxs-lookup"><span data-stu-id="2cabb-110">Description</span></span>

<span data-ttu-id="2cabb-111">GetItem 要求の次の例では、電子メール メッセージに関する情報にアクセスする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="2cabb-111">The following example of a GetItem request shows how to access information about e-mail messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="2cabb-112">コード</span><span class="sxs-lookup"><span data-stu-id="2cabb-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAlAF" ChangeKey="CQAAAB" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="2cabb-113">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="2cabb-113">Request elements</span></span>

<span data-ttu-id="2cabb-114">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cabb-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2cabb-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="2cabb-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="2cabb-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="2cabb-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="2cabb-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="2cabb-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="2cabb-118">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="2cabb-118">IncludeMimeContent</span></span>](includemimecontent.md)
    
- [<span data-ttu-id="2cabb-119">Itemid</span><span class="sxs-lookup"><span data-stu-id="2cabb-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2cabb-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="2cabb-120">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-e-mail-message-response-example"></a><span data-ttu-id="2cabb-121">成功 GetItem (電子メール メッセージ) の応答の例</span><span class="sxs-lookup"><span data-stu-id="2cabb-121">Successful GetItem (E-mail Message) response example</span></span>

### <a name="description"></a><span data-ttu-id="2cabb-122">説明</span><span class="sxs-lookup"><span data-stu-id="2cabb-122">Description</span></span>

<span data-ttu-id="2cabb-123">GetItem 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cabb-123">The following example shows a successful response to the GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="2cabb-124">コード</span><span class="sxs-lookup"><span data-stu-id="2cabb-124">Code</span></span>

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
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:MimeContent CharacterSet="UTF-8">UmVjZWl</t:MimeContent>
              <t:ItemId Id="AAAlAFVz" ChangeKey="CQAAAB" />
              <t:Subject />
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="HTML">
                <html dir="ltr">
                  <head>
                    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
                      <meta content="MSHTML 6.00.3790.2759" name="GENERATOR">
                        <style title="owaParaStyle">P { MARGIN-TOP: 0px; MARGIN-BOTTOM: 0px } </style>
                      </head>
                  <body ocsi="x">
                    <div dir="ltr">
                      <font face="Tahoma" color="#000000" size="2"></font>&amp;nbsp;
                    </div>
                  </body>
                </html>
              </t:Body>
              <t:Size>881</t:Size>
              <t:DateTimeSent>2006-10-28T01:37:06Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-10-28T01:37:06Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ReplyToItem />
                <t:ReplyAllToItem />
                <t:ForwardItem />
              </t:ResponseObjects>
              <t:HasAttachments>false</t:HasAttachments>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>User1</t:Name>
                  <t:EmailAddress>User1@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:ToRecipients>
              <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
              <t:IsDeliveryReceiptRequested>false</t:IsDeliveryReceiptRequested>
              <t:From>
                <t:Mailbox>
                  <t:Name>User2</t:Name>
                  <t:EmailAddress>User2@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:From>
              <t:IsRead>false</t:IsRead>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2cabb-125">コメント</span><span class="sxs-lookup"><span data-stu-id="2cabb-125">Comments</span></span>

<span data-ttu-id="2cabb-126">MIME コンテンツ、フォルダー、およびアイテムの識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2cabb-126">The MIME content, folder, and item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="2cabb-127">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="2cabb-127">Successful response elements</span></span>

<span data-ttu-id="2cabb-128">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cabb-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2cabb-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2cabb-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2cabb-130">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="2cabb-130">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="2cabb-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cabb-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2cabb-132">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2cabb-132">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="2cabb-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2cabb-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2cabb-134">Items</span><span class="sxs-lookup"><span data-stu-id="2cabb-134">Items</span></span>](items.md)
    
- [<span data-ttu-id="2cabb-135">Message</span><span class="sxs-lookup"><span data-stu-id="2cabb-135">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="2cabb-136">MimeContent</span><span class="sxs-lookup"><span data-stu-id="2cabb-136">MimeContent</span></span>](mimecontent.md)
    
- [<span data-ttu-id="2cabb-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="2cabb-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="2cabb-138">Subject</span><span class="sxs-lookup"><span data-stu-id="2cabb-138">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="2cabb-139">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="2cabb-139">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="2cabb-140">Body/本文</span><span class="sxs-lookup"><span data-stu-id="2cabb-140">Body</span></span>](body.md)
    
- [<span data-ttu-id="2cabb-141">Size</span><span class="sxs-lookup"><span data-stu-id="2cabb-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="2cabb-142">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="2cabb-142">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="2cabb-143">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="2cabb-143">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="2cabb-144">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="2cabb-144">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="2cabb-145">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2cabb-145">ReplyToItem</span></span>](replytoitem.md)
    
- [<span data-ttu-id="2cabb-146">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="2cabb-146">ReplyAllToItem</span></span>](replyalltoitem.md)
    
- [<span data-ttu-id="2cabb-147">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="2cabb-147">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="2cabb-148">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="2cabb-148">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="2cabb-149">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="2cabb-149">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="2cabb-150">メールボックス</span><span class="sxs-lookup"><span data-stu-id="2cabb-150">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="2cabb-151">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2cabb-151">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="2cabb-152">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="2cabb-152">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="2cabb-153">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="2cabb-153">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="2cabb-154">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2cabb-154">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md)
    
- [<span data-ttu-id="2cabb-155">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2cabb-155">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md)
    
- [<span data-ttu-id="2cabb-156">From</span><span class="sxs-lookup"><span data-stu-id="2cabb-156">From</span></span>](from.md)
    
- [<span data-ttu-id="2cabb-157">IsRead</span><span class="sxs-lookup"><span data-stu-id="2cabb-157">IsRead</span></span>](isread.md)
    
## <a name="getitem-e-mail-message-error-response-example"></a><span data-ttu-id="2cabb-158">GetItem (電子メール メッセージ) のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="2cabb-158">GetItem (E-mail Message) Error response example</span></span>

### <a name="description"></a><span data-ttu-id="2cabb-159">説明</span><span class="sxs-lookup"><span data-stu-id="2cabb-159">Description</span></span>

<span data-ttu-id="2cabb-160">GetItem 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cabb-160">The following example shows an error response to a GetItem request.</span></span> <span data-ttu-id="2cabb-161">無効な追加のプロパティを取得しようとしてエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="2cabb-161">The error was caused by an attempt to get an invalid additional property.</span></span>
  
### <a name="code"></a><span data-ttu-id="2cabb-162">コード</span><span class="sxs-lookup"><span data-stu-id="2cabb-162">Code</span></span>

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
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Property is not valid for this object type.</m:MessageText>
          <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
          </m:MessageXml>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="2cabb-163">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="2cabb-163">Error response elements</span></span>

<span data-ttu-id="2cabb-164">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2cabb-164">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2cabb-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2cabb-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2cabb-166">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="2cabb-166">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="2cabb-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cabb-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2cabb-168">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2cabb-168">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="2cabb-169">MessageText</span><span class="sxs-lookup"><span data-stu-id="2cabb-169">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2cabb-170">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2cabb-170">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2cabb-171">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2cabb-171">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="2cabb-172">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2cabb-172">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="2cabb-173">FieldURI</span><span class="sxs-lookup"><span data-stu-id="2cabb-173">FieldURI</span></span>](fielduri.md)
    
## <a name="see-also"></a><span data-ttu-id="2cabb-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cabb-174">See also</span></span>



<span data-ttu-id="2cabb-175">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="2cabb-175">[GetItem operation](getitem-operation.md)</span></span>

