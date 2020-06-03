---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: CopiedEvent 要素は、アイテムまたはフォルダーがコピーされるイベントを表します。
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529246"
---
# <a name="copiedevent"></a><span data-ttu-id="9dde8-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="9dde8-103">CopiedEvent</span></span>

<span data-ttu-id="9dde8-104">**Copiedevent**要素は、アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

<span data-ttu-id="9dde8-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="9dde8-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9dde8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9dde8-106">Attributes and elements</span></span>

<span data-ttu-id="9dde8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9dde8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9dde8-108">Attributes</span></span>

<span data-ttu-id="9dde8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9dde8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9dde8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9dde8-110">Child elements</span></span>

|<span data-ttu-id="9dde8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9dde8-111">**Element**</span></span>|<span data-ttu-id="9dde8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9dde8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dde8-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="9dde8-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9dde8-114">メールボックスイベントテーブルのイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-115">示</span><span class="sxs-lookup"><span data-stu-id="9dde8-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="9dde8-116">コピーアイテム/フォルダーメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="9dde8-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9dde8-118">フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="9dde8-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9dde8-120">アイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9dde8-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9dde8-122">コピーが格納されているフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="9dde8-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="9dde8-124">コピー前の元のフォルダーのフォルダー識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9dde8-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="9dde8-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="9dde8-126">コピーされる前の元のアイテムの一意識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="9dde8-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="9dde8-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9dde8-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="9dde8-128">コピーされたアイテムまたはフォルダーの元の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9dde8-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9dde8-129">親要素</span><span class="sxs-lookup"><span data-stu-id="9dde8-129">Parent elements</span></span>

|<span data-ttu-id="9dde8-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="9dde8-130">**Element**</span></span>|<span data-ttu-id="9dde8-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="9dde8-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dde8-132">通知</span><span class="sxs-lookup"><span data-stu-id="9dde8-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9dde8-133">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9dde8-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9dde8-134">注釈</span><span class="sxs-lookup"><span data-stu-id="9dde8-134">Remarks</span></span>

<span data-ttu-id="9dde8-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9dde8-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9dde8-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9dde8-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9dde8-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="9dde8-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9dde8-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9dde8-138">Schema name</span></span>  <br/> |<span data-ttu-id="9dde8-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9dde8-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9dde8-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9dde8-140">Validation file</span></span>  <br/> |<span data-ttu-id="9dde8-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9dde8-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9dde8-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9dde8-142">Can be empty</span></span>  <br/> |<span data-ttu-id="9dde8-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="9dde8-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9dde8-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9dde8-144">See also</span></span>

- [<span data-ttu-id="9dde8-145">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9dde8-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="9dde8-146">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9dde8-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="9dde8-147">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9dde8-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="9dde8-148">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="9dde8-148">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="9dde8-149">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9dde8-149">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

