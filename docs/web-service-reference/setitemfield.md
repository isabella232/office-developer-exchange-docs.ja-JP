---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: SetItemField 要素は、UpdateItem 操作内の項目の 1 つのプロパティへの更新プログラムを表します。
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833439"
---
# <a name="setitemfield"></a><span data-ttu-id="c058e-103">SetItemField</span><span class="sxs-lookup"><span data-stu-id="c058e-103">SetItemField</span></span>

<span data-ttu-id="c058e-104">**SetItemField**要素は、 [UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティへの更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 <span data-ttu-id="c058e-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="c058e-105">**SetItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c058e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c058e-106">Attributes and elements</span></span>

<span data-ttu-id="c058e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c058e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c058e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c058e-108">Attributes</span></span>

<span data-ttu-id="c058e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c058e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c058e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c058e-110">Child elements</span></span>

|<span data-ttu-id="c058e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c058e-111">**Element**</span></span>|<span data-ttu-id="c058e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c058e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c058e-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c058e-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c058e-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c058e-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c058e-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c058e-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c058e-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c058e-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c058e-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c058e-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c058e-118">設定するのには、拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c058e-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="c058e-119">アイテム</span><span class="sxs-lookup"><span data-stu-id="c058e-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="c058e-120">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c058e-121">Message</span><span class="sxs-lookup"><span data-stu-id="c058e-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c058e-122">更新する Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-123">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="c058e-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c058e-124">更新するのには、Exchange 予定表のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-125">Contact</span><span class="sxs-lookup"><span data-stu-id="c058e-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c058e-126">Exchange 連絡先を更新する項目を表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c058e-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c058e-128">更新する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c058e-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c058e-130">会議を更新するメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c058e-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c058e-132">更新する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c058e-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c058e-134">更新するのには会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c058e-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c058e-136">更新するのには、会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="c058e-137">タスク</span><span class="sxs-lookup"><span data-stu-id="c058e-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="c058e-138">更新するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="c058e-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c058e-139">親要素</span><span class="sxs-lookup"><span data-stu-id="c058e-139">Parent elements</span></span>

|<span data-ttu-id="c058e-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="c058e-140">**Element**</span></span>|<span data-ttu-id="c058e-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="c058e-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c058e-142">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="c058e-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="c058e-143">定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="c058e-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c058e-144">備考</span><span class="sxs-lookup"><span data-stu-id="c058e-144">Remarks</span></span>

<span data-ttu-id="c058e-145">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c058e-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c058e-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="c058e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c058e-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="c058e-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c058e-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c058e-148">Schema Name</span></span>  <br/> |<span data-ttu-id="c058e-149">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c058e-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="c058e-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c058e-150">Validation File</span></span>  <br/> |<span data-ttu-id="c058e-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c058e-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c058e-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c058e-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="c058e-153">False</span><span class="sxs-lookup"><span data-stu-id="c058e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c058e-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="c058e-154">See also</span></span>



<span data-ttu-id="c058e-155">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c058e-155">[UpdateItem operation](updateitem-operation.md)</span></span>

