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
ms.openlocfilehash: f06ca0727916f415c648e876f88bf7eacef5a5ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759969"
---
# <a name="deletedevent"></a><span data-ttu-id="d56cd-103">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="d56cd-103">DeletedEvent</span></span>

<span data-ttu-id="d56cd-104">**DeletedEvent**要素は、アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-104">The **DeletedEvent** element represents an event in which an item or folder is deleted.</span></span> 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

<span data-ttu-id="d56cd-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="d56cd-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d56cd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d56cd-106">Attributes and elements</span></span>

<span data-ttu-id="d56cd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d56cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="d56cd-108">Attributes</span></span>

<span data-ttu-id="d56cd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d56cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d56cd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d56cd-110">Child elements</span></span>

|<span data-ttu-id="d56cd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d56cd-111">**Element**</span></span>|<span data-ttu-id="d56cd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d56cd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d56cd-113">透かし</span><span class="sxs-lookup"><span data-stu-id="d56cd-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d56cd-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="d56cd-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="d56cd-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="d56cd-116">アイテムまたはフォルダーの削除済みメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-116">Represents the timestamp of a deleted item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="d56cd-117">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="d56cd-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d56cd-118">削除されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-118">Represents the identifier of the deleted folder.</span></span>  <br/> |
|[<span data-ttu-id="d56cd-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="d56cd-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d56cd-120">削除された項目の識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-120">Represents the identifier of the deleted item.</span></span>  <br/> |
|[<span data-ttu-id="d56cd-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d56cd-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d56cd-122">フォルダーを削除する前に、削除された項目の親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="d56cd-122">Represents the identifier of the parent folder of the deleted item or folder before deletion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d56cd-123">親要素</span><span class="sxs-lookup"><span data-stu-id="d56cd-123">Parent elements</span></span>

|<span data-ttu-id="d56cd-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="d56cd-124">**Element**</span></span>|<span data-ttu-id="d56cd-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="d56cd-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d56cd-126">通知</span><span class="sxs-lookup"><span data-stu-id="d56cd-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d56cd-127">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d56cd-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d56cd-128">備考</span><span class="sxs-lookup"><span data-stu-id="d56cd-128">Remarks</span></span>

<span data-ttu-id="d56cd-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d56cd-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d56cd-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="d56cd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d56cd-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="d56cd-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d56cd-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d56cd-132">Schema name</span></span>  <br/> |<span data-ttu-id="d56cd-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d56cd-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d56cd-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d56cd-134">Validation file</span></span>  <br/> |<span data-ttu-id="d56cd-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d56cd-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d56cd-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d56cd-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d56cd-137">False</span><span class="sxs-lookup"><span data-stu-id="d56cd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d56cd-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="d56cd-138">See also</span></span>

- [<span data-ttu-id="d56cd-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="d56cd-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="d56cd-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="d56cd-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="d56cd-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="d56cd-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

