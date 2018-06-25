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
description: CopiedEvent 要素は、アイテムまたはフォルダーのコピー先のイベントを表します。
ms.openlocfilehash: 89ca9fb1fd2f4187efdec0e087d840bfee197a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759774"
---
# <a name="copiedevent"></a><span data-ttu-id="b09ec-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="b09ec-103">CopiedEvent</span></span>

<span data-ttu-id="b09ec-104">**CopiedEvent**要素は、アイテムまたはフォルダーのコピー先のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
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

 <span data-ttu-id="b09ec-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="b09ec-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b09ec-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b09ec-106">Attributes and elements</span></span>

<span data-ttu-id="b09ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b09ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="b09ec-108">Attributes</span></span>

<span data-ttu-id="b09ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b09ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b09ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b09ec-110">Child elements</span></span>

|<span data-ttu-id="b09ec-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="b09ec-111">**Element**</span></span>|<span data-ttu-id="b09ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b09ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b09ec-113">透かし</span><span class="sxs-lookup"><span data-stu-id="b09ec-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="b09ec-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="b09ec-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="b09ec-116">コピー アイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-117">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="b09ec-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="b09ec-118">フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="b09ec-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b09ec-120">項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b09ec-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="b09ec-122">コピーを含むフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="b09ec-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="b09ec-124">それがコピーされる前に、元のフォルダーのフォルダー id を表します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="b09ec-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="b09ec-126">コピーする前に元のアイテムの一意の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b09ec-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="b09ec-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b09ec-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="b09ec-128">項目またはコピーしたフォルダーの元の親フォルダーの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b09ec-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b09ec-129">親要素</span><span class="sxs-lookup"><span data-stu-id="b09ec-129">Parent elements</span></span>

|<span data-ttu-id="b09ec-130">**要素**</span><span class="sxs-lookup"><span data-stu-id="b09ec-130">**Element**</span></span>|<span data-ttu-id="b09ec-131">**説明**</span><span class="sxs-lookup"><span data-stu-id="b09ec-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b09ec-132">通知</span><span class="sxs-lookup"><span data-stu-id="b09ec-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b09ec-133">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b09ec-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b09ec-134">備考</span><span class="sxs-lookup"><span data-stu-id="b09ec-134">Remarks</span></span>

<span data-ttu-id="b09ec-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="b09ec-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b09ec-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="b09ec-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b09ec-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="b09ec-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b09ec-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b09ec-138">Schema name</span></span>  <br/> |<span data-ttu-id="b09ec-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="b09ec-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b09ec-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b09ec-140">Validation file</span></span>  <br/> |<span data-ttu-id="b09ec-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b09ec-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b09ec-142">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b09ec-142">Can be empty</span></span>  <br/> |<span data-ttu-id="b09ec-143">False</span><span class="sxs-lookup"><span data-stu-id="b09ec-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b09ec-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="b09ec-144">See also</span></span>



[<span data-ttu-id="b09ec-145">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="b09ec-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="b09ec-146">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="b09ec-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="b09ec-147">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="b09ec-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="b09ec-148">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="b09ec-148">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="b09ec-149">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b09ec-149">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

