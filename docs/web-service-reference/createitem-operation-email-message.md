---
title: CreateItem 操作 (電子メールメッセージ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: CreateItem 操作は、電子メールメッセージを作成するために使用されます。
ms.openlocfilehash: 384ed8ff653029c2b7db0b36986d85842b0a06cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457117"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="e4676-103">CreateItem 操作 (電子メールメッセージ)</span><span class="sxs-lookup"><span data-stu-id="e4676-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="e4676-104">CreateItem 操作は、電子メールメッセージを作成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4676-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="e4676-105">CreateItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="e4676-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="e4676-106">Description</span><span class="sxs-lookup"><span data-stu-id="e4676-106">Description</span></span>

<span data-ttu-id="e4676-107">CreateItem 要求の次の例は、新しい電子メールメッセージを作成し、メッセージを送信して、そのコピーを [下書き] フォルダーに保存する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e4676-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4676-108">コード</span><span class="sxs-lookup"><span data-stu-id="e4676-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="e4676-109">Request 要素</span><span class="sxs-lookup"><span data-stu-id="e4676-109">Request elements</span></span>

<span data-ttu-id="e4676-110">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4676-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="e4676-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="e4676-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="e4676-112">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="e4676-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="e4676-113">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="e4676-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="e4676-114">Message</span><span class="sxs-lookup"><span data-stu-id="e4676-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e4676-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e4676-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="e4676-116">件名</span><span class="sxs-lookup"><span data-stu-id="e4676-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="e4676-117">Body</span><span class="sxs-lookup"><span data-stu-id="e4676-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="e4676-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="e4676-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="e4676-119">メールボックス</span><span class="sxs-lookup"><span data-stu-id="e4676-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="e4676-120">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="e4676-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="e4676-121">IsRead</span><span class="sxs-lookup"><span data-stu-id="e4676-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="e4676-122">CreateItem 操作の要求メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4676-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4676-123">[CreateItem](createitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="e4676-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="e4676-124">成功した CreateItem 応答</span><span class="sxs-lookup"><span data-stu-id="e4676-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="e4676-125">Description</span><span class="sxs-lookup"><span data-stu-id="e4676-125">Description</span></span>

<span data-ttu-id="e4676-126">次の例は、CreateItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e4676-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4676-127">コード</span><span class="sxs-lookup"><span data-stu-id="e4676-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="e4676-128">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="e4676-128">Successful response elements</span></span>

<span data-ttu-id="e4676-129">応答には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4676-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="e4676-130">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e4676-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="e4676-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e4676-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e4676-132">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e4676-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="e4676-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e4676-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e4676-134">Items</span><span class="sxs-lookup"><span data-stu-id="e4676-134">Items</span></span>](items.md)
    
<span data-ttu-id="e4676-135">CreateItem 操作の応答メッセージに関するその他のオプションについては、スキーマ階層を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4676-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4676-136">[Createitemresponse](createitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="e4676-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="e4676-137">エラー CreateItem 応答</span><span class="sxs-lookup"><span data-stu-id="e4676-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="e4676-138">Description</span><span class="sxs-lookup"><span data-stu-id="e4676-138">Description</span></span>

<span data-ttu-id="e4676-139">次の例は、CreateItem 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e4676-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4676-140">コード</span><span class="sxs-lookup"><span data-stu-id="e4676-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="e4676-141">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="e4676-141">Error response elements</span></span>

<span data-ttu-id="e4676-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e4676-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="e4676-143">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e4676-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="e4676-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e4676-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e4676-145">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e4676-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="e4676-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="e4676-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e4676-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e4676-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e4676-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e4676-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e4676-149">Items</span><span class="sxs-lookup"><span data-stu-id="e4676-149">Items</span></span>](items.md)
    
<span data-ttu-id="e4676-150">CreateItem 操作のエラー応答メッセージに関するその他のオプションについては、「スキーマ階層」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4676-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4676-151">[Createitemresponse](createitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="e4676-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e4676-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4676-152">See also</span></span>



[<span data-ttu-id="e4676-153">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="e4676-153">CreateItem operation</span></span>](createitem-operation.md)

