---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: ItemAttachment 要素は、別の Exchange アイテムに関連付けられている Exchange アイテムを表します。
ms.openlocfilehash: c3a07fa091c05654a03cbff58fb20204c26c9061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526439"
---
# <a name="itemattachment"></a><span data-ttu-id="2aeff-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="2aeff-103">ItemAttachment</span></span>

<span data-ttu-id="2aeff-104">**Itemattachment**要素は、別の exchange アイテムに関連付けられている exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Message/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <CalendarItem/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Contact/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Task/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingMessage/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingRequest/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingResponse/>
</ItemAttachment>
```

```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <MeetingCancellation/>
</ItemAttachment>
```

<span data-ttu-id="2aeff-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="2aeff-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2aeff-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2aeff-106">Attributes and elements</span></span>

<span data-ttu-id="2aeff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2aeff-108">属性</span><span class="sxs-lookup"><span data-stu-id="2aeff-108">Attributes</span></span>

<span data-ttu-id="2aeff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2aeff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2aeff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2aeff-110">Child elements</span></span>

|<span data-ttu-id="2aeff-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2aeff-111">**Element**</span></span>|<span data-ttu-id="2aeff-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2aeff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2aeff-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="2aeff-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="2aeff-114">添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-115">Name (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="2aeff-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="2aeff-116">添付ファイルの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="2aeff-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="2aeff-118">添付ファイルのコンテンツのマルチパーパスインターネットメール内線 (MIME) の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="2aeff-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="2aeff-120">添付ファイルのコンテンツの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="2aeff-121">[ContentId](contentid.md)は、任意の文字列値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="2aeff-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="2aeff-122">アプリケーションでは、 [ContentId](contentid.md)を使用して独自の識別メカニズムを実装できます。</span><span class="sxs-lookup"><span data-stu-id="2aeff-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="2aeff-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="2aeff-124">添付ファイルのコンテンツの場所に対応する Uniform Resource Identifier (URI) を含みます。</span><span class="sxs-lookup"><span data-stu-id="2aeff-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-125">Size</span><span class="sxs-lookup"><span data-stu-id="2aeff-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="2aeff-126">添付ファイルのサイズ (バイト単位) を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2aeff-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="2aeff-128">添付ファイルが最後に変更された日時を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="2aeff-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="2aeff-130">添付ファイルがアイテム内にインラインで表示されるかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-131">Item</span><span class="sxs-lookup"><span data-stu-id="2aeff-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="2aeff-132">一般的な Exchange アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-133">Message</span><span class="sxs-lookup"><span data-stu-id="2aeff-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2aeff-134">Exchange 電子メールメッセージの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2aeff-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2aeff-136">Exchange 予定表アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-137">Contact</span><span class="sxs-lookup"><span data-stu-id="2aeff-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="2aeff-138">Exchange の連絡先アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-139">タスク</span><span class="sxs-lookup"><span data-stu-id="2aeff-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="2aeff-140">Exchange タスクの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="2aeff-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="2aeff-142">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2aeff-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2aeff-144">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="2aeff-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="2aeff-146">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2aeff-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="2aeff-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="2aeff-148">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="2aeff-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2aeff-149">親要素</span><span class="sxs-lookup"><span data-stu-id="2aeff-149">Parent elements</span></span>

|<span data-ttu-id="2aeff-150">**要素**</span><span class="sxs-lookup"><span data-stu-id="2aeff-150">**Element**</span></span>|<span data-ttu-id="2aeff-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="2aeff-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2aeff-152">Attachments</span><span class="sxs-lookup"><span data-stu-id="2aeff-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2aeff-153">Exchange ストア内のアイテムに添付されているアイテムやファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="2aeff-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2aeff-154">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2aeff-154">Text value</span></span>

<span data-ttu-id="2aeff-155">なし。</span><span class="sxs-lookup"><span data-stu-id="2aeff-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2aeff-156">注釈</span><span class="sxs-lookup"><span data-stu-id="2aeff-156">Remarks</span></span>

<span data-ttu-id="2aeff-157">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2aeff-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2aeff-158">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2aeff-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2aeff-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="2aeff-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2aeff-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2aeff-160">Schema Name</span></span>  <br/> |<span data-ttu-id="2aeff-161">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2aeff-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="2aeff-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2aeff-162">Validation File</span></span>  <br/> |<span data-ttu-id="2aeff-163">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2aeff-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2aeff-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2aeff-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="2aeff-165">正しくない</span><span class="sxs-lookup"><span data-stu-id="2aeff-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2aeff-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="2aeff-166">See also</span></span>

- [<span data-ttu-id="2aeff-167">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2aeff-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

