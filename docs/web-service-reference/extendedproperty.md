---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: ExtendedProperty 要素では、フォルダーおよびアイテムの拡張 MAPI プロパティを識別します。
ms.openlocfilehash: 6a0aecc732ef634c2258127fca89b19461e25762
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760409"
---
# <a name="extendedproperty"></a><span data-ttu-id="e6c15-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e6c15-103">ExtendedProperty</span></span>

<span data-ttu-id="e6c15-104">**ExtendedProperty**要素では、フォルダーおよびアイテムの拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

 <span data-ttu-id="e6c15-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="e6c15-105">**ExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6c15-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e6c15-106">Attributes and elements</span></span>

<span data-ttu-id="e6c15-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6c15-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6c15-108">Attributes</span></span>

<span data-ttu-id="e6c15-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e6c15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6c15-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e6c15-110">Child elements</span></span>

|<span data-ttu-id="e6c15-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6c15-111">**Element**</span></span>|<span data-ttu-id="e6c15-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6c15-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6c15-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e6c15-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e6c15-114">取得、設定、または作成する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-115">Values</span><span class="sxs-lookup"><span data-stu-id="e6c15-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="e6c15-116">複数値を持つ拡張 MAPI プロパティの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6c15-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-117">値</span><span class="sxs-lookup"><span data-stu-id="e6c15-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="e6c15-118">単一値の MAPI 拡張プロパティの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e6c15-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6c15-119">親要素</span><span class="sxs-lookup"><span data-stu-id="e6c15-119">Parent elements</span></span>

|<span data-ttu-id="e6c15-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6c15-120">**Element**</span></span>|<span data-ttu-id="e6c15-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6c15-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6c15-122">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="e6c15-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e6c15-123">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-124">Contact</span><span class="sxs-lookup"><span data-stu-id="e6c15-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e6c15-125">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e6c15-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e6c15-127">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-128">アイテム</span><span class="sxs-lookup"><span data-stu-id="e6c15-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="e6c15-129">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e6c15-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e6c15-131">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e6c15-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e6c15-133">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e6c15-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e6c15-135">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e6c15-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e6c15-137">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-138">Message</span><span class="sxs-lookup"><span data-stu-id="e6c15-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e6c15-139">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="e6c15-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="e6c15-141">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-142">タスク</span><span class="sxs-lookup"><span data-stu-id="e6c15-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="e6c15-143">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="e6c15-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="e6c15-145">主に予定表のアイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-146">メッセージ</span><span class="sxs-lookup"><span data-stu-id="e6c15-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="e6c15-147">メールボックスの連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-148">Folder</span><span class="sxs-lookup"><span data-stu-id="e6c15-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="e6c15-149">作成、取得、検索、同期、または更新するフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="e6c15-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="e6c15-151">メールボックスに格納されている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e6c15-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="e6c15-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="e6c15-153">メールボックスに含まれるタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="e6c15-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e6c15-154">備考</span><span class="sxs-lookup"><span data-stu-id="e6c15-154">Remarks</span></span>

<span data-ttu-id="e6c15-155">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e6c15-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6c15-156">要素情報</span><span class="sxs-lookup"><span data-stu-id="e6c15-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6c15-157">名前空間</span><span class="sxs-lookup"><span data-stu-id="e6c15-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6c15-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e6c15-158">Schema Name</span></span>  <br/> |<span data-ttu-id="e6c15-159">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e6c15-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6c15-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e6c15-160">Validation File</span></span>  <br/> |<span data-ttu-id="e6c15-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6c15-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6c15-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e6c15-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6c15-163">False</span><span class="sxs-lookup"><span data-stu-id="e6c15-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6c15-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6c15-164">See also</span></span>



- [<span data-ttu-id="e6c15-165">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e6c15-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

