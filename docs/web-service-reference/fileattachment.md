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
description: FileAttachment 要素は、Exchange ストア内のアイテムに関連付けられているファイルを表します。
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760484"
---
# <a name="fileattachment"></a><span data-ttu-id="661fd-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="661fd-103">FileAttachment</span></span>

<span data-ttu-id="661fd-104">**FileAttachment**要素は、Exchange ストア内のアイテムに関連付けられているファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="661fd-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="661fd-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="661fd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="661fd-106">Attributes and elements</span></span>

<span data-ttu-id="661fd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="661fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="661fd-108">属性</span><span class="sxs-lookup"><span data-stu-id="661fd-108">Attributes</span></span>

<span data-ttu-id="661fd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="661fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="661fd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="661fd-110">Child elements</span></span>

|<span data-ttu-id="661fd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="661fd-111">**Element**</span></span>|<span data-ttu-id="661fd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="661fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="661fd-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="661fd-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="661fd-114">添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="661fd-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="661fd-115">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="661fd-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="661fd-116">添付ファイルの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="661fd-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="661fd-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="661fd-118">添付ファイルのコンテンツの多目的インターネット メール拡張 (MIME) の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="661fd-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="661fd-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="661fd-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="661fd-120">添付ファイルの内容の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="661fd-121">[ContentId](contentid.md)は、任意の文字列値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="661fd-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="661fd-122">アプリケーションは、独自の識別メカニズムを実装するために、 [ContentId](contentid.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="661fd-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="661fd-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="661fd-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="661fd-124">統一リソース識別子 (URI) の添付ファイルのコンテンツの場所に対応するが含まれています。</span><span class="sxs-lookup"><span data-stu-id="661fd-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="661fd-125">Size</span><span class="sxs-lookup"><span data-stu-id="661fd-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="661fd-126">添付ファイルのバイト単位でサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="661fd-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="661fd-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="661fd-128">添付ファイルが最後に変更されたときを表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="661fd-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="661fd-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="661fd-130">添付ファイルの項目内でのインラインで表示されているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="661fd-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="661fd-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="661fd-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="661fd-132">添付ファイルが連絡先の写真であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="661fd-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="661fd-133">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="661fd-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="661fd-134">添付ファイルの Base64 でエンコードされた内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="661fd-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="661fd-135">親要素</span><span class="sxs-lookup"><span data-stu-id="661fd-135">Parent elements</span></span>

|<span data-ttu-id="661fd-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="661fd-136">**Element**</span></span>|<span data-ttu-id="661fd-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="661fd-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="661fd-138">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="661fd-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="661fd-139">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="661fd-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="661fd-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="661fd-140">Text value</span></span>

<span data-ttu-id="661fd-141">なし。</span><span class="sxs-lookup"><span data-stu-id="661fd-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="661fd-142">備考</span><span class="sxs-lookup"><span data-stu-id="661fd-142">Remarks</span></span>

<span data-ttu-id="661fd-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="661fd-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="661fd-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="661fd-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="661fd-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="661fd-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="661fd-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="661fd-146">Schema name</span></span>  <br/> |<span data-ttu-id="661fd-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="661fd-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="661fd-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="661fd-148">Validation file</span></span>  <br/> |<span data-ttu-id="661fd-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="661fd-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="661fd-150">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="661fd-150">Can be empty</span></span>  <br/> |<span data-ttu-id="661fd-151">False</span><span class="sxs-lookup"><span data-stu-id="661fd-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="661fd-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="661fd-152">See also</span></span>



- [<span data-ttu-id="661fd-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="661fd-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

