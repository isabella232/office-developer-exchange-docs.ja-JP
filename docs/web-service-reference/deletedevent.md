---
title: DeletedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: DeletedEvent 要素は、アイテムまたはフォルダーが削除されるイベントを表します。
ms.openlocfilehash: 5eb0c947aacc592f81c595da2cc00bf4874f300b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526943"
---
# <a name="deletedevent"></a><span data-ttu-id="5bddd-103">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="5bddd-103">DeletedEvent</span></span>

<span data-ttu-id="5bddd-104">**Deletedevent**要素は、アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-104">The **DeletedEvent** element represents an event in which an item or folder is deleted.</span></span> 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</DeletedEvent>
```

<span data-ttu-id="5bddd-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="5bddd-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5bddd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5bddd-106">Attributes and elements</span></span>

<span data-ttu-id="5bddd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bddd-108">属性</span><span class="sxs-lookup"><span data-stu-id="5bddd-108">Attributes</span></span>

<span data-ttu-id="5bddd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5bddd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bddd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5bddd-110">Child elements</span></span>

|<span data-ttu-id="5bddd-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5bddd-111">**Element**</span></span>|<span data-ttu-id="5bddd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bddd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bddd-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="5bddd-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="5bddd-114">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="5bddd-115">示</span><span class="sxs-lookup"><span data-stu-id="5bddd-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="5bddd-116">削除されたアイテムまたはフォルダーのメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-116">Represents the timestamp of a deleted item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="5bddd-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="5bddd-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="5bddd-118">削除されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-118">Represents the identifier of the deleted folder.</span></span>  <br/> |
|[<span data-ttu-id="5bddd-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="5bddd-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5bddd-120">削除されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-120">Represents the identifier of the deleted item.</span></span>  <br/> |
|[<span data-ttu-id="5bddd-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5bddd-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5bddd-122">削除する前に削除されたアイテムまたはフォルダーの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5bddd-122">Represents the identifier of the parent folder of the deleted item or folder before deletion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5bddd-123">親要素</span><span class="sxs-lookup"><span data-stu-id="5bddd-123">Parent elements</span></span>

|<span data-ttu-id="5bddd-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="5bddd-124">**Element**</span></span>|<span data-ttu-id="5bddd-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="5bddd-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bddd-126">通知</span><span class="sxs-lookup"><span data-stu-id="5bddd-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5bddd-127">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5bddd-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bddd-128">注釈</span><span class="sxs-lookup"><span data-stu-id="5bddd-128">Remarks</span></span>

<span data-ttu-id="5bddd-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5bddd-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bddd-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5bddd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bddd-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5bddd-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bddd-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5bddd-132">Schema name</span></span>  <br/> |<span data-ttu-id="5bddd-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5bddd-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bddd-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5bddd-134">Validation file</span></span>  <br/> |<span data-ttu-id="5bddd-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5bddd-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bddd-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5bddd-136">Can be empty</span></span>  <br/> |<span data-ttu-id="5bddd-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="5bddd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bddd-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5bddd-138">See also</span></span>

- [<span data-ttu-id="5bddd-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="5bddd-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="5bddd-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="5bddd-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="5bddd-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="5bddd-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

