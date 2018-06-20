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
ms.openlocfilehash: a375f421ca9159103e47b515729316b21149c68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832479"
---
# <a name="movedevent"></a><span data-ttu-id="9b785-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="9b785-103">MovedEvent</span></span>

<span data-ttu-id="9b785-104">**MovedEvent**要素は、アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
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

 <span data-ttu-id="9b785-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="9b785-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b785-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9b785-106">Attributes and elements</span></span>

<span data-ttu-id="9b785-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9b785-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b785-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b785-108">Attributes</span></span>

<span data-ttu-id="9b785-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9b785-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b785-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9b785-110">Child elements</span></span>

|<span data-ttu-id="9b785-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9b785-111">**Element**</span></span>|<span data-ttu-id="9b785-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b785-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b785-113">透かし</span><span class="sxs-lookup"><span data-stu-id="9b785-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9b785-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="9b785-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="9b785-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="9b785-116">移動アイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="9b785-117">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="9b785-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9b785-118">移動したフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="9b785-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="9b785-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9b785-120">移動された項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="9b785-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9b785-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9b785-122">移動したアイテムまたはフォルダーを含むフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="9b785-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="9b785-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="9b785-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="9b785-124">移動またはコピーする前に元のフォルダーのフォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b785-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="9b785-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="9b785-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="9b785-126">移動する前に元のアイテムの一意の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b785-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="9b785-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9b785-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="9b785-128">アイテムまたはフォルダーの移動元の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b785-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b785-129">親要素</span><span class="sxs-lookup"><span data-stu-id="9b785-129">Parent elements</span></span>

|<span data-ttu-id="9b785-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="9b785-130">**Element**</span></span>|<span data-ttu-id="9b785-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="9b785-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b785-132">通知</span><span class="sxs-lookup"><span data-stu-id="9b785-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9b785-133">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9b785-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b785-134">備考</span><span class="sxs-lookup"><span data-stu-id="9b785-134">Remarks</span></span>

<span data-ttu-id="9b785-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9b785-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b785-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="9b785-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b785-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="9b785-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b785-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9b785-138">Schema name</span></span>  <br/> |<span data-ttu-id="9b785-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9b785-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b785-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9b785-140">Validation file</span></span>  <br/> |<span data-ttu-id="9b785-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9b785-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b785-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9b785-142">Can be empty</span></span>  <br/> |<span data-ttu-id="9b785-143">False</span><span class="sxs-lookup"><span data-stu-id="9b785-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b785-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="9b785-144">See also</span></span>



[<span data-ttu-id="9b785-145">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9b785-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="9b785-146">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9b785-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="9b785-147">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9b785-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

