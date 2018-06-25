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
description: CreateAttachment 操作では、アイテムまたはファイルのいずれかの添付ファイルを作成し、指定された項目に結び付けます。
ms.openlocfilehash: fed60275a007f2796c60d936def7a937e4982f29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759797"
---
# <a name="createattachment-operation"></a><span data-ttu-id="b001a-103">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b001a-103">CreateAttachment operation</span></span>

<span data-ttu-id="b001a-104">CreateAttachment 操作では、アイテムまたはファイルのいずれかの添付ファイルを作成し、指定された項目に結び付けます。</span><span class="sxs-lookup"><span data-stu-id="b001a-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="b001a-105">CreateAttachment 要求のファイルの例</span><span class="sxs-lookup"><span data-stu-id="b001a-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="b001a-106">説明</span><span class="sxs-lookup"><span data-stu-id="b001a-106">Description</span></span>

<span data-ttu-id="b001a-107">CreateAttachment 要求の次の使用例は、添付ファイルを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b001a-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="b001a-108">コード</span><span class="sxs-lookup"><span data-stu-id="b001a-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="b001a-109">Comment</span><span class="sxs-lookup"><span data-stu-id="b001a-109">Comment</span></span>

<span data-ttu-id="b001a-110">添付ファイルの名前を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b001a-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="b001a-111">親項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b001a-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b001a-112">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="b001a-112">Request elements</span></span>

<span data-ttu-id="b001a-113">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b001a-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b001a-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="b001a-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="b001a-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="b001a-116">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b001a-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b001a-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="b001a-118">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b001a-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="b001a-119">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="b001a-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="b001a-120">ファイル CreateAttachment 応答の成功の例</span><span class="sxs-lookup"><span data-stu-id="b001a-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="b001a-121">説明</span><span class="sxs-lookup"><span data-stu-id="b001a-121">Description</span></span>

<span data-ttu-id="b001a-122">CreateAttachment 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b001a-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b001a-123">コード</span><span class="sxs-lookup"><span data-stu-id="b001a-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="b001a-124">Comment</span><span class="sxs-lookup"><span data-stu-id="b001a-124">Comment</span></span>

<span data-ttu-id="b001a-125">応答には、添付ファイルの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b001a-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="b001a-126">ルート アイテムの識別子と変更キーも含まれています。</span><span class="sxs-lookup"><span data-stu-id="b001a-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="b001a-127">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b001a-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="b001a-128">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="b001a-128">Successful response elements</span></span>

<span data-ttu-id="b001a-129">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b001a-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b001a-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b001a-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b001a-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b001a-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b001a-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b001a-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b001a-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b001a-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b001a-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b001a-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b001a-135">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b001a-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b001a-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="b001a-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="b001a-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="b001a-138">アイテム CreateAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="b001a-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="b001a-139">説明</span><span class="sxs-lookup"><span data-stu-id="b001a-139">Description</span></span>

<span data-ttu-id="b001a-140">CreateAttachment 要求の次の例では、アイテムの添付ファイルを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b001a-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="b001a-141">コード</span><span class="sxs-lookup"><span data-stu-id="b001a-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="b001a-142">Comment</span><span class="sxs-lookup"><span data-stu-id="b001a-142">Comment</span></span>

<span data-ttu-id="b001a-143">添付ファイルの名前を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b001a-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="b001a-144">**メモ**親項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b001a-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b001a-145">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="b001a-145">Request elements</span></span>

<span data-ttu-id="b001a-146">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b001a-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b001a-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="b001a-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="b001a-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="b001a-149">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b001a-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b001a-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="b001a-151">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b001a-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="b001a-152">Message</span><span class="sxs-lookup"><span data-stu-id="b001a-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b001a-153">Subject</span><span class="sxs-lookup"><span data-stu-id="b001a-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="b001a-154">成功アイテム CreateAttachment 応答の例</span><span class="sxs-lookup"><span data-stu-id="b001a-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="b001a-155">説明</span><span class="sxs-lookup"><span data-stu-id="b001a-155">Description</span></span>

<span data-ttu-id="b001a-156">CreateAttachment 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b001a-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b001a-157">コード</span><span class="sxs-lookup"><span data-stu-id="b001a-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="b001a-158">Comment</span><span class="sxs-lookup"><span data-stu-id="b001a-158">Comment</span></span>

<span data-ttu-id="b001a-159">応答には、新しい添付ファイルの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b001a-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="b001a-160">ルート アイテムの識別子と変更キーも含まれています。</span><span class="sxs-lookup"><span data-stu-id="b001a-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="b001a-161">ルート アイテムは、添付ファイルが含まれているアイテムです。</span><span class="sxs-lookup"><span data-stu-id="b001a-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="b001a-162">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b001a-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="b001a-163">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="b001a-163">Successful response elements</span></span>

<span data-ttu-id="b001a-164">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b001a-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b001a-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b001a-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b001a-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b001a-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b001a-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b001a-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b001a-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b001a-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b001a-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b001a-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b001a-170">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b001a-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b001a-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b001a-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="b001a-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="b001a-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="b001a-173">CreateAttachment エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="b001a-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b001a-174">説明</span><span class="sxs-lookup"><span data-stu-id="b001a-174">Description</span></span>

<span data-ttu-id="b001a-175">CreateAttachment 要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b001a-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="b001a-176">エラーは、添付ファイルの名前が指定されていないことが原因です。</span><span class="sxs-lookup"><span data-stu-id="b001a-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="b001a-177">コード</span><span class="sxs-lookup"><span data-stu-id="b001a-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="b001a-178">エラー応答の要素</span><span class="sxs-lookup"><span data-stu-id="b001a-178">Error response elements</span></span>

<span data-ttu-id="b001a-179">エラー応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="b001a-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b001a-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b001a-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b001a-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b001a-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="b001a-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b001a-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b001a-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b001a-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="b001a-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="b001a-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b001a-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b001a-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b001a-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b001a-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b001a-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b001a-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="b001a-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="b001a-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="b001a-189">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="b001a-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="b001a-190">備考</span><span class="sxs-lookup"><span data-stu-id="b001a-190">Remarks</span></span>

<span data-ttu-id="b001a-191">複数の添付ファイルは、単一のラウンド トリップ内のアイテムに関連付けられている、最後の応答メッセージの RootItemChangeKey が、添付ファイルのあるアイテムの新しい変更キーを表す 1 つ。</span><span class="sxs-lookup"><span data-stu-id="b001a-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b001a-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="b001a-192">See also</span></span>



[<span data-ttu-id="b001a-193">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b001a-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="b001a-194">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="b001a-194">GetAttachment operation</span></span>](getattachment-operation.md)

