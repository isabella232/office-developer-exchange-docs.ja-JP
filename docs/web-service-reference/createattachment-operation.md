---
title: CreateAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: CreateAttachment 操作は、アイテムまたは添付ファイルのいずれかを作成し、指定されたアイテムに添付します。
ms.openlocfilehash: 8028c56aa306774b54b39e5ee1ac0382b9113fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456571"
---
# <a name="createattachment-operation"></a><span data-ttu-id="98d12-103">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="98d12-103">CreateAttachment operation</span></span>

<span data-ttu-id="98d12-104">CreateAttachment 操作は、アイテムまたは添付ファイルのいずれかを作成し、指定されたアイテムに添付します。</span><span class="sxs-lookup"><span data-stu-id="98d12-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="98d12-105">ファイル CreateAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="98d12-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="98d12-106">説明</span><span class="sxs-lookup"><span data-stu-id="98d12-106">Description</span></span>

<span data-ttu-id="98d12-107">次の CreateAttachment 要求の例は、添付ファイルを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98d12-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="98d12-108">コード</span><span class="sxs-lookup"><span data-stu-id="98d12-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="98d12-109">コメント</span><span class="sxs-lookup"><span data-stu-id="98d12-109">Comment</span></span>

<span data-ttu-id="98d12-110">添付ファイルの名前を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98d12-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="98d12-111">読みやすくするために、親アイテムの識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98d12-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="98d12-112">Request 要素</span><span class="sxs-lookup"><span data-stu-id="98d12-112">Request elements</span></span>

<span data-ttu-id="98d12-113">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d12-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="98d12-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="98d12-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="98d12-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="98d12-116">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="98d12-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="98d12-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="98d12-118">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="98d12-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="98d12-119">Content</span><span class="sxs-lookup"><span data-stu-id="98d12-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="98d12-120">正常なファイル CreateAttachment の応答の例</span><span class="sxs-lookup"><span data-stu-id="98d12-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="98d12-121">説明</span><span class="sxs-lookup"><span data-stu-id="98d12-121">Description</span></span>

<span data-ttu-id="98d12-122">次の例は、CreateAttachment 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="98d12-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="98d12-123">コード</span><span class="sxs-lookup"><span data-stu-id="98d12-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="98d12-124">コメント</span><span class="sxs-lookup"><span data-stu-id="98d12-124">Comment</span></span>

<span data-ttu-id="98d12-125">応答には、添付ファイルの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="98d12-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="98d12-126">また、ルートアイテムの識別子と変更キーも含みます。</span><span class="sxs-lookup"><span data-stu-id="98d12-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="98d12-127">読みやすくするために、アイテムの識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98d12-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="98d12-128">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="98d12-128">Successful response elements</span></span>

<span data-ttu-id="98d12-129">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d12-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="98d12-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="98d12-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="98d12-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="98d12-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="98d12-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="98d12-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="98d12-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98d12-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="98d12-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="98d12-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="98d12-135">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="98d12-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="98d12-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="98d12-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="98d12-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="98d12-138">アイテム CreateAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="98d12-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="98d12-139">説明</span><span class="sxs-lookup"><span data-stu-id="98d12-139">Description</span></span>

<span data-ttu-id="98d12-140">次の CreateAttachment 要求の例は、アイテムの添付ファイルを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="98d12-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="98d12-141">コード</span><span class="sxs-lookup"><span data-stu-id="98d12-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="98d12-142">コメント</span><span class="sxs-lookup"><span data-stu-id="98d12-142">Comment</span></span>

<span data-ttu-id="98d12-143">添付ファイルの名前を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98d12-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="98d12-144">**メモ**読みやすくするために、親アイテムの識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98d12-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="98d12-145">Request 要素</span><span class="sxs-lookup"><span data-stu-id="98d12-145">Request elements</span></span>

<span data-ttu-id="98d12-146">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d12-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="98d12-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="98d12-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="98d12-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="98d12-149">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="98d12-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="98d12-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="98d12-151">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="98d12-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="98d12-152">Message</span><span class="sxs-lookup"><span data-stu-id="98d12-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- <span data-ttu-id="98d12-153">[[件名]](subject.md)</span><span class="sxs-lookup"><span data-stu-id="98d12-153">[Subject](subject.md)</span></span>
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="98d12-154">正常なアイテム CreateAttachment の応答の例</span><span class="sxs-lookup"><span data-stu-id="98d12-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="98d12-155">説明</span><span class="sxs-lookup"><span data-stu-id="98d12-155">Description</span></span>

<span data-ttu-id="98d12-156">次の例は、CreateAttachment 要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="98d12-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="98d12-157">コード</span><span class="sxs-lookup"><span data-stu-id="98d12-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="98d12-158">コメント</span><span class="sxs-lookup"><span data-stu-id="98d12-158">Comment</span></span>

<span data-ttu-id="98d12-159">応答には、新しい添付ファイルの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="98d12-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="98d12-160">また、ルートアイテムの識別子と変更キーも含みます。</span><span class="sxs-lookup"><span data-stu-id="98d12-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="98d12-161">ルートアイテムは、添付ファイルを含むアイテムです。</span><span class="sxs-lookup"><span data-stu-id="98d12-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="98d12-162">読みやすくするために、アイテムの識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="98d12-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="98d12-163">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="98d12-163">Successful response elements</span></span>

<span data-ttu-id="98d12-164">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d12-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="98d12-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="98d12-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="98d12-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="98d12-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="98d12-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="98d12-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="98d12-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98d12-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="98d12-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="98d12-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="98d12-170">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="98d12-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="98d12-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="98d12-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="98d12-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="98d12-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="98d12-173">CreateAttachment エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="98d12-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="98d12-174">説明</span><span class="sxs-lookup"><span data-stu-id="98d12-174">Description</span></span>

<span data-ttu-id="98d12-175">次の例は、CreateAttachment 要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="98d12-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="98d12-176">このエラーは、添付ファイルの名前が指定されていないことが原因で発生します。</span><span class="sxs-lookup"><span data-stu-id="98d12-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="98d12-177">コード</span><span class="sxs-lookup"><span data-stu-id="98d12-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="98d12-178">エラー応答要素</span><span class="sxs-lookup"><span data-stu-id="98d12-178">Error response elements</span></span>

<span data-ttu-id="98d12-179">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="98d12-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="98d12-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="98d12-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="98d12-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="98d12-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="98d12-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="98d12-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="98d12-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98d12-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="98d12-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="98d12-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="98d12-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="98d12-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="98d12-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="98d12-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="98d12-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="98d12-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="98d12-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="98d12-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="98d12-189">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="98d12-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="98d12-190">注釈</span><span class="sxs-lookup"><span data-stu-id="98d12-190">Remarks</span></span>

<span data-ttu-id="98d12-191">1回のラウンドトリップで複数の添付ファイルがアイテムに添付されている場合、最後の応答メッセージの RootItemChangeKey は、添付ファイルを持つアイテムの新しい変更キーを表すものです。</span><span class="sxs-lookup"><span data-stu-id="98d12-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="98d12-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="98d12-192">See also</span></span>



[<span data-ttu-id="98d12-193">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="98d12-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="98d12-194">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="98d12-194">GetAttachment operation</span></span>](getattachment-operation.md)

