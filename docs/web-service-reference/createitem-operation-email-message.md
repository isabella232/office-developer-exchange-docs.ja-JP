---
title: CreateItem 操作 (電子メール)
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
description: CreateItem 操作を使用して、電子メール メッセージを作成します。
ms.openlocfilehash: 591209165cfbafc2d5f4036dd8fab6659523a044
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759835"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="54fac-103">CreateItem 操作 (電子メール)</span><span class="sxs-lookup"><span data-stu-id="54fac-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="54fac-104">CreateItem 操作を使用して、電子メール メッセージを作成します。</span><span class="sxs-lookup"><span data-stu-id="54fac-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="54fac-105">CreateItem 要求の例</span><span class="sxs-lookup"><span data-stu-id="54fac-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="54fac-106">説明</span><span class="sxs-lookup"><span data-stu-id="54fac-106">Description</span></span>

<span data-ttu-id="54fac-107">CreateItem 要求の次の例では、新しい電子メール メッセージを作成、メッセージを送信し、[下書き] フォルダーのコピーを保存する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="54fac-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="54fac-108">コード</span><span class="sxs-lookup"><span data-stu-id="54fac-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="54fac-109">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="54fac-109">Request elements</span></span>

<span data-ttu-id="54fac-110">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="54fac-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="54fac-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="54fac-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="54fac-112">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="54fac-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="54fac-113">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="54fac-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="54fac-114">Message</span><span class="sxs-lookup"><span data-stu-id="54fac-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="54fac-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="54fac-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="54fac-116">Subject</span><span class="sxs-lookup"><span data-stu-id="54fac-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="54fac-117">Body/本文</span><span class="sxs-lookup"><span data-stu-id="54fac-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="54fac-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="54fac-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="54fac-119">メールボックス</span><span class="sxs-lookup"><span data-stu-id="54fac-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="54fac-120">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="54fac-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="54fac-121">IsRead</span><span class="sxs-lookup"><span data-stu-id="54fac-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="54fac-122">CreateItem 操作の要求メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="54fac-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54fac-123">[CreateItem](createitem.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="54fac-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="54fac-124">Createitem メソッドの正常な応答</span><span class="sxs-lookup"><span data-stu-id="54fac-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="54fac-125">説明</span><span class="sxs-lookup"><span data-stu-id="54fac-125">Description</span></span>

<span data-ttu-id="54fac-126">次の使用例は、CreateItem 要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="54fac-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="54fac-127">コード</span><span class="sxs-lookup"><span data-stu-id="54fac-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="54fac-128">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="54fac-128">Successful response elements</span></span>

<span data-ttu-id="54fac-129">応答では、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54fac-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="54fac-130">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="54fac-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="54fac-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="54fac-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="54fac-132">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54fac-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="54fac-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54fac-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="54fac-134">Items</span><span class="sxs-lookup"><span data-stu-id="54fac-134">Items</span></span>](items.md)
    
<span data-ttu-id="54fac-135">CreateItem 操作の応答メッセージには、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="54fac-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54fac-136">[CreateItemResponse](createitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="54fac-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="54fac-137">Createitem メソッドのエラー応答</span><span class="sxs-lookup"><span data-stu-id="54fac-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="54fac-138">説明</span><span class="sxs-lookup"><span data-stu-id="54fac-138">Description</span></span>

<span data-ttu-id="54fac-139">次の使用例は、CreateItem 要求に対してエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="54fac-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="54fac-140">コード</span><span class="sxs-lookup"><span data-stu-id="54fac-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="54fac-141">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="54fac-141">Error response elements</span></span>

<span data-ttu-id="54fac-142">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="54fac-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="54fac-143">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="54fac-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="54fac-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="54fac-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="54fac-145">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54fac-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="54fac-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="54fac-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="54fac-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54fac-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="54fac-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="54fac-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="54fac-149">Items</span><span class="sxs-lookup"><span data-stu-id="54fac-149">Items</span></span>](items.md)
    
<span data-ttu-id="54fac-150">CreateItem 操作の応答のエラー メッセージについては、他のオプションを検索するには、スキーマの階層構造を表示します。</span><span class="sxs-lookup"><span data-stu-id="54fac-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="54fac-151">[CreateItemResponse](createitemresponse.md)要素から開始します。</span><span class="sxs-lookup"><span data-stu-id="54fac-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="54fac-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="54fac-152">See also</span></span>



<span data-ttu-id="54fac-153">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="54fac-153">[CreateItem operation](createitem-operation.md)</span></span>

