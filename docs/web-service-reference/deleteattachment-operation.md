---
title: DeleteAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: DeleteAttachment 操作を使用して、Exchange ストア内の既存の項目からファイルおよびアイテムの添付ファイルを削除します。
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759964"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="1c033-103">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="1c033-103">DeleteAttachment operation</span></span>

<span data-ttu-id="1c033-104">DeleteAttachment 操作を使用して、Exchange ストア内の既存の項目からファイルおよびアイテムの添付ファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="1c033-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1c033-105">備考</span><span class="sxs-lookup"><span data-stu-id="1c033-105">Remarks</span></span>

<span data-ttu-id="1c033-106">この操作では、ID で 1 つまたは複数の添付ファイルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="1c033-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="1c033-107">DeleteAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="1c033-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="1c033-108">説明</span><span class="sxs-lookup"><span data-stu-id="1c033-108">Description</span></span>

<span data-ttu-id="1c033-109">DeleteAttachment 要求の次の例では、アイテムの添付ファイルを削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1c033-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c033-110">コード</span><span class="sxs-lookup"><span data-stu-id="1c033-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="1c033-111">コメント</span><span class="sxs-lookup"><span data-stu-id="1c033-111">Comments</span></span>

<span data-ttu-id="1c033-112">添付ファイル識別子が読みやすさを保持するために小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="1c033-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="1c033-113">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="1c033-113">Request elements</span></span>

<span data-ttu-id="1c033-114">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1c033-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="1c033-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1c033-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="1c033-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="1c033-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="1c033-117">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="1c033-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="1c033-118">DeleteAttachment 応答の例</span><span class="sxs-lookup"><span data-stu-id="1c033-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="1c033-119">説明</span><span class="sxs-lookup"><span data-stu-id="1c033-119">Description</span></span>

<span data-ttu-id="1c033-120">DeleteAttachment 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c033-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c033-121">コード</span><span class="sxs-lookup"><span data-stu-id="1c033-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="1c033-122">コメント</span><span class="sxs-lookup"><span data-stu-id="1c033-122">Comments</span></span>

<span data-ttu-id="1c033-123">CreateAttachment 操作では、 **RootItemId**と**RootItemChangeKey**を含む AttachmentIdType 型の要素を返します。</span><span class="sxs-lookup"><span data-stu-id="1c033-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="1c033-124">DeleteAttachment 要求内の識別子には、これらの属性は許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1c033-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="1c033-125">DeleteAttachment は、これらの属性が含まれていない RequestAttachmentIdType の種類の要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="1c033-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="1c033-126">DeleteAttachment の応答には、親項目の ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c033-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="1c033-127">アイテムから添付ファイルが削除されると、アイテムの変更キーが変更されます。</span><span class="sxs-lookup"><span data-stu-id="1c033-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="1c033-128">DeleteAttachment の応答から、新しいアイテムの変更キーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="1c033-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1c033-129">[RootItemId](rootitemid.md)の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="1c033-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="1c033-130">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="1c033-130">Successful response elements</span></span>

<span data-ttu-id="1c033-131">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1c033-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="1c033-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1c033-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="1c033-133">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="1c033-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="1c033-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1c033-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="1c033-135">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1c033-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="1c033-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1c033-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1c033-137">RootItemId</span><span class="sxs-lookup"><span data-stu-id="1c033-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="1c033-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c033-138">See also</span></span>

- [<span data-ttu-id="1c033-139">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="1c033-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="1c033-140">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="1c033-140">GetAttachment operation</span></span>](getattachment-operation.md)

