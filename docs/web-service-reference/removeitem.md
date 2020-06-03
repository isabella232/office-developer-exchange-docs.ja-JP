---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: RemoveItem 要素は、会議の取り消しメッセージが受信されたときに会議アイテムを削除するために使用される response オブジェクトを表します。
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467691"
---
# <a name="removeitem"></a><span data-ttu-id="000a0-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="000a0-103">RemoveItem</span></span>

<span data-ttu-id="000a0-104">**Removeitem**要素は、会議の取り消しメッセージが受信されたときに会議アイテムを削除するために使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="000a0-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="000a0-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="000a0-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="000a0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="000a0-106">Attributes and elements</span></span>

<span data-ttu-id="000a0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="000a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="000a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="000a0-108">Attributes</span></span>

|<span data-ttu-id="000a0-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="000a0-109">**Attribute**</span></span>|<span data-ttu-id="000a0-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="000a0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000a0-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="000a0-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="000a0-112">RemoveItem reply オブジェクトクラスの名前を英語の文字列として表します。</span><span class="sxs-lookup"><span data-stu-id="000a0-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="000a0-113">子要素</span><span class="sxs-lookup"><span data-stu-id="000a0-113">Child elements</span></span>

|<span data-ttu-id="000a0-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="000a0-114">**Element**</span></span>|<span data-ttu-id="000a0-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="000a0-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="000a0-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="000a0-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="000a0-117">RemoveItem response オブジェクトが参照するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="000a0-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="000a0-118">親要素</span><span class="sxs-lookup"><span data-stu-id="000a0-118">Parent elements</span></span>

|<span data-ttu-id="000a0-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="000a0-119">**Element**</span></span>|<span data-ttu-id="000a0-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="000a0-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="000a0-121">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="000a0-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="000a0-122">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="000a0-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="000a0-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="000a0-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="000a0-124">Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="000a0-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="000a0-125">注釈</span><span class="sxs-lookup"><span data-stu-id="000a0-125">Remarks</span></span>

 <span data-ttu-id="000a0-126">**Removeitem**は、[会議の取り消し](meetingcancellation.md)に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="000a0-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="000a0-127">それ以外の場合は、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="000a0-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="000a0-128">会議のキャンセルの[Itemclass](itemclass.md)は IPM です。予約を取り消しました。</span><span class="sxs-lookup"><span data-stu-id="000a0-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="000a0-129">[会議の要求](meetingrequest.md)および関連付けられた予定表[アイテム](calendaritem.md)を削除するには、 **Removeitem**ではなく、 [declineitem](declineitem.md) response オブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="000a0-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="000a0-130">**Removeitem**は、代理人アクセスをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="000a0-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="000a0-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="000a0-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="000a0-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="000a0-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="000a0-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="000a0-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="000a0-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="000a0-134">Schema Name</span></span>  <br/> |<span data-ttu-id="000a0-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="000a0-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="000a0-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="000a0-136">Validation File</span></span>  <br/> |<span data-ttu-id="000a0-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="000a0-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="000a0-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="000a0-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="000a0-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="000a0-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="000a0-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="000a0-140">See also</span></span>



- [<span data-ttu-id="000a0-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="000a0-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

