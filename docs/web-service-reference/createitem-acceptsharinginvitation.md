---
title: Createitem メソッド (AcceptSharingInvitation)
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
description: CreateItem 操作を使用して、別のユーザーの予定表や連絡先のデータを共有するための招待を承諾します。
ms.openlocfilehash: 993ef0402e624af69f632af5bdce4c02bd9d41f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759828"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="b34ac-103">Createitem メソッド (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="b34ac-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="b34ac-104">**CreateItem**操作を使用して、別のユーザーの予定表や連絡先のデータを共有するための招待を承諾します。</span><span class="sxs-lookup"><span data-stu-id="b34ac-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="b34ac-105">要求の例を共有への招待を受け入れる</span><span class="sxs-lookup"><span data-stu-id="b34ac-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="b34ac-106">説明</span><span class="sxs-lookup"><span data-stu-id="b34ac-106">Description</span></span>

<span data-ttu-id="b34ac-107">次の例では、共有への招待を承諾する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b34ac-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="b34ac-108">コード</span><span class="sxs-lookup"><span data-stu-id="b34ac-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="b34ac-109">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="b34ac-109">Request elements</span></span>

<span data-ttu-id="b34ac-110">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b34ac-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b34ac-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="b34ac-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="b34ac-112">Items</span><span class="sxs-lookup"><span data-stu-id="b34ac-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="b34ac-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="b34ac-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="b34ac-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="b34ac-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="b34ac-115">コメント</span><span class="sxs-lookup"><span data-stu-id="b34ac-115">Comments</span></span>

<span data-ttu-id="b34ac-116">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b34ac-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="b34ac-117">成功の共有への招待の承諾の応答の例</span><span class="sxs-lookup"><span data-stu-id="b34ac-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="b34ac-118">説明</span><span class="sxs-lookup"><span data-stu-id="b34ac-118">Description</span></span>

<span data-ttu-id="b34ac-119">次の使用例は、 **CreateItem**要求に正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="b34ac-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b34ac-120">コード</span><span class="sxs-lookup"><span data-stu-id="b34ac-120">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="b34ac-121">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="b34ac-121">Successful response elements</span></span>

<span data-ttu-id="b34ac-122">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b34ac-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b34ac-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b34ac-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b34ac-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="b34ac-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="b34ac-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b34ac-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b34ac-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b34ac-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="b34ac-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b34ac-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b34ac-128">Items</span><span class="sxs-lookup"><span data-stu-id="b34ac-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="b34ac-129">共有への招待のエラー応答の例をそのまま使用します。</span><span class="sxs-lookup"><span data-stu-id="b34ac-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b34ac-130">説明</span><span class="sxs-lookup"><span data-stu-id="b34ac-130">Description</span></span>

<span data-ttu-id="b34ac-131">次の使用例は、 **CreateItem**要求に対してエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="b34ac-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="b34ac-132">見つからない共有への招待を受け入れるようにしようとしてエラーの原因が Exchange ストアにします。</span><span class="sxs-lookup"><span data-stu-id="b34ac-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b34ac-133">コード</span><span class="sxs-lookup"><span data-stu-id="b34ac-133">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="b34ac-134">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="b34ac-134">Error response elements</span></span>

<span data-ttu-id="b34ac-135">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b34ac-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b34ac-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b34ac-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b34ac-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="b34ac-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="b34ac-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b34ac-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b34ac-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b34ac-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="b34ac-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="b34ac-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b34ac-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b34ac-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b34ac-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b34ac-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b34ac-143">Items</span><span class="sxs-lookup"><span data-stu-id="b34ac-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="b34ac-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="b34ac-144">See also</span></span>



<span data-ttu-id="b34ac-145">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="b34ac-145">[CreateItem operation](createitem-operation.md)</span></span>

