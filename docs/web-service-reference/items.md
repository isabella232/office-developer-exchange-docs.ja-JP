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
description: 項目要素には、項目の配列が含まれています。
ms.openlocfilehash: 241a56ee23e87d6a4320b93cc65b1f5aa1f60120
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832163"
---
# <a name="items"></a><span data-ttu-id="d5165-103">アイテム</span><span class="sxs-lookup"><span data-stu-id="d5165-103">Items</span></span>

<span data-ttu-id="d5165-104">**項目**要素には、項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5165-104">The **Items** element contains an array of items.</span></span> 
  
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

 <span data-ttu-id="d5165-105">**ArrayOfRealItemsType**</span><span class="sxs-lookup"><span data-stu-id="d5165-105">**ArrayOfRealItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5165-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d5165-106">Attributes and elements</span></span>

<span data-ttu-id="d5165-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5165-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5165-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5165-108">Attributes</span></span>

<span data-ttu-id="d5165-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d5165-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5165-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d5165-110">Child elements</span></span>

|<span data-ttu-id="d5165-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5165-111">**Element**</span></span>|<span data-ttu-id="d5165-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5165-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5165-113">Item</span><span class="sxs-lookup"><span data-stu-id="d5165-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="d5165-114">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-115">Message</span><span class="sxs-lookup"><span data-stu-id="d5165-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d5165-116">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-116">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="d5165-117">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="d5165-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d5165-118">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d5165-119">Contact</span><span class="sxs-lookup"><span data-stu-id="d5165-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d5165-120">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="d5165-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d5165-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d5165-122">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d5165-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d5165-124">Exchange ストア内の会議のメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-125">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d5165-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d5165-126">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d5165-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d5165-128">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d5165-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d5165-130">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-131">タスク</span><span class="sxs-lookup"><span data-stu-id="d5165-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="d5165-132">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d5165-133">PostItem</span><span class="sxs-lookup"><span data-stu-id="d5165-133">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="d5165-134">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-134">Represents a post item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5165-135">親要素</span><span class="sxs-lookup"><span data-stu-id="d5165-135">Parent elements</span></span>

|<span data-ttu-id="d5165-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5165-136">**Element**</span></span>|<span data-ttu-id="d5165-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5165-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5165-138">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-138">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="d5165-139">[CopyItem 操作](copyitem-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="d5165-139">Contains the status and result of a [CopyItem operation](copyitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d5165-140">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-140">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="d5165-141">状態および 1 つの結果が含まれています[CreateItem 操作](createitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="d5165-141">Contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d5165-142">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-142">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="d5165-143">[GetItem 操作](getitem-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="d5165-143">Contains the status and result of a [GetItem operation](getitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d5165-144">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d5165-144">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="d5165-145">グループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="d5165-145">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="d5165-146">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-146">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="d5165-147">[MoveItem 操作](moveitem-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="d5165-147">Contains the status and result of a [MoveItem operation](moveitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="d5165-148">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d5165-148">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="d5165-149">[FindItem 操作](finditem-operation.md)時に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5165-149">Contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="d5165-150">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d5165-150">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="d5165-151">[UpdateItem 操作](updateitem-operation.md)要求の結果ステータスを格納します。</span><span class="sxs-lookup"><span data-stu-id="d5165-151">Contains the status and result of an [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5165-152">備考</span><span class="sxs-lookup"><span data-stu-id="d5165-152">Remarks</span></span>

<span data-ttu-id="d5165-153">[CreateItem 操作](createitem-operation.md)要求内の項目の設定方法については、 [(NonEmptyArrayOfAllItemsType) の項目](items-nonemptyarrayofallitemstype.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5165-153">For information about the set of items in a [CreateItem operation](createitem-operation.md) request, see [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span></span>
  
<span data-ttu-id="d5165-154">[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d5165-154">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="d5165-155">IPM などの項目です。共有し、IPM.InfoPath は、**メッセージ**の要素として返されます。</span><span class="sxs-lookup"><span data-stu-id="d5165-155">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="d5165-156">バージョンの Exchange が Exchange Server 2010 で始まるでは、応答の基本要素の[項目](item.md)は返されません。</span><span class="sxs-lookup"><span data-stu-id="d5165-156">Versions of Exchange starting with Exchange Server 2010 do not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="d5165-157">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5165-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5165-158">要素情報</span><span class="sxs-lookup"><span data-stu-id="d5165-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5165-159">名前空間</span><span class="sxs-lookup"><span data-stu-id="d5165-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5165-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5165-160">Schema Name</span></span>  <br/> |<span data-ttu-id="d5165-161">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d5165-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5165-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5165-162">Validation File</span></span>  <br/> |<span data-ttu-id="d5165-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5165-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5165-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5165-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5165-165">False</span><span class="sxs-lookup"><span data-stu-id="d5165-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5165-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5165-166">See also</span></span>



<span data-ttu-id="d5165-167">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="d5165-167">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
  
- [<span data-ttu-id="d5165-168">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d5165-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

