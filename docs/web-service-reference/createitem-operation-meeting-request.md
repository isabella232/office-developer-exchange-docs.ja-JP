---
title: CreateItem 操作 (会議出席依頼)
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
ms.assetid: fe136881-a804-456a-8552-8a1bea5eb9c8
description: CreateItem 操作は、会議出席依頼に応答するために使用されます。
ms.openlocfilehash: f9e6bd1742e6a30d08736ea67c0ff80b7a18e88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457110"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="11e34-103">CreateItem 操作 (会議出席依頼)</span><span class="sxs-lookup"><span data-stu-id="11e34-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="11e34-104">CreateItem 操作は、会議出席依頼に応答するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="11e34-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11e34-105">注釈</span><span class="sxs-lookup"><span data-stu-id="11e34-105">Remarks</span></span>

<span data-ttu-id="11e34-106">CreateItem 操作には、会議出席依頼に返信するための3つのオプション (承諾、仮承諾、または辞退) が用意されています。</span><span class="sxs-lookup"><span data-stu-id="11e34-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="11e34-107">会議出席依頼の承諾の例</span><span class="sxs-lookup"><span data-stu-id="11e34-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="11e34-108">説明</span><span class="sxs-lookup"><span data-stu-id="11e34-108">Description</span></span>

<span data-ttu-id="11e34-109">次の例は、会議出席依頼の招待を承諾する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="11e34-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="11e34-110">コード</span><span class="sxs-lookup"><span data-stu-id="11e34-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="11e34-111">コメント</span><span class="sxs-lookup"><span data-stu-id="11e34-111">Comments</span></span>

<span data-ttu-id="11e34-112">会議出席依頼を仮承諾または辞退するには、 [Acceptitem](acceptitem.md)要素の代わりに[TentativelyAcceptItem](tentativelyacceptitem.md)または[declineitem](declineitem.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="11e34-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="11e34-113">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="11e34-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="11e34-114">会議出席依頼の要素を承諾する</span><span class="sxs-lookup"><span data-stu-id="11e34-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="11e34-115">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="11e34-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="11e34-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="11e34-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="11e34-117">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="11e34-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="11e34-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="11e34-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="11e34-119">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="11e34-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="11e34-120">正常な会議の応答の例</span><span class="sxs-lookup"><span data-stu-id="11e34-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="11e34-121">説明</span><span class="sxs-lookup"><span data-stu-id="11e34-121">Description</span></span>

<span data-ttu-id="11e34-122">次の例は、CreateItem 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="11e34-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="11e34-123">コード</span><span class="sxs-lookup"><span data-stu-id="11e34-123">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="11e34-124">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="11e34-124">Successful response elements</span></span>

<span data-ttu-id="11e34-125">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="11e34-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="11e34-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="11e34-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="11e34-127">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="11e34-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="11e34-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="11e34-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="11e34-129">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="11e34-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="11e34-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="11e34-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="11e34-131">Items</span><span class="sxs-lookup"><span data-stu-id="11e34-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="11e34-132">会議エラー応答の承諾の例</span><span class="sxs-lookup"><span data-stu-id="11e34-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="11e34-133">説明</span><span class="sxs-lookup"><span data-stu-id="11e34-133">Description</span></span>

<span data-ttu-id="11e34-134">次の例は、CreateItem 要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="11e34-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="11e34-135">このエラーは、Exchange ストアに存在しない会議出席依頼を承諾しようとしたために発生します。</span><span class="sxs-lookup"><span data-stu-id="11e34-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="11e34-136">コード</span><span class="sxs-lookup"><span data-stu-id="11e34-136">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="11e34-137">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="11e34-137">Error response elements</span></span>

<span data-ttu-id="11e34-138">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="11e34-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="11e34-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="11e34-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="11e34-140">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="11e34-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="11e34-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="11e34-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="11e34-142">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="11e34-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="11e34-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="11e34-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="11e34-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="11e34-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="11e34-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="11e34-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="11e34-146">Items</span><span class="sxs-lookup"><span data-stu-id="11e34-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="11e34-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="11e34-147">See also</span></span>



<span data-ttu-id="11e34-148">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="11e34-148">[CreateItem operation](createitem-operation.md)</span></span>
  
[<span data-ttu-id="11e34-149">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="11e34-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

