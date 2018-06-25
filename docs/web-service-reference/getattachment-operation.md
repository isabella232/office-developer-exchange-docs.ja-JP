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
description: GetAttachment 操作を使用して、Exchange ストア内の項目に既存の添付ファイルを取得します。
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760643"
---
# <a name="getattachment-operation"></a><span data-ttu-id="7ec18-103">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="7ec18-103">GetAttachment operation</span></span>

<span data-ttu-id="7ec18-104">GetAttachment 操作を使用して、Exchange ストア内の項目に既存の添付ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="7ec18-105">GetAttachment 要求の例</span><span class="sxs-lookup"><span data-stu-id="7ec18-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="7ec18-106">説明</span><span class="sxs-lookup"><span data-stu-id="7ec18-106">Description</span></span>

<span data-ttu-id="7ec18-107">GetAttachment 要求の次の使用例は、添付ファイルを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7ec18-108">コード</span><span class="sxs-lookup"><span data-stu-id="7ec18-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="7ec18-109">コメント</span><span class="sxs-lookup"><span data-stu-id="7ec18-109">Comments</span></span>

<span data-ttu-id="7ec18-110">[AttachmentShape](attachmentshape.md)要素を使用する添付ファイルの情報が返される必要がありますを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="7ec18-111">空の[AttachmentShape](attachmentshape.md)要素は有効であり、テキスト本文の種類、し、追加のプロパティを使用しない項目の添付ファイルの MIME コンテンツのない添付ファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="7ec18-112">[AttachmentIds](attachmentids.md)コレクションを取得する 1 つまたは複数の添付ファイルの識別子を指定できます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="7ec18-113">**GetAttachment**に渡す前に RequestAttachmentIdType、 **CreateAttachment**から受信するすべての AttachmentIds、 **RootItemId**および**RootItemChangeKey**属性が必要であるためにの削除の種類は、これらに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7ec18-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7ec18-114">添付ファイルの識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="7ec18-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7ec18-115">要素を要求します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-115">Request elements</span></span>

<span data-ttu-id="7ec18-116">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7ec18-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7ec18-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="7ec18-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="7ec18-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="7ec18-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="7ec18-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="7ec18-120">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="7ec18-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="7ec18-121">GetAttachment 応答の例</span><span class="sxs-lookup"><span data-stu-id="7ec18-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="7ec18-122">説明</span><span class="sxs-lookup"><span data-stu-id="7ec18-122">Description</span></span>

<span data-ttu-id="7ec18-123">GetAttachment 要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="7ec18-124">この例では、添付ファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="7ec18-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7ec18-125">コード</span><span class="sxs-lookup"><span data-stu-id="7ec18-125">Code</span></span>

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
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="7ec18-126">コメント</span><span class="sxs-lookup"><span data-stu-id="7ec18-126">Comments</span></span>

<span data-ttu-id="7ec18-127">GetAttachment の応答メッセージは常に、すべて添付ファイルを含みます。すべてのプロパティ常に含まれます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="7ec18-128">ファイルの添付ファイルのこれらのプロパティは、[名前 (AttachmentType)](name-attachmenttype.md)、[コンテンツ タイプ](contenttype.md)、 [ContentId](contentid.md)、 [ContentLocation](contentlocation.md)、および[コンテンツ](content.md)です。</span><span class="sxs-lookup"><span data-stu-id="7ec18-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="7ec18-129">項目の添付ファイルのこれらのプロパティは[(AttachmentType) の名前](name-attachmenttype.md)、[コンテンツ タイプ](contenttype.md)、 [ContentId](contentid.md)、 [ContentLocation](contentlocation.md)すべてのアイテムのプロパティでは、 **AllProperties**の図形が使われていた場合と同様、GetItem の呼び出しで。</span><span class="sxs-lookup"><span data-stu-id="7ec18-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="7ec18-130">[AttachmentShape](attachmentshape.md)要素では、存在する場合、項目の添付ファイルの拡張プロパティの追加を要求するコンシューマー アプリケーションできます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="7ec18-131">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="7ec18-131">Successful response elements</span></span>

<span data-ttu-id="7ec18-132">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="7ec18-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7ec18-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7ec18-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7ec18-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="7ec18-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="7ec18-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7ec18-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7ec18-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ec18-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="7ec18-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ec18-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7ec18-138">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="7ec18-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7ec18-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="7ec18-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="7ec18-140">AttachmentId (GetAttachment と DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="7ec18-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="7ec18-141">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="7ec18-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="7ec18-142">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="7ec18-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="7ec18-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ec18-143">See also</span></span>



[<span data-ttu-id="7ec18-144">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="7ec18-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="7ec18-145">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="7ec18-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

