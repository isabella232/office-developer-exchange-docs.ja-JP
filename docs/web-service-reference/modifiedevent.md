---
title: 対する modifiedevent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: "\"修飾\" 要素は、アイテムまたはフォルダーが変更されるイベントを表します。"
ms.openlocfilehash: 1a798773601a0857b9064c7fa6a532a7a36517ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468552"
---
# <a name="modifiedevent"></a><span data-ttu-id="d866b-103">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="d866b-103">ModifiedEvent</span></span>

<span data-ttu-id="d866b-104">"修飾" 要素は、アイテムまたはフォルダーが変更されるイベントを**表します。**</span><span class="sxs-lookup"><span data-stu-id="d866b-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

<span data-ttu-id="d866b-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="d866b-105">**ModifiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d866b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d866b-106">Attributes and elements</span></span>

<span data-ttu-id="d866b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d866b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d866b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d866b-108">Attributes</span></span>

<span data-ttu-id="d866b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d866b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d866b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d866b-110">Child elements</span></span>

|<span data-ttu-id="d866b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d866b-111">**Element**</span></span>|<span data-ttu-id="d866b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d866b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d866b-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="d866b-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d866b-114">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="d866b-115">示</span><span class="sxs-lookup"><span data-stu-id="d866b-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="d866b-116">変更されたアイテムまたはフォルダーのメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="d866b-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="d866b-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d866b-118">変更されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="d866b-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="d866b-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d866b-120">変更されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="d866b-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d866b-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d866b-122">変更されたアイテムまたはフォルダーの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="d866b-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="d866b-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="d866b-124">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d866b-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d866b-125">親要素</span><span class="sxs-lookup"><span data-stu-id="d866b-125">Parent elements</span></span>

|<span data-ttu-id="d866b-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="d866b-126">**Element**</span></span>|<span data-ttu-id="d866b-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="d866b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d866b-128">通知</span><span class="sxs-lookup"><span data-stu-id="d866b-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d866b-129">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d866b-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d866b-130">注釈</span><span class="sxs-lookup"><span data-stu-id="d866b-130">Remarks</span></span>

<span data-ttu-id="d866b-131">フォルダー内のアイテムの変更ごとに、2つの変更されたイベントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="d866b-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="d866b-132">変更されたアイテムに関連するイベントが1つあります。</span><span class="sxs-lookup"><span data-stu-id="d866b-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="d866b-133">その他のイベントは、アイテムの親フォルダーに関連しています。</span><span class="sxs-lookup"><span data-stu-id="d866b-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="d866b-134">これは、サブスクリプションが作成されたものと同じフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="d866b-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="d866b-135">フォルダーに関連付けられているイベントを使用して、フォルダーの[UnreadCount](unreadcount.md)プロパティに対する潜在的な変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="d866b-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="d866b-136">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d866b-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d866b-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d866b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d866b-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="d866b-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d866b-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d866b-139">Schema name</span></span>  <br/> |<span data-ttu-id="d866b-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d866b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="d866b-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d866b-141">Validation file</span></span>  <br/> |<span data-ttu-id="d866b-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d866b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d866b-143">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d866b-143">Can be empty</span></span>  <br/> |<span data-ttu-id="d866b-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="d866b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d866b-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d866b-145">See also</span></span>

- [<span data-ttu-id="d866b-146">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d866b-146">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="d866b-147">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d866b-147">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="d866b-148">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d866b-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

