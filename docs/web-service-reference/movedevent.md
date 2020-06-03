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
description: MovedEvent 要素は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。
ms.openlocfilehash: 1f8fb57dba7edb769fe0dd658d89c032dccf8c5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530409"
---
# <a name="movedevent"></a><span data-ttu-id="9ecc7-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="9ecc7-103">MovedEvent</span></span>

<span data-ttu-id="9ecc7-104">**Movedevent**要素は、ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
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


<span data-ttu-id="9ecc7-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="9ecc7-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9ecc7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9ecc7-106">Attributes and elements</span></span>

<span data-ttu-id="9ecc7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ecc7-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ecc7-108">Attributes</span></span>

<span data-ttu-id="9ecc7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ecc7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ecc7-110">Child elements</span></span>

|<span data-ttu-id="9ecc7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9ecc7-111">**Element**</span></span>|<span data-ttu-id="9ecc7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ecc7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ecc7-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="9ecc7-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9ecc7-114">メールボックスイベントテーブルのイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-115">示</span><span class="sxs-lookup"><span data-stu-id="9ecc7-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="9ecc7-116">移動アイテム/フォルダーメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9ecc7-118">移動されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9ecc7-120">移動されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9ecc7-122">移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="9ecc7-124">移動またはコピーされる前の元のフォルダーのフォルダー識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="9ecc7-126">移動される前の元のアイテムの一意識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="9ecc7-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9ecc7-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="9ecc7-128">移動されたアイテムまたはフォルダーの元の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ecc7-129">親要素</span><span class="sxs-lookup"><span data-stu-id="9ecc7-129">Parent elements</span></span>

|<span data-ttu-id="9ecc7-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ecc7-130">**Element**</span></span>|<span data-ttu-id="9ecc7-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ecc7-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ecc7-132">通知</span><span class="sxs-lookup"><span data-stu-id="9ecc7-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9ecc7-133">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ecc7-134">注釈</span><span class="sxs-lookup"><span data-stu-id="9ecc7-134">Remarks</span></span>

<span data-ttu-id="9ecc7-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ecc7-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9ecc7-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ecc7-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ecc7-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ecc7-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ecc7-138">Schema name</span></span>  <br/> |<span data-ttu-id="9ecc7-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9ecc7-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ecc7-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ecc7-140">Validation file</span></span>  <br/> |<span data-ttu-id="9ecc7-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9ecc7-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ecc7-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9ecc7-142">Can be empty</span></span>  <br/> |<span data-ttu-id="9ecc7-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="9ecc7-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ecc7-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ecc7-144">See also</span></span>

- [<span data-ttu-id="9ecc7-145">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9ecc7-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="9ecc7-146">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9ecc7-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="9ecc7-147">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9ecc7-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

