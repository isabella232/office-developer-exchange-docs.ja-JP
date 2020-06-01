---
title: 対する createdevent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreatedEvent
api_type:
- schema
ms.assetid: f0e53a53-c352-42a5-8280-cd808b0e961b
description: CreatedEvent 要素は、アイテムまたはフォルダーが作成されるイベントを表します。
ms.openlocfilehash: 546dde782b3b20cd76acb625067b5f2d8f568854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44445322"
---
# <a name="createdevent"></a><span data-ttu-id="e3abb-103">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="e3abb-103">CreatedEvent</span></span>

<span data-ttu-id="e3abb-104">**Createdevent**要素は、アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</CreatedEvent>
```

<span data-ttu-id="e3abb-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="e3abb-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e3abb-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e3abb-106">Attributes and elements</span></span>

<span data-ttu-id="e3abb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3abb-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3abb-108">Attributes</span></span>

<span data-ttu-id="e3abb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3abb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3abb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3abb-110">Child elements</span></span>

|<span data-ttu-id="e3abb-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e3abb-111">**Element**</span></span>|<span data-ttu-id="e3abb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3abb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3abb-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="e3abb-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="e3abb-114">メールボックスイベントテーブル内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="e3abb-115">示</span><span class="sxs-lookup"><span data-stu-id="e3abb-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="e3abb-116">作成されたアイテムまたはフォルダーのメールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="e3abb-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="e3abb-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e3abb-118">作成されたフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="e3abb-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="e3abb-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e3abb-120">作成されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="e3abb-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e3abb-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e3abb-122">作成されたアイテムまたはフォルダーの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e3abb-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3abb-123">親要素</span><span class="sxs-lookup"><span data-stu-id="e3abb-123">Parent elements</span></span>

|<span data-ttu-id="e3abb-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3abb-124">**Element**</span></span>|<span data-ttu-id="e3abb-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3abb-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3abb-126">通知</span><span class="sxs-lookup"><span data-stu-id="e3abb-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e3abb-127">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e3abb-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3abb-128">注釈</span><span class="sxs-lookup"><span data-stu-id="e3abb-128">Remarks</span></span>

<span data-ttu-id="e3abb-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e3abb-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3abb-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e3abb-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3abb-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3abb-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3abb-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3abb-132">Schema name</span></span>  <br/> |<span data-ttu-id="e3abb-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e3abb-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3abb-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3abb-134">Validation file</span></span>  <br/> |<span data-ttu-id="e3abb-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e3abb-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3abb-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e3abb-136">Can be empty</span></span>  <br/> |<span data-ttu-id="e3abb-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="e3abb-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3abb-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3abb-138">See also</span></span>

- [<span data-ttu-id="e3abb-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="e3abb-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="e3abb-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="e3abb-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="e3abb-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="e3abb-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="e3abb-142">プルサブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="e3abb-142">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="e3abb-143">EWS でのイベント通知</span><span class="sxs-lookup"><span data-stu-id="e3abb-143">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

