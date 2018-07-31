---
title: CreatedEvent
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
description: CreatedEvent 要素は、アイテムまたはフォルダーが作成されているイベントを表します。
ms.openlocfilehash: 791b8af87c0cc8ae7f07850e3a6fedd9975a251e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353176"
---
# <a name="createdevent"></a><span data-ttu-id="15b50-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="15b50-103">CreatedEvent</span></span>

<span data-ttu-id="15b50-104">**CreatedEvent**要素は、アイテムまたはフォルダーが作成されているイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
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

<span data-ttu-id="15b50-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="15b50-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15b50-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="15b50-106">Attributes and elements</span></span>

<span data-ttu-id="15b50-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15b50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15b50-108">属性</span><span class="sxs-lookup"><span data-stu-id="15b50-108">Attributes</span></span>

<span data-ttu-id="15b50-109">なし。</span><span class="sxs-lookup"><span data-stu-id="15b50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15b50-110">子要素</span><span class="sxs-lookup"><span data-stu-id="15b50-110">Child elements</span></span>

|<span data-ttu-id="15b50-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="15b50-111">**Element**</span></span>|<span data-ttu-id="15b50-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="15b50-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15b50-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="15b50-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="15b50-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="15b50-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="15b50-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="15b50-116">作成されたアイテムまたはフォルダーのメールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="15b50-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="15b50-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="15b50-118">作成したフォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="15b50-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="15b50-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="15b50-120">作成されたアイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="15b50-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="15b50-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="15b50-122">作成したアイテムまたはフォルダーの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="15b50-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15b50-123">親要素</span><span class="sxs-lookup"><span data-stu-id="15b50-123">Parent elements</span></span>

|<span data-ttu-id="15b50-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="15b50-124">**Element**</span></span>|<span data-ttu-id="15b50-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="15b50-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15b50-126">通知</span><span class="sxs-lookup"><span data-stu-id="15b50-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="15b50-127">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15b50-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15b50-128">注釈</span><span class="sxs-lookup"><span data-stu-id="15b50-128">Remarks</span></span>

<span data-ttu-id="15b50-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="15b50-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15b50-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="15b50-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15b50-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="15b50-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15b50-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15b50-132">Schema name</span></span>  <br/> |<span data-ttu-id="15b50-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="15b50-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="15b50-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15b50-134">Validation file</span></span>  <br/> |<span data-ttu-id="15b50-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15b50-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15b50-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="15b50-136">Can be empty</span></span>  <br/> |<span data-ttu-id="15b50-137">False</span><span class="sxs-lookup"><span data-stu-id="15b50-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15b50-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="15b50-138">See also</span></span>

- [<span data-ttu-id="15b50-139">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="15b50-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="15b50-140">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="15b50-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="15b50-141">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="15b50-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="15b50-142">プル サブスクリプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="15b50-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="15b50-143">EWS でのイベントの通知</span><span class="sxs-lookup"><span data-stu-id="15b50-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

