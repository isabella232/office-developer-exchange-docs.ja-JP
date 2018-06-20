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
description: CreateItem 操作を使用して、会議出席依頼に応答します。
ms.openlocfilehash: a8aea688e46376906554952ce8ec45022cf613e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759837"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="1f614-103">CreateItem 操作 (会議出席依頼)</span><span class="sxs-lookup"><span data-stu-id="1f614-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="1f614-104">CreateItem 操作を使用して、会議出席依頼に応答します。</span><span class="sxs-lookup"><span data-stu-id="1f614-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f614-105">備考</span><span class="sxs-lookup"><span data-stu-id="1f614-105">Remarks</span></span>

<span data-ttu-id="1f614-106">CreateItem 操作には、会議出席依頼に応答するための 3 つのオプションが用意されています: 承諾、仮承諾、または辞退します。</span><span class="sxs-lookup"><span data-stu-id="1f614-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="1f614-107">会議出席要求の例をそのまま使用します。</span><span class="sxs-lookup"><span data-stu-id="1f614-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="1f614-108">説明</span><span class="sxs-lookup"><span data-stu-id="1f614-108">Description</span></span>

<span data-ttu-id="1f614-109">次の使用例は、会議を承諾する方法を示しています。 招待状を要求します。</span><span class="sxs-lookup"><span data-stu-id="1f614-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="1f614-110">コード</span><span class="sxs-lookup"><span data-stu-id="1f614-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="1f614-111">コメント</span><span class="sxs-lookup"><span data-stu-id="1f614-111">Comments</span></span>

<span data-ttu-id="1f614-112">仮承諾または、会議出席依頼を辞退するには、 [AcceptItem](acceptitem.md)要素の代わりに[TentativelyAcceptItem](tentativelyacceptitem.md)または[DeclineItem](declineitem.md)要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="1f614-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="1f614-113">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="1f614-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="1f614-114">会議出席依頼の要素を受け入れる</span><span class="sxs-lookup"><span data-stu-id="1f614-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="1f614-115">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f614-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1f614-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="1f614-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="1f614-117">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="1f614-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="1f614-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="1f614-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="1f614-119">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="1f614-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="1f614-120">成功した会議の承諾の応答の例</span><span class="sxs-lookup"><span data-stu-id="1f614-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="1f614-121">説明</span><span class="sxs-lookup"><span data-stu-id="1f614-121">Description</span></span>

<span data-ttu-id="1f614-122">次の使用例は、CreateItem 要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="1f614-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1f614-123">コード</span><span class="sxs-lookup"><span data-stu-id="1f614-123">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="1f614-124">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="1f614-124">Successful response elements</span></span>

<span data-ttu-id="1f614-125">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f614-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1f614-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1f614-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1f614-127">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="1f614-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="1f614-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1f614-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1f614-129">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1f614-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="1f614-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1f614-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1f614-131">Items</span><span class="sxs-lookup"><span data-stu-id="1f614-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="1f614-132">会議エラー応答の例をそのまま使用します。</span><span class="sxs-lookup"><span data-stu-id="1f614-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="1f614-133">説明</span><span class="sxs-lookup"><span data-stu-id="1f614-133">Description</span></span>

<span data-ttu-id="1f614-134">次の使用例は、CreateItem 要求に対してエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="1f614-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="1f614-135">見つからないことを会議出席依頼を受け入れるようにしようとしてエラーの原因が Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="1f614-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="1f614-136">コード</span><span class="sxs-lookup"><span data-stu-id="1f614-136">Code</span></span>

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="1f614-137">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="1f614-137">Error response elements</span></span>

<span data-ttu-id="1f614-138">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f614-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="1f614-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1f614-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1f614-140">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="1f614-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="1f614-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1f614-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1f614-142">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1f614-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="1f614-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="1f614-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1f614-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1f614-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1f614-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1f614-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1f614-146">Items</span><span class="sxs-lookup"><span data-stu-id="1f614-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="1f614-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f614-147">See also</span></span>



<span data-ttu-id="1f614-148">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="1f614-148">[CreateItem operation](createitem-operation.md)</span></span>
  
[<span data-ttu-id="1f614-149">CreateItem 操作 (予定表アイテム)</span><span class="sxs-lookup"><span data-stu-id="1f614-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

