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
description: AppendToItemField 要素は、UpdateItem 操作中にアイテムの1つのプロパティに追加するデータを識別します。
ms.openlocfilehash: 902239155bff45d6f81989de954c9459cf012288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466046"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="af6b8-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="af6b8-103">AppendToItemField</span></span>

<span data-ttu-id="af6b8-104">**Appendtoitemfield**要素は、 [updateitem 操作](updateitem-operation.md)中にアイテムの1つのプロパティに追加するデータを識別します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="af6b8-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="af6b8-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="af6b8-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="af6b8-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="af6b8-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="af6b8-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="af6b8-108">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="af6b8-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="af6b8-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="af6b8-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="af6b8-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="af6b8-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af6b8-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="af6b8-111">Attributes and elements</span></span>

<span data-ttu-id="af6b8-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af6b8-113">属性</span><span class="sxs-lookup"><span data-stu-id="af6b8-113">Attributes</span></span>

<span data-ttu-id="af6b8-114">なし。</span><span class="sxs-lookup"><span data-stu-id="af6b8-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af6b8-115">子要素</span><span class="sxs-lookup"><span data-stu-id="af6b8-115">Child elements</span></span>

|<span data-ttu-id="af6b8-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="af6b8-116">**Element**</span></span>|<span data-ttu-id="af6b8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="af6b8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af6b8-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="af6b8-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="af6b8-119">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="af6b8-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="af6b8-121">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="af6b8-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="af6b8-123">追加する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-124">アイテム</span><span class="sxs-lookup"><span data-stu-id="af6b8-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="af6b8-125">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-126">Message</span><span class="sxs-lookup"><span data-stu-id="af6b8-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="af6b8-127">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="af6b8-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="af6b8-129">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-130">連絡先</span><span class="sxs-lookup"><span data-stu-id="af6b8-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="af6b8-131">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="af6b8-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="af6b8-133">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="af6b8-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="af6b8-135">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="af6b8-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="af6b8-137">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="af6b8-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="af6b8-139">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="af6b8-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="af6b8-141">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af6b8-142">Task</span><span class="sxs-lookup"><span data-stu-id="af6b8-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="af6b8-143">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af6b8-144">親要素</span><span class="sxs-lookup"><span data-stu-id="af6b8-144">Parent elements</span></span>

|<span data-ttu-id="af6b8-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="af6b8-145">**Element**</span></span>|<span data-ttu-id="af6b8-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="af6b8-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af6b8-147">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="af6b8-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="af6b8-148">アイテムのプロパティに対する追加、設定、および削除の変更を定義する配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="af6b8-149">この要素の XPath 式を次に示します。`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="af6b8-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af6b8-150">注釈</span><span class="sxs-lookup"><span data-stu-id="af6b8-150">Remarks</span></span>

<span data-ttu-id="af6b8-151">追加操作をサポートするのは、特定のプロパティだけです。</span><span class="sxs-lookup"><span data-stu-id="af6b8-151">Only certain properties support append operations.</span></span> <span data-ttu-id="af6b8-152">追加をサポートしないプロパティに追加しようとすると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="af6b8-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="af6b8-153">更新操作では、1つの要求内で変更できるプロパティは1つだけです。</span><span class="sxs-lookup"><span data-stu-id="af6b8-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="af6b8-154">この単一のプロパティは[Path](path.md)要素で参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="af6b8-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="af6b8-155">派生クラスの**Item**要素は、1つの**Path**要素を使用して合意した1つのプロパティのみを保持できます。</span><span class="sxs-lookup"><span data-stu-id="af6b8-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="af6b8-156">[Path](path.md)要素は抽象型です。</span><span class="sxs-lookup"><span data-stu-id="af6b8-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="af6b8-157">[FieldURI](fielduri.md)、 [IndexedFieldURI](indexedfielduri.md)、または[ExtendedFieldURI](extendedfielduri.md)要素に置き換える必要があります。</span><span class="sxs-lookup"><span data-stu-id="af6b8-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="af6b8-158">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="af6b8-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af6b8-159">要素の情報</span><span class="sxs-lookup"><span data-stu-id="af6b8-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af6b8-160">Namespace</span><span class="sxs-lookup"><span data-stu-id="af6b8-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af6b8-161">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af6b8-161">Schema Name</span></span>  <br/> |<span data-ttu-id="af6b8-162">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="af6b8-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="af6b8-163">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af6b8-163">Validation File</span></span>  <br/> |<span data-ttu-id="af6b8-164">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="af6b8-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af6b8-165">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af6b8-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="af6b8-166">正しくない</span><span class="sxs-lookup"><span data-stu-id="af6b8-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af6b8-167">関連項目</span><span class="sxs-lookup"><span data-stu-id="af6b8-167">See also</span></span>

- <span data-ttu-id="af6b8-168">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="af6b8-168">[UpdateItem operation](updateitem-operation.md)</span></span>
- [<span data-ttu-id="af6b8-169">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="af6b8-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

