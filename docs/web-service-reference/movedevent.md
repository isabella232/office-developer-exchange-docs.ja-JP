---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: MovedEvent 要素は、アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。
ms.openlocfilehash: 07f9c02ea194187a9fdfb1e27b19eb311392f51f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353260"
---
# <a name="movedevent"></a><span data-ttu-id="6f939-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="6f939-103">MovedEvent</span></span>

<span data-ttu-id="6f939-104">**MovedEvent**要素は、アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


<span data-ttu-id="6f939-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="6f939-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6f939-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6f939-106">Attributes and elements</span></span>

<span data-ttu-id="6f939-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f939-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f939-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f939-108">Attributes</span></span>

<span data-ttu-id="6f939-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6f939-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f939-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6f939-110">Child elements</span></span>

|<span data-ttu-id="6f939-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="6f939-111">**Element**</span></span>|<span data-ttu-id="6f939-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f939-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f939-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="6f939-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="6f939-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="6f939-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="6f939-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="6f939-116">移動アイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="6f939-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="6f939-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6f939-118">移動したフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="6f939-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="6f939-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="6f939-120">移動された項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="6f939-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6f939-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="6f939-122">移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6f939-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="6f939-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="6f939-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="6f939-124">移動またはコピーする前に元のフォルダーのフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f939-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="6f939-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="6f939-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="6f939-126">移動する前に元のアイテムの一意の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f939-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="6f939-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="6f939-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="6f939-128">アイテムまたはフォルダーの移動元の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f939-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f939-129">親要素</span><span class="sxs-lookup"><span data-stu-id="6f939-129">Parent elements</span></span>

|<span data-ttu-id="6f939-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="6f939-130">**Element**</span></span>|<span data-ttu-id="6f939-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="6f939-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f939-132">通知</span><span class="sxs-lookup"><span data-stu-id="6f939-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6f939-133">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f939-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f939-134">注釈</span><span class="sxs-lookup"><span data-stu-id="6f939-134">Remarks</span></span>

<span data-ttu-id="6f939-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6f939-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f939-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="6f939-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f939-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="6f939-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f939-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6f939-138">Schema name</span></span>  <br/> |<span data-ttu-id="6f939-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6f939-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f939-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6f939-140">Validation file</span></span>  <br/> |<span data-ttu-id="6f939-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f939-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f939-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f939-142">Can be empty</span></span>  <br/> |<span data-ttu-id="6f939-143">False</span><span class="sxs-lookup"><span data-stu-id="6f939-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f939-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="6f939-144">See also</span></span>

- [<span data-ttu-id="6f939-145">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="6f939-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="6f939-146">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="6f939-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="6f939-147">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="6f939-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

