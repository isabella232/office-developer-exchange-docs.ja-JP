---
title: 示
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
description: Timestamp 要素は、メールボックスイベントのタイムスタンプを表します。
ms.openlocfilehash: f2280d4eab67b603963c4f0a7468bf35a2b63a88
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459890"
---
# <a name="timestamp"></a><span data-ttu-id="9cd93-103">示</span><span class="sxs-lookup"><span data-stu-id="9cd93-103">TimeStamp</span></span>

<span data-ttu-id="9cd93-104">**Timestamp**要素は、メールボックスイベントのタイムスタンプを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-104">The **Timestamp** element represents the timestamp of a mailbox event.</span></span> 
  
```xml
<TimeStamp/>
```

 <span data-ttu-id="9cd93-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="9cd93-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cd93-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9cd93-106">Attributes and elements</span></span>

<span data-ttu-id="9cd93-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cd93-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cd93-108">Attributes</span></span>

<span data-ttu-id="9cd93-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9cd93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cd93-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9cd93-110">Child elements</span></span>

<span data-ttu-id="9cd93-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cd93-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cd93-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9cd93-112">Parent elements</span></span>

|<span data-ttu-id="9cd93-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9cd93-113">**Element**</span></span>|<span data-ttu-id="9cd93-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cd93-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cd93-115">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="9cd93-115">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="9cd93-116">アイテムまたはフォルダーがコピーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-116">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="9cd93-117">対する createdevent</span><span class="sxs-lookup"><span data-stu-id="9cd93-117">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="9cd93-118">アイテムまたはフォルダーが作成されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-118">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="9cd93-119">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="9cd93-119">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="9cd93-120">アイテムまたはフォルダーが削除されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-120">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="9cd93-121">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="9cd93-121">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="9cd93-122">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-122">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="9cd93-123">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="9cd93-123">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="9cd93-124">ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-124">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="9cd93-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="9cd93-125">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="9cd93-126">メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-126">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cd93-127">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9cd93-127">Text value</span></span>

<span data-ttu-id="9cd93-128">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9cd93-128">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9cd93-129">注釈</span><span class="sxs-lookup"><span data-stu-id="9cd93-129">Remarks</span></span>

<span data-ttu-id="9cd93-130">この要素は、主に、イベント頻度をクライアントに決定するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="9cd93-130">This element is primarily available for use in client determination of event frequency.</span></span> <span data-ttu-id="9cd93-131">これは[Statusevent](statusevent.md)では存在しません。</span><span class="sxs-lookup"><span data-stu-id="9cd93-131">This is not present in [StatusEvent](statusevent.md).</span></span>
  
<span data-ttu-id="9cd93-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9cd93-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cd93-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9cd93-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cd93-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="9cd93-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cd93-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9cd93-135">Schema name</span></span>  <br/> |<span data-ttu-id="9cd93-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9cd93-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="9cd93-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9cd93-137">Validation file</span></span>  <br/> |<span data-ttu-id="9cd93-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9cd93-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cd93-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9cd93-139">Can be empty</span></span>  <br/> |<span data-ttu-id="9cd93-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="9cd93-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cd93-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="9cd93-141">See also</span></span>



[<span data-ttu-id="9cd93-142">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="9cd93-142">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="9cd93-143">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="9cd93-143">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="9cd93-144">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="9cd93-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

