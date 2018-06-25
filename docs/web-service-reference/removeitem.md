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
description: RemoveItem 要素は、MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。
ms.openlocfilehash: 6897363eba602e6a135ad255822197f9296dd44a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833108"
---
# <a name="removeitem"></a><span data-ttu-id="180dc-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="180dc-103">RemoveItem</span></span>

<span data-ttu-id="180dc-104">**RemoveItem**要素は、MeetingCancellation メッセージを受信したとき、会議アイテムを削除するために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="180dc-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="180dc-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="180dc-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="180dc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="180dc-106">Attributes and elements</span></span>

<span data-ttu-id="180dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="180dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="180dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="180dc-108">Attributes</span></span>

|<span data-ttu-id="180dc-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="180dc-109">**Attribute**</span></span>|<span data-ttu-id="180dc-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="180dc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="180dc-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="180dc-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="180dc-112">英語の文字列での RemoveItem 応答オブジェクトのクラスの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="180dc-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="180dc-113">子要素</span><span class="sxs-lookup"><span data-stu-id="180dc-113">Child elements</span></span>

|<span data-ttu-id="180dc-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="180dc-114">**Element**</span></span>|<span data-ttu-id="180dc-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="180dc-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="180dc-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="180dc-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="180dc-117">RemoveItem 応答オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="180dc-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="180dc-118">親要素</span><span class="sxs-lookup"><span data-stu-id="180dc-118">Parent elements</span></span>

|<span data-ttu-id="180dc-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="180dc-119">**Element**</span></span>|<span data-ttu-id="180dc-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="180dc-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="180dc-121">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="180dc-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="180dc-122">[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="180dc-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="180dc-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="180dc-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="180dc-124">Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="180dc-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="180dc-125">備考</span><span class="sxs-lookup"><span data-stu-id="180dc-125">Remarks</span></span>

 <span data-ttu-id="180dc-126">**RemoveItem**はの[MeetingCancellation](meetingcancellation.md)に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="180dc-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="180dc-127">それ以外の場合、エラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="180dc-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="180dc-128">会議の取り消しの[ItemClass](itemclass.md)は、IPM.Schedule.Meeting.Canceled。</span><span class="sxs-lookup"><span data-stu-id="180dc-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="180dc-129">の[MeetingRequest](meetingrequest.md)と関連付けられている[カレンダー項目](calendaritem.md)を削除する**での RemoveItem**の代わりに[DeclineItem](declineitem.md)の応答オブジェクトを使用します。</span><span class="sxs-lookup"><span data-stu-id="180dc-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="180dc-130">**RemoveItem**を代理人アクセスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="180dc-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="180dc-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="180dc-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="180dc-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="180dc-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="180dc-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="180dc-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="180dc-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="180dc-134">Schema Name</span></span>  <br/> |<span data-ttu-id="180dc-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="180dc-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="180dc-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="180dc-136">Validation File</span></span>  <br/> |<span data-ttu-id="180dc-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="180dc-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="180dc-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="180dc-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="180dc-139">False</span><span class="sxs-lookup"><span data-stu-id="180dc-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="180dc-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="180dc-140">See also</span></span>



- [<span data-ttu-id="180dc-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="180dc-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

