---
title: アイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Items 要素には、項目の配列が含まれています。
ms.openlocfilehash: 489e34ad0e4bcc2520febb3c213db970fa496051
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458132"
---
# <a name="items"></a><span data-ttu-id="f9fa4-103">アイテム</span><span class="sxs-lookup"><span data-stu-id="f9fa4-103">Items</span></span>

<span data-ttu-id="f9fa4-104">**Items**要素には、項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-104">The **Items** element contains an array of items.</span></span> 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 <span data-ttu-id="f9fa4-105">**ArrayOfRealItemsType**</span><span class="sxs-lookup"><span data-stu-id="f9fa4-105">**ArrayOfRealItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9fa4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f9fa4-106">Attributes and elements</span></span>

<span data-ttu-id="f9fa4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9fa4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9fa4-108">Attributes</span></span>

<span data-ttu-id="f9fa4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9fa4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f9fa4-110">Child elements</span></span>

|<span data-ttu-id="f9fa4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f9fa4-111">**Element**</span></span>|<span data-ttu-id="f9fa4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9fa4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fa4-113">Item</span><span class="sxs-lookup"><span data-stu-id="f9fa4-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="f9fa4-114">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-115">Message</span><span class="sxs-lookup"><span data-stu-id="f9fa4-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f9fa4-116">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-116">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f9fa4-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f9fa4-118">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-119">Contact</span><span class="sxs-lookup"><span data-stu-id="f9fa4-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f9fa4-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f9fa4-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f9fa4-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f9fa4-124">Exchange ストア内の会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-125">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f9fa4-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f9fa4-126">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f9fa4-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f9fa4-128">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f9fa4-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f9fa4-130">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-131">タスク</span><span class="sxs-lookup"><span data-stu-id="f9fa4-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="f9fa4-132">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-133">PostItem</span><span class="sxs-lookup"><span data-stu-id="f9fa4-133">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="f9fa4-134">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-134">Represents a post item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9fa4-135">親要素</span><span class="sxs-lookup"><span data-stu-id="f9fa4-135">Parent elements</span></span>

|<span data-ttu-id="f9fa4-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="f9fa4-136">**Element**</span></span>|<span data-ttu-id="f9fa4-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9fa4-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fa4-138">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-138">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-139">[Copyitem 操作](copyitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-139">Contains the status and result of a [CopyItem operation](copyitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-140">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-140">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-141">単一の[CreateItem 操作](createitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-141">Contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-142">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-142">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-143">[GetItem 操作](getitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-143">Contains the status and result of a [GetItem operation](getitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-144">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="f9fa4-144">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="f9fa4-145">グループ化された[FindItem 操作](finditem-operation.md)呼び出しの結果であるアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-145">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-146">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-146">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-147">[Moveitem 操作](moveitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-147">Contains the status and result of a [MoveItem operation](moveitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-148">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="f9fa4-148">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-149">[FindItem 操作](finditem-operation.md)中の1つのルートフォルダの検索結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-149">Contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f9fa4-150">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9fa4-150">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="f9fa4-151">[Updateitem 操作](updateitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-151">Contains the status and result of an [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9fa4-152">注釈</span><span class="sxs-lookup"><span data-stu-id="f9fa4-152">Remarks</span></span>

<span data-ttu-id="f9fa4-153">[CreateItem 操作](createitem-operation.md)要求のアイテムセットの詳細については、「 [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-153">For information about the set of items in a [CreateItem operation](createitem-operation.md) request, see [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span></span>
  
<span data-ttu-id="f9fa4-154">[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージ、および Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-154">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="f9fa4-155">IPM などのアイテム。共有と IPM. InfoPath は、**メッセージ**要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-155">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="f9fa4-156">Exchange Server 2010 以降のバージョンの Exchange では、応答で基本[アイテム](item.md)要素は返されません。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-156">Versions of Exchange starting with Exchange Server 2010 do not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="f9fa4-157">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f9fa4-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9fa4-158">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f9fa4-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9fa4-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9fa4-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9fa4-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9fa4-160">Schema Name</span></span>  <br/> |<span data-ttu-id="f9fa4-161">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f9fa4-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9fa4-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9fa4-162">Validation File</span></span>  <br/> |<span data-ttu-id="f9fa4-163">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f9fa4-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9fa4-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f9fa4-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9fa4-165">正しくない</span><span class="sxs-lookup"><span data-stu-id="f9fa4-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9fa4-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9fa4-166">See also</span></span>



[<span data-ttu-id="f9fa4-167">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="f9fa4-167">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="f9fa4-168">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f9fa4-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

