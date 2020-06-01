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
description: DeleteAttachment 操作は、Exchange ストア内の既存のアイテムからファイルおよびアイテムの添付ファイルを削除するために使用されます。
ms.openlocfilehash: 1d34ce4c5ba1d955989a35dafb8ab3c5d229d505
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457334"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="e5e9a-103">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="e5e9a-103">DeleteAttachment operation</span></span>

<span data-ttu-id="e5e9a-104">DeleteAttachment 操作は、Exchange ストア内の既存のアイテムからファイルおよびアイテムの添付ファイルを削除するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5e9a-105">注釈</span><span class="sxs-lookup"><span data-stu-id="e5e9a-105">Remarks</span></span>

<span data-ttu-id="e5e9a-106">この操作により、ID で1つ以上の添付ファイルを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="e5e9a-107">DeleteAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="e5e9a-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="e5e9a-108">説明</span><span class="sxs-lookup"><span data-stu-id="e5e9a-108">Description</span></span>

<span data-ttu-id="e5e9a-109">次の DeleteAttachment 要求の例は、アイテムの添付ファイルを削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="e5e9a-110">コード</span><span class="sxs-lookup"><span data-stu-id="e5e9a-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e5e9a-111">コメント</span><span class="sxs-lookup"><span data-stu-id="e5e9a-111">Comments</span></span>

<span data-ttu-id="e5e9a-112">添付ファイル識別子は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="e5e9a-113">Request 要素</span><span class="sxs-lookup"><span data-stu-id="e5e9a-113">Request elements</span></span>

<span data-ttu-id="e5e9a-114">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e5e9a-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="e5e9a-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="e5e9a-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="e5e9a-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="e5e9a-117">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="e5e9a-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="e5e9a-118">DeleteAttachment 応答の例</span><span class="sxs-lookup"><span data-stu-id="e5e9a-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="e5e9a-119">説明</span><span class="sxs-lookup"><span data-stu-id="e5e9a-119">Description</span></span>

<span data-ttu-id="e5e9a-120">次の例は、DeleteAttachment 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e5e9a-121">コード</span><span class="sxs-lookup"><span data-stu-id="e5e9a-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="e5e9a-122">コメント</span><span class="sxs-lookup"><span data-stu-id="e5e9a-122">Comments</span></span>

<span data-ttu-id="e5e9a-123">CreateAttachment 操作は、 **RootItemId**と**RootItemChangeKey**を含む AttachmentIdType type の要素を返します。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="e5e9a-124">これらの属性は、DeleteAttachment 要求内の識別子には許可されていません。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="e5e9a-125">DeleteAttachment は、RequestAttachmentIdType 型の要素を使用します。これらの属性は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="e5e9a-126">DeleteAttachment 応答には、親アイテムの ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="e5e9a-127">アイテムから添付ファイルが削除されると、アイテムの変更キーが変更されます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="e5e9a-128">新しいアイテム変更キーは、DeleteAttachment 応答から取得できます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e5e9a-129">読みやすくするために、 [RootItemId](rootitemid.md) Identifier および changekey が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="e5e9a-130">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="e5e9a-130">Successful response elements</span></span>

<span data-ttu-id="e5e9a-131">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="e5e9a-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e5e9a-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e5e9a-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e5e9a-133">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="e5e9a-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="e5e9a-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e5e9a-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e5e9a-135">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e5e9a-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="e5e9a-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e5e9a-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e5e9a-137">RootItemId</span><span class="sxs-lookup"><span data-stu-id="e5e9a-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="e5e9a-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5e9a-138">See also</span></span>

- [<span data-ttu-id="e5e9a-139">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="e5e9a-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="e5e9a-140">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="e5e9a-140">GetAttachment operation</span></span>](getattachment-operation.md)

