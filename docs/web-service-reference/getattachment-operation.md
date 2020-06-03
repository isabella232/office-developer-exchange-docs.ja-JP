---
title: GetAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: GetAttachment 操作は、Exchange ストア内のアイテムの既存の添付ファイルを取得するために使用されます。
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461290"
---
# <a name="getattachment-operation"></a><span data-ttu-id="a2bfd-103">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="a2bfd-103">GetAttachment operation</span></span>

<span data-ttu-id="a2bfd-104">GetAttachment 操作は、Exchange ストア内のアイテムの既存の添付ファイルを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="a2bfd-105">GetAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="a2bfd-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="a2bfd-106">Description</span><span class="sxs-lookup"><span data-stu-id="a2bfd-106">Description</span></span>

<span data-ttu-id="a2bfd-107">次の GetAttachment 要求の例は、添付ファイルを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="a2bfd-108">コード</span><span class="sxs-lookup"><span data-stu-id="a2bfd-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a2bfd-109">コメント</span><span class="sxs-lookup"><span data-stu-id="a2bfd-109">Comments</span></span>

<span data-ttu-id="a2bfd-110">[Attachmentshape](attachmentshape.md)要素を使用すると、どの添付ファイル情報を返すかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="a2bfd-111">空の[Attachmentshape](attachmentshape.md)要素は有効であり、アイテムの添付ファイルの MIME コンテンツのない添付ファイル、テキストの本文の種類、および追加のプロパティを持たない添付ファイルをレンダリングします。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="a2bfd-112">[AttachmentIds](attachmentids.md)コレクションを使用すると、返される1つ以上の添付ファイル識別子を指定できます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="a2bfd-113">これらの型は RequestAttachmentIdType であることに注意してください。 **createattachment**から受け取る AttachmentIds は、 **RootItemId**属性と**RootItemChangeKey**属性を削除してから、 **getattachment**に渡す必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a2bfd-114">読みやすくするために、添付ファイル識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a2bfd-115">Request 要素</span><span class="sxs-lookup"><span data-stu-id="a2bfd-115">Request elements</span></span>

<span data-ttu-id="a2bfd-116">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a2bfd-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="a2bfd-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="a2bfd-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="a2bfd-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="a2bfd-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="a2bfd-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="a2bfd-120">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="a2bfd-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="a2bfd-121">GetAttachment 応答の例</span><span class="sxs-lookup"><span data-stu-id="a2bfd-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="a2bfd-122">Description</span><span class="sxs-lookup"><span data-stu-id="a2bfd-122">Description</span></span>

<span data-ttu-id="a2bfd-123">次の例は、GetAttachment 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="a2bfd-124">次の使用例は、添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="a2bfd-125">コード</span><span class="sxs-lookup"><span data-stu-id="a2bfd-125">Code</span></span>

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
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a2bfd-126">コメント</span><span class="sxs-lookup"><span data-stu-id="a2bfd-126">Comments</span></span>

<span data-ttu-id="a2bfd-127">GetAttachment の応答メッセージには常に、完全な添付ファイルが含まれます。つまり、すべてのプロパティが常に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="a2bfd-128">添付ファイルの場合、これらのプロパティは[Name (AttachmentType)](name-attachmenttype.md)、 [ContentType](contenttype.md)、 [ContentId](contentid.md)、 [contentlocation](contentlocation.md)、および[Content](content.md)です。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="a2bfd-129">アイテムの添付ファイルの場合、これらのプロパティは、GetItem 呼び出しで**allproperties**図形が使用されている場合と同様に、 [Name (attachmenttype)](name-attachmenttype.md)、 [ContentType](contenttype.md)、 [ContentId](contentid.md)、 [contentlocation](contentlocation.md) 、およびすべてのアイテムのプロパティに該当します。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="a2bfd-130">[Attachmentshape](attachmentshape.md)要素が存在する場合、コンシューマーアプリケーションは、アイテムの添付ファイルに追加の拡張プロパティを要求できます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="a2bfd-131">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="a2bfd-131">Successful response elements</span></span>

<span data-ttu-id="a2bfd-132">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2bfd-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a2bfd-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a2bfd-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a2bfd-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="a2bfd-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="a2bfd-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2bfd-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a2bfd-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2bfd-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="a2bfd-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a2bfd-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a2bfd-138">Attachments</span><span class="sxs-lookup"><span data-stu-id="a2bfd-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a2bfd-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="a2bfd-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="a2bfd-140">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="a2bfd-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="a2bfd-141">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="a2bfd-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="a2bfd-142">Content</span><span class="sxs-lookup"><span data-stu-id="a2bfd-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="a2bfd-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2bfd-143">See also</span></span>



[<span data-ttu-id="a2bfd-144">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="a2bfd-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="a2bfd-145">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="a2bfd-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

