---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: FileAttachment 要素は、Exchange ストア内のアイテムに添付されているファイルを表します。
ms.openlocfilehash: db9b541fb2527ae3c09cbdb33bedea7fb215bd30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461017"
---
# <a name="fileattachment"></a><span data-ttu-id="d2b90-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d2b90-103">FileAttachment</span></span>

<span data-ttu-id="d2b90-104">**Fileattachment**要素は、Exchange ストア内のアイテムに添付されているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 <span data-ttu-id="d2b90-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="d2b90-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2b90-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2b90-106">Attributes and elements</span></span>

<span data-ttu-id="d2b90-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2b90-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2b90-108">Attributes</span></span>

<span data-ttu-id="d2b90-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2b90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2b90-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2b90-110">Child elements</span></span>

|<span data-ttu-id="d2b90-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d2b90-111">**Element**</span></span>|<span data-ttu-id="d2b90-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2b90-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2b90-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="d2b90-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="d2b90-114">添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-115">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="d2b90-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="d2b90-116">添付ファイルの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="d2b90-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="d2b90-118">添付ファイルのコンテンツのマルチパーパスインターネットメール内線 (MIME) の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="d2b90-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="d2b90-120">添付ファイルのコンテンツの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="d2b90-121">[ContentId](contentid.md)は、任意の文字列値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="d2b90-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="d2b90-122">アプリケーションでは、 [ContentId](contentid.md)を使用して独自の識別メカニズムを実装できます。</span><span class="sxs-lookup"><span data-stu-id="d2b90-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="d2b90-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="d2b90-124">添付ファイルのコンテンツの場所に対応する Uniform Resource Identifier (URI) を含みます。</span><span class="sxs-lookup"><span data-stu-id="d2b90-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|<span data-ttu-id="d2b90-125">[[サイズ]](size.md)</span><span class="sxs-lookup"><span data-stu-id="d2b90-125">[Size](size.md)</span></span> <br/> |<span data-ttu-id="d2b90-126">添付ファイルのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="d2b90-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="d2b90-128">添付ファイルが最後に変更された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="d2b90-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="d2b90-130">添付ファイルがアイテム内にインラインで表示されるかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="d2b90-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="d2b90-132">添付ファイルが連絡先の画像であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="d2b90-133">Content</span><span class="sxs-lookup"><span data-stu-id="d2b90-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="d2b90-134">添付ファイルの Base64 でエンコードされたコンテンツを格納します。</span><span class="sxs-lookup"><span data-stu-id="d2b90-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2b90-135">親要素</span><span class="sxs-lookup"><span data-stu-id="d2b90-135">Parent elements</span></span>

|<span data-ttu-id="d2b90-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2b90-136">**Element**</span></span>|<span data-ttu-id="d2b90-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2b90-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2b90-138">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="d2b90-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d2b90-139">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="d2b90-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2b90-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d2b90-140">Text value</span></span>

<span data-ttu-id="d2b90-141">なし。</span><span class="sxs-lookup"><span data-stu-id="d2b90-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2b90-142">注釈</span><span class="sxs-lookup"><span data-stu-id="d2b90-142">Remarks</span></span>

<span data-ttu-id="d2b90-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d2b90-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2b90-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2b90-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2b90-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2b90-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2b90-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2b90-146">Schema name</span></span>  <br/> |<span data-ttu-id="d2b90-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d2b90-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2b90-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2b90-148">Validation file</span></span>  <br/> |<span data-ttu-id="d2b90-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d2b90-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2b90-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2b90-150">Can be empty</span></span>  <br/> |<span data-ttu-id="d2b90-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="d2b90-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2b90-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2b90-152">See also</span></span>



- [<span data-ttu-id="d2b90-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2b90-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

