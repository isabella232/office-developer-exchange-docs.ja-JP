---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: AppendToItemField 要素は、UpdateItem 操作中に 1 つのアイテムのプロパティを追加するデータを識別します。
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759338"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="9ec90-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="9ec90-103">AppendToItemField</span></span>

<span data-ttu-id="9ec90-104">**AppendToItemField**要素は、 [UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="9ec90-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="9ec90-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="9ec90-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="9ec90-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="9ec90-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="9ec90-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="9ec90-108">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="9ec90-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="9ec90-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="9ec90-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="9ec90-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="9ec90-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ec90-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ec90-111">Attributes and elements</span></span>

<span data-ttu-id="9ec90-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ec90-113">属性</span><span class="sxs-lookup"><span data-stu-id="9ec90-113">Attributes</span></span>

<span data-ttu-id="9ec90-114">なし。</span><span class="sxs-lookup"><span data-stu-id="9ec90-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ec90-115">子要素</span><span class="sxs-lookup"><span data-stu-id="9ec90-115">Child elements</span></span>

|<span data-ttu-id="9ec90-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ec90-116">**Element**</span></span>|<span data-ttu-id="9ec90-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ec90-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ec90-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="9ec90-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="9ec90-119">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9ec90-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="9ec90-121">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9ec90-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9ec90-123">追加するのには、拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-124">アイテム</span><span class="sxs-lookup"><span data-stu-id="9ec90-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="9ec90-125">Exchange ストア内の項目を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-126">Message</span><span class="sxs-lookup"><span data-stu-id="9ec90-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9ec90-127">Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-128">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="9ec90-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9ec90-129">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-130">Contact</span><span class="sxs-lookup"><span data-stu-id="9ec90-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9ec90-131">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9ec90-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="9ec90-133">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9ec90-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9ec90-135">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9ec90-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9ec90-137">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9ec90-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9ec90-139">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9ec90-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9ec90-141">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9ec90-142">タスク</span><span class="sxs-lookup"><span data-stu-id="9ec90-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="9ec90-143">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ec90-144">親要素</span><span class="sxs-lookup"><span data-stu-id="9ec90-144">Parent elements</span></span>

|<span data-ttu-id="9ec90-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ec90-145">**Element**</span></span>|<span data-ttu-id="9ec90-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ec90-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ec90-147">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="9ec90-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="9ec90-148">定義する配列が含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="9ec90-149">この要素への XPath 式は、次のようにします。`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="9ec90-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ec90-150">備考</span><span class="sxs-lookup"><span data-stu-id="9ec90-150">Remarks</span></span>

<span data-ttu-id="9ec90-151">特定のプロパティのサポートだけでは、操作を追加します。</span><span class="sxs-lookup"><span data-stu-id="9ec90-151">Only certain properties support append operations.</span></span> <span data-ttu-id="9ec90-152">追加することをサポートしていないプロパティを追加しようとするは、エラーになります。</span><span class="sxs-lookup"><span data-stu-id="9ec90-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="9ec90-153">更新操作の場合は、1 つの要求内で 1 つのプロパティを変更できます。</span><span class="sxs-lookup"><span data-stu-id="9ec90-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="9ec90-154">その 1 つのプロパティは、 [Path](path.md)要素に参照されなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9ec90-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="9ec90-155">だけ、派生クラス内の**項目**要素では、**パス**要素を 1 つだけ、1 つのプロパティを格納できますし。</span><span class="sxs-lookup"><span data-stu-id="9ec90-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9ec90-156">[Path](path.md)要素は、抽象です。</span><span class="sxs-lookup"><span data-stu-id="9ec90-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="9ec90-157">[FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素によってそれに置き換え 必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ec90-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="9ec90-158">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="9ec90-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ec90-159">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ec90-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ec90-160">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ec90-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ec90-161">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ec90-161">Schema Name</span></span>  <br/> |<span data-ttu-id="9ec90-162">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9ec90-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ec90-163">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ec90-163">Validation File</span></span>  <br/> |<span data-ttu-id="9ec90-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ec90-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ec90-165">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ec90-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ec90-166">False</span><span class="sxs-lookup"><span data-stu-id="9ec90-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ec90-167">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ec90-167">See also</span></span>

- <span data-ttu-id="9ec90-168">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="9ec90-168">[UpdateItem operation](updateitem-operation.md)</span></span>
- [<span data-ttu-id="9ec90-169">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ec90-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

