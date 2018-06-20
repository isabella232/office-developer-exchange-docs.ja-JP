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
description: SuppressReadReceipt 要素を使用して、開封確認メッセージを抑制します。
ms.openlocfilehash: de2eef68abd25c8208530ba5e98ab3278c8702d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839628"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="4182e-103">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="4182e-103">SuppressReadReceipt</span></span>

<span data-ttu-id="4182e-104">**SuppressReadReceipt**要素を使用して、開封確認メッセージを抑制します。</span><span class="sxs-lookup"><span data-stu-id="4182e-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="4182e-105">**SuppressReadReceiptType**</span><span class="sxs-lookup"><span data-stu-id="4182e-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4182e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4182e-106">Attributes and elements</span></span>

<span data-ttu-id="4182e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4182e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4182e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4182e-108">Attributes</span></span>

<span data-ttu-id="4182e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4182e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4182e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4182e-110">Child elements</span></span>

|<span data-ttu-id="4182e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4182e-111">**Element**</span></span>|<span data-ttu-id="4182e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4182e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4182e-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="4182e-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="4182e-114">応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="4182e-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4182e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4182e-115">Parent elements</span></span>

|<span data-ttu-id="4182e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4182e-116">**Element**</span></span>|<span data-ttu-id="4182e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4182e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4182e-118">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="4182e-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="4182e-119">会議の時刻に隣接しているすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="4182e-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="4182e-120">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="4182e-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="4182e-121">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="4182e-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="4182e-122">会議の時間と競合するすべての項目について説明します。</span><span class="sxs-lookup"><span data-stu-id="4182e-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="4182e-123">以下は、この要素への XPath 式の一部です。</span><span class="sxs-lookup"><span data-stu-id="4182e-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="4182e-124">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="4182e-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="4182e-125">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4182e-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4182e-126">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="4182e-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="4182e-127">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4182e-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4182e-128">備考</span><span class="sxs-lookup"><span data-stu-id="4182e-128">Remarks</span></span>

<span data-ttu-id="4182e-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4182e-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4182e-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="4182e-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4182e-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="4182e-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4182e-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4182e-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4182e-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4182e-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="4182e-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4182e-134">Validation File</span></span>  <br/> |<span data-ttu-id="4182e-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4182e-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4182e-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4182e-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4182e-137">False</span><span class="sxs-lookup"><span data-stu-id="4182e-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4182e-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="4182e-138">See also</span></span>

- [<span data-ttu-id="4182e-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4182e-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

