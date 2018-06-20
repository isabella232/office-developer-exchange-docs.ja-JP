---
title: NewMailEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewMailEvent
api_type:
- schema
ms.assetid: 45057945-a3ec-4dac-92db-f0dc5fcfc34d
description: NewMailEvent 要素は、メールボックス内の新しいメール アイテムによって発生するイベントを表します。
ms.openlocfilehash: 8df3e4a218a8eaa9d129854e4816a3a43beddafa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832527"
---
# <a name="newmailevent"></a><span data-ttu-id="0e354-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="0e354-103">NewMailEvent</span></span>

<span data-ttu-id="0e354-104">**NewMailEvent**要素は、メールボックス内の新しいメール アイテムによって発生するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="0e354-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="0e354-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="0e354-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e354-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0e354-106">Attributes and elements</span></span>

<span data-ttu-id="0e354-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e354-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e354-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e354-108">Attributes</span></span>

<span data-ttu-id="0e354-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e354-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e354-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e354-110">Child elements</span></span>

|<span data-ttu-id="0e354-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e354-111">**Element**</span></span>|<span data-ttu-id="0e354-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e354-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e354-113">透かし</span><span class="sxs-lookup"><span data-stu-id="0e354-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="0e354-114">メールボックス イベント テーブル内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="0e354-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="0e354-115">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="0e354-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="0e354-116">メールボックス内の新しいメール アイテムの受信のタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="0e354-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0e354-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="0e354-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0e354-118">新しいメール アイテムの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="0e354-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="0e354-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0e354-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0e354-120">新しい電子メール アイテムの親フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="0e354-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e354-121">親要素</span><span class="sxs-lookup"><span data-stu-id="0e354-121">Parent elements</span></span>

|<span data-ttu-id="0e354-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e354-122">**Element**</span></span>|<span data-ttu-id="0e354-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e354-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e354-124">通知</span><span class="sxs-lookup"><span data-stu-id="0e354-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0e354-125">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e354-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0e354-126">備考</span><span class="sxs-lookup"><span data-stu-id="0e354-126">Remarks</span></span>

<span data-ttu-id="0e354-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0e354-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e354-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="0e354-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e354-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="0e354-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e354-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e354-130">Schema name</span></span>  <br/> |<span data-ttu-id="0e354-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0e354-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e354-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e354-132">Validation file</span></span>  <br/> |<span data-ttu-id="0e354-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0e354-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e354-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0e354-134">Can be empty</span></span>  <br/> |<span data-ttu-id="0e354-135">False</span><span class="sxs-lookup"><span data-stu-id="0e354-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e354-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e354-136">See also</span></span>



[<span data-ttu-id="0e354-137">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="0e354-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0e354-138">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="0e354-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="0e354-139">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="0e354-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

