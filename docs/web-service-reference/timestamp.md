---
title: タイムスタンプ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: タイムスタンプの要素は、メールボックス イベントのタイムスタンプを表します。
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839743"
---
# <a name="timestamp"></a><span data-ttu-id="41ed7-103">タイムスタンプ</span><span class="sxs-lookup"><span data-stu-id="41ed7-103">TimeStamp</span></span>

<span data-ttu-id="41ed7-104">**タイムスタンプ**の要素は、メールボックス イベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-104">The **Timestamp** element represents the timestamp of a mailbox event.</span></span> 
  
```xml
<TimeStamp/>
```

 <span data-ttu-id="41ed7-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="41ed7-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41ed7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="41ed7-106">Attributes and elements</span></span>

<span data-ttu-id="41ed7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41ed7-108">属性</span><span class="sxs-lookup"><span data-stu-id="41ed7-108">Attributes</span></span>

<span data-ttu-id="41ed7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="41ed7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41ed7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="41ed7-110">Child elements</span></span>

<span data-ttu-id="41ed7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="41ed7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41ed7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="41ed7-112">Parent elements</span></span>

|<span data-ttu-id="41ed7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="41ed7-113">**Element**</span></span>|<span data-ttu-id="41ed7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="41ed7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41ed7-115">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-115">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="41ed7-116">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-116">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="41ed7-117">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-117">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="41ed7-118">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-118">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="41ed7-119">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-119">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="41ed7-120">アイテムまたはフォルダーが削除されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-120">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="41ed7-121">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-121">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="41ed7-122">アイテムまたはフォルダーが変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-122">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="41ed7-123">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-123">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="41ed7-124">アイテムまたはフォルダーの移動先フォルダーの 1 つの親から別の親フォルダー イベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-124">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="41ed7-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="41ed7-125">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="41ed7-126">メールボックス内の新しいメール アイテムによって発生したイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="41ed7-126">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41ed7-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="41ed7-127">Text value</span></span>

<span data-ttu-id="41ed7-128">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="41ed7-128">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41ed7-129">備考</span><span class="sxs-lookup"><span data-stu-id="41ed7-129">Remarks</span></span>

<span data-ttu-id="41ed7-130">この要素は、主にイベントの頻度の決定をクライアントで使用できます。</span><span class="sxs-lookup"><span data-stu-id="41ed7-130">This element is primarily available for use in client determination of event frequency.</span></span> <span data-ttu-id="41ed7-131">[StatusEvent](statusevent.md)の存在ではありません。</span><span class="sxs-lookup"><span data-stu-id="41ed7-131">This is not present in [StatusEvent](statusevent.md).</span></span>
  
<span data-ttu-id="41ed7-132">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="41ed7-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41ed7-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="41ed7-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41ed7-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="41ed7-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41ed7-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="41ed7-135">Schema name</span></span>  <br/> |<span data-ttu-id="41ed7-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="41ed7-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="41ed7-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="41ed7-137">Validation file</span></span>  <br/> |<span data-ttu-id="41ed7-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41ed7-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41ed7-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="41ed7-139">Can be empty</span></span>  <br/> |<span data-ttu-id="41ed7-140">False</span><span class="sxs-lookup"><span data-stu-id="41ed7-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41ed7-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="41ed7-141">See also</span></span>



[<span data-ttu-id="41ed7-142">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="41ed7-142">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="41ed7-143">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="41ed7-143">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="41ed7-144">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="41ed7-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

