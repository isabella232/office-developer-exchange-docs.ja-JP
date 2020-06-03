---
title: SuppressReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuppressReadReceipt
api_type:
- schema
ms.assetid: fc09bcc2-c003-4322-8315-d929bd0a9e2e
description: SuppressReadReceipt 要素は開封確認を抑制するために使用されます。
ms.openlocfilehash: b6b4fe5db26195882a7def5cac8266a942def996
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455955"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="f5e91-103">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="f5e91-103">SuppressReadReceipt</span></span>

<span data-ttu-id="f5e91-104">**SuppressReadReceipt**要素は開封確認を抑制するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5e91-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="f5e91-105">**SuppressReadReceiptType**</span><span class="sxs-lookup"><span data-stu-id="f5e91-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5e91-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f5e91-106">Attributes and elements</span></span>

<span data-ttu-id="f5e91-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5e91-108">属性</span><span class="sxs-lookup"><span data-stu-id="f5e91-108">Attributes</span></span>

<span data-ttu-id="f5e91-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f5e91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5e91-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f5e91-110">Child elements</span></span>

|<span data-ttu-id="f5e91-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f5e91-111">**Element**</span></span>|<span data-ttu-id="f5e91-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5e91-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5e91-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="f5e91-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="f5e91-114">Response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5e91-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f5e91-115">Parent elements</span></span>

|<span data-ttu-id="f5e91-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f5e91-116">**Element**</span></span>|<span data-ttu-id="f5e91-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f5e91-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5e91-118">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="f5e91-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="f5e91-119">会議の時刻に隣接しているすべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="f5e91-120">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="f5e91-121">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="f5e91-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="f5e91-122">会議の時間と競合するすべてのアイテムについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="f5e91-123">この要素の XPath 式の一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="f5e91-124">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="f5e91-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="f5e91-125">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="f5e91-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f5e91-126">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="f5e91-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="f5e91-127">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f5e91-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5e91-128">注釈</span><span class="sxs-lookup"><span data-stu-id="f5e91-128">Remarks</span></span>

<span data-ttu-id="f5e91-129">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="f5e91-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5e91-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f5e91-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5e91-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5e91-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5e91-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f5e91-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f5e91-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f5e91-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5e91-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f5e91-134">Validation File</span></span>  <br/> |<span data-ttu-id="f5e91-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f5e91-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5e91-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f5e91-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5e91-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="f5e91-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5e91-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="f5e91-138">See also</span></span>

- [<span data-ttu-id="f5e91-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f5e91-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

