---
title: ModifiedEvent
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
description: ModifiedEvent 要素は、アイテムまたはフォルダーが変更されるイベントを表します。
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832482"
---
# <a name="modifiedevent"></a><span data-ttu-id="1ae16-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="1ae16-103">ModifiedEvent</span></span>

<span data-ttu-id="1ae16-104">**ModifiedEvent**要素は、アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 <span data-ttu-id="1ae16-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="1ae16-105">**ModifiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ae16-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1ae16-106">Attributes and elements</span></span>

<span data-ttu-id="1ae16-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ae16-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ae16-108">Attributes</span></span>

<span data-ttu-id="1ae16-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1ae16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ae16-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1ae16-110">Child elements</span></span>

|<span data-ttu-id="1ae16-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ae16-111">**Element**</span></span>|<span data-ttu-id="1ae16-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ae16-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ae16-113">透かし</span><span class="sxs-lookup"><span data-stu-id="1ae16-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="1ae16-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="1ae16-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="1ae16-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="1ae16-116">変更されたアイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="1ae16-117">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="1ae16-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="1ae16-118">変更されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="1ae16-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="1ae16-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="1ae16-120">変更されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="1ae16-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="1ae16-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="1ae16-122">変更されたアイテムまたはフォルダーの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="1ae16-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="1ae16-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="1ae16-124">指定したフォルダー内の未読アイテムの数を表します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ae16-125">親要素</span><span class="sxs-lookup"><span data-stu-id="1ae16-125">Parent elements</span></span>

|<span data-ttu-id="1ae16-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ae16-126">**Element**</span></span>|<span data-ttu-id="1ae16-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ae16-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ae16-128">通知</span><span class="sxs-lookup"><span data-stu-id="1ae16-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1ae16-129">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ae16-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ae16-130">備考</span><span class="sxs-lookup"><span data-stu-id="1ae16-130">Remarks</span></span>

<span data-ttu-id="1ae16-131">フォルダー内のアイテムの各変更に対して 2 つの変更イベントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="1ae16-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="1ae16-132">1 つのイベントは、変更されたアイテムに関連します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="1ae16-133">その他のイベントは、アイテムの親フォルダーに関連します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="1ae16-134">これは、サブスクリプションが作成されたのと同じフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="1ae16-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="1ae16-135">フォルダーの[UnreadCount](unreadcount.md)プロパティへの潜在的な変更を通信するためにこのフォルダーに関連付けられているイベントを使用します。</span><span class="sxs-lookup"><span data-stu-id="1ae16-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="1ae16-136">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1ae16-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ae16-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="1ae16-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ae16-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="1ae16-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ae16-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ae16-139">Schema name</span></span>  <br/> |<span data-ttu-id="1ae16-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ae16-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ae16-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ae16-141">Validation file</span></span>  <br/> |<span data-ttu-id="1ae16-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ae16-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ae16-143">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1ae16-143">Can be empty</span></span>  <br/> |<span data-ttu-id="1ae16-144">False</span><span class="sxs-lookup"><span data-stu-id="1ae16-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ae16-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ae16-145">See also</span></span>



[<span data-ttu-id="1ae16-146">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="1ae16-146">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="1ae16-147">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="1ae16-147">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="1ae16-148">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="1ae16-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

