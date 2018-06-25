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
description: ItemAttachment 要素は、Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832137"
---
# <a name="itemattachment"></a><span data-ttu-id="43776-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="43776-103">ItemAttachment</span></span>

<span data-ttu-id="43776-104">**ItemAttachment**要素は、Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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

 <span data-ttu-id="43776-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="43776-105">**ItemAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43776-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="43776-106">Attributes and elements</span></span>

<span data-ttu-id="43776-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="43776-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43776-108">属性</span><span class="sxs-lookup"><span data-stu-id="43776-108">Attributes</span></span>

<span data-ttu-id="43776-109">なし。</span><span class="sxs-lookup"><span data-stu-id="43776-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43776-110">子要素</span><span class="sxs-lookup"><span data-stu-id="43776-110">Child elements</span></span>

|<span data-ttu-id="43776-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="43776-111">**Element**</span></span>|<span data-ttu-id="43776-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="43776-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43776-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="43776-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="43776-114">添付ファイルを識別します。</span><span class="sxs-lookup"><span data-stu-id="43776-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-115">名 (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="43776-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="43776-116">添付ファイルの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="43776-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="43776-118">添付ファイルのコンテンツの多目的インターネット メール拡張 (MIME) の種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="43776-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="43776-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="43776-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="43776-120">添付ファイルの内容には、識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="43776-121">[ContentId](contentid.md)は、任意の文字列値に設定できます。</span><span class="sxs-lookup"><span data-stu-id="43776-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="43776-122">アプリケーションは、独自の識別メカニズムを実装するために、 [ContentId](contentid.md)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="43776-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="43776-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="43776-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="43776-124">統一リソース識別子 (URI) の添付ファイルのコンテンツの場所に対応するが含まれています。</span><span class="sxs-lookup"><span data-stu-id="43776-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-125">Size</span><span class="sxs-lookup"><span data-stu-id="43776-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="43776-126">添付ファイルのバイト単位でサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="43776-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="43776-128">添付ファイルが最後に変更されたときを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="43776-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="43776-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="43776-130">添付ファイルの項目内でのインラインで表示されているかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="43776-131">アイテム</span><span class="sxs-lookup"><span data-stu-id="43776-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="43776-132">一般的な Exchange アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-133">Message</span><span class="sxs-lookup"><span data-stu-id="43776-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="43776-134">Exchange 電子メール メッセージの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-135">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="43776-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="43776-136">Exchange 予定表アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-137">Contact</span><span class="sxs-lookup"><span data-stu-id="43776-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="43776-138">Exchange 連絡先アイテムの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-139">タスク</span><span class="sxs-lookup"><span data-stu-id="43776-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="43776-140">Exchange タスクの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="43776-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="43776-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="43776-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="43776-142">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43776-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="43776-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="43776-144">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43776-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="43776-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="43776-146">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43776-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="43776-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="43776-148">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="43776-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43776-149">親要素</span><span class="sxs-lookup"><span data-stu-id="43776-149">Parent elements</span></span>

|<span data-ttu-id="43776-150">**要素**</span><span class="sxs-lookup"><span data-stu-id="43776-150">**Element**</span></span>|<span data-ttu-id="43776-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="43776-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43776-152">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="43776-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="43776-153">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="43776-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43776-154">テキスト値</span><span class="sxs-lookup"><span data-stu-id="43776-154">Text value</span></span>

<span data-ttu-id="43776-155">なし。</span><span class="sxs-lookup"><span data-stu-id="43776-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="43776-156">備考</span><span class="sxs-lookup"><span data-stu-id="43776-156">Remarks</span></span>

<span data-ttu-id="43776-157">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="43776-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43776-158">要素情報</span><span class="sxs-lookup"><span data-stu-id="43776-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43776-159">名前空間</span><span class="sxs-lookup"><span data-stu-id="43776-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43776-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="43776-160">Schema Name</span></span>  <br/> |<span data-ttu-id="43776-161">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="43776-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="43776-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="43776-162">Validation File</span></span>  <br/> |<span data-ttu-id="43776-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43776-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43776-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="43776-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="43776-165">False</span><span class="sxs-lookup"><span data-stu-id="43776-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43776-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="43776-166">See also</span></span>



- [<span data-ttu-id="43776-167">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="43776-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

