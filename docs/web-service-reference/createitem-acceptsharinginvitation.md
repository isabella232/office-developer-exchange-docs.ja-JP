---
title: CreateItem (AcceptSharingInvitation)
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
ms.assetid: 710c893a-3037-4f04-b336-aefedd36c406
description: CreateItem 操作は、別のユーザーの予定表または連絡先データを共有するための招待を承諾するために使用されます。
ms.openlocfilehash: eda846b72f42fe886497b355d9cddade7c5f4044
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457516"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="e5d3d-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="e5d3d-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="e5d3d-104">**CreateItem**操作は、別のユーザーの予定表または連絡先データを共有するための招待を承諾するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="e5d3d-105">共有への招待の要求の例</span><span class="sxs-lookup"><span data-stu-id="e5d3d-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="e5d3d-106">Description</span><span class="sxs-lookup"><span data-stu-id="e5d3d-106">Description</span></span>

<span data-ttu-id="e5d3d-107">次の例は、共有への招待を承諾する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="e5d3d-108">コード</span><span class="sxs-lookup"><span data-stu-id="e5d3d-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="e5d3d-109">Request 要素</span><span class="sxs-lookup"><span data-stu-id="e5d3d-109">Request elements</span></span>

<span data-ttu-id="e5d3d-110">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e5d3d-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="e5d3d-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="e5d3d-112">Items</span><span class="sxs-lookup"><span data-stu-id="e5d3d-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="e5d3d-113">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="e5d3d-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="e5d3d-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="e5d3d-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="e5d3d-115">コメント</span><span class="sxs-lookup"><span data-stu-id="e5d3d-115">Comments</span></span>

<span data-ttu-id="e5d3d-116">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="e5d3d-117">成功した共有への招待の応答の例</span><span class="sxs-lookup"><span data-stu-id="e5d3d-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="e5d3d-118">Description</span><span class="sxs-lookup"><span data-stu-id="e5d3d-118">Description</span></span>

<span data-ttu-id="e5d3d-119">次の例は、 **CreateItem**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e5d3d-120">コード</span><span class="sxs-lookup"><span data-stu-id="e5d3d-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
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

### <a name="successful-response-elements"></a><span data-ttu-id="e5d3d-121">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="e5d3d-121">Successful response elements</span></span>

<span data-ttu-id="e5d3d-122">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e5d3d-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e5d3d-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e5d3d-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e5d3d-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="e5d3d-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e5d3d-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e5d3d-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e5d3d-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="e5d3d-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e5d3d-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e5d3d-128">Items</span><span class="sxs-lookup"><span data-stu-id="e5d3d-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="e5d3d-129">共有への招待の承諾のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="e5d3d-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="e5d3d-130">Description</span><span class="sxs-lookup"><span data-stu-id="e5d3d-130">Description</span></span>

<span data-ttu-id="e5d3d-131">次の例は、 **CreateItem**要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="e5d3d-132">このエラーは、Exchange ストアに存在しない共有への招待を承諾しようとしたことが原因で発生します。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e5d3d-133">コード</span><span class="sxs-lookup"><span data-stu-id="e5d3d-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
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

### <a name="error-response-elements"></a><span data-ttu-id="e5d3d-134">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="e5d3d-134">Error response elements</span></span>

<span data-ttu-id="e5d3d-135">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5d3d-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e5d3d-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e5d3d-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e5d3d-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e5d3d-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="e5d3d-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e5d3d-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e5d3d-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e5d3d-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="e5d3d-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="e5d3d-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e5d3d-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e5d3d-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e5d3d-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e5d3d-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e5d3d-143">Items</span><span class="sxs-lookup"><span data-stu-id="e5d3d-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="e5d3d-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5d3d-144">See also</span></span>



[<span data-ttu-id="e5d3d-145">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="e5d3d-145">CreateItem operation</span></span>](createitem-operation.md)

