---
title: UpdateItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: UpdateItem 操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459392"
---
# <a name="updateitem-operation"></a><span data-ttu-id="ce3d6-103">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="ce3d6-103">UpdateItem operation</span></span>

<span data-ttu-id="ce3d6-104">**Updateitem**操作は、Exchange ストア内の既存のアイテムのプロパティを変更するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ce3d6-105">注釈</span><span class="sxs-lookup"><span data-stu-id="ce3d6-105">Remarks</span></span>

<span data-ttu-id="ce3d6-106">アイテムに対して3つの基本的な更新操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="ce3d6-107">次の表に、実行できるアクションを示します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="ce3d6-108">**操作**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-108">**Action**</span></span>|<span data-ttu-id="ce3d6-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce3d6-110">追加</span><span class="sxs-lookup"><span data-stu-id="ce3d6-110">Append</span></span>  <br/> |<span data-ttu-id="ce3d6-111">既存のプロパティにデータを追加します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-111">Adds data to an existing property.</span></span> <span data-ttu-id="ce3d6-112">この操作を行うと、現在のデータが保持されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-112">This action preserves the current data.</span></span> <span data-ttu-id="ce3d6-113">Append は、すべてのプロパティに適用されません。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="ce3d6-114">Set</span><span class="sxs-lookup"><span data-stu-id="ce3d6-114">Set</span></span>  <br/> |<span data-ttu-id="ce3d6-115">プロパティのデータが含まれている場合は、プロパティのデータを置換します。プロパティが存在しない場合は、プロパティを作成し、その値を設定します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="ce3d6-116">Set アクションは、書き込み可能なプロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="ce3d6-117">削除</span><span class="sxs-lookup"><span data-stu-id="ce3d6-117">Delete</span></span>  <br/> |<span data-ttu-id="ce3d6-118">アイテムからプロパティを削除します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-118">Removes a property from an item.</span></span> <span data-ttu-id="ce3d6-119">これは、プロパティを空の値に設定することとは異なります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="ce3d6-120">この操作が完了すると、アイテムのプロパティが存在しなくなります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="ce3d6-121">Delete は、書き込み可能なプロパティにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="ce3d6-122">**Updateitem**呼び出しを使用すると、1つ以上のアイテム、および各アイテムの1つ以上のプロパティを変更できます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="ce3d6-123">[Itemchanges](itemchanges.md)要素には、この呼び出しの一部として実行されるすべての変更が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="ce3d6-124">[Itemchange](itemchange.md)要素 ( [itemchange](itemchanges.md)要素の子) は、1つのアイテムに対して実行される変更を表します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="ce3d6-125">[Itemchange](itemchange.md)要素には、1つのアイテムに対して実行できる更新アクションのセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="ce3d6-126">これらの変更は、 [Updates (Item)](updates-item.md)要素に含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="ce3d6-127">[ItemId](itemid.md)要素は、更新するアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="ce3d6-128">アイテムで複数のプロパティを更新するには、更新が必要な各プロパティに対して[SetItemField](setitemfield.md)、 [appendtoitemfield](appendtoitemfield.md)、または[deleteitemfield](deleteitemfield.md)を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ce3d6-129">更新操作は、指定された順序で適用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="ce3d6-130">変更ごとに、変更するプロパティのパスと、そのアイテムの新しい値を表す表現を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="ce3d6-131">Delete アクションは、削除する必要のあるプロパティのパスのみが必要になるということとは少し異なります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="ce3d6-132">Set および append アクションの場合、指定されたパスは、アイテム表現で設定されているのと同じプロパティを参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="ce3d6-133">これらが異なる場合は、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="ce3d6-134">**Updateitem**操作は、Exchange ストアアイテムの[開始](start.md)時刻と[終了](end-ex15websvcsotherref.md)時刻を設定できます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="ce3d6-135">**Updateitem**要求では、[終了](end-ex15websvcsotherref.md)時刻を設定することなく、[開始](start.md)時刻を設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="ce3d6-136">これにより、[開始](start.md)時刻が[終了](end-ex15websvcsotherref.md)時刻よりも後の場合にエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="ce3d6-137">期間を保持するために[開始](start.md)時刻が変更された場合、クライアントアプリケーションは[終了](end-ex15websvcsotherref.md)時刻を調整する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="ce3d6-138">1つの予定表アイテムを定期的マスターの予定表アイテムに更新する場合は、予定表アイテムの元のタイムゾーンを保持するために、 **updateitem**操作によって、[会議 timezone](meetingtimezone.md)プロパティを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="ce3d6-139">SetItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="ce3d6-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ce3d6-140">Description</span><span class="sxs-lookup"><span data-stu-id="ce3d6-140">Description</span></span>

<span data-ttu-id="ce3d6-141">次の**updateitem**要求の例は、アイテムに対して [秘密度] プロパティを設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce3d6-142">コード</span><span class="sxs-lookup"><span data-stu-id="ce3d6-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce3d6-143">コメント</span><span class="sxs-lookup"><span data-stu-id="ce3d6-143">Comments</span></span>

<span data-ttu-id="ce3d6-144">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="ce3d6-145">SetItemField Request 要素</span><span class="sxs-lookup"><span data-stu-id="ce3d6-145">SetItemField Request Elements</span></span>

<span data-ttu-id="ce3d6-146">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce3d6-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ce3d6-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ce3d6-148">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ce3d6-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ce3d6-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ce3d6-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ce3d6-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce3d6-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ce3d6-151">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="ce3d6-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ce3d6-152">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ce3d6-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="ce3d6-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ce3d6-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="ce3d6-154">Message</span><span class="sxs-lookup"><span data-stu-id="ce3d6-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ce3d6-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ce3d6-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="ce3d6-156">AppendToItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="ce3d6-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ce3d6-157">Description</span><span class="sxs-lookup"><span data-stu-id="ce3d6-157">Description</span></span>

<span data-ttu-id="ce3d6-158">次の**updateitem**要求の例は、アイテムの body プロパティにテキストを追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce3d6-159">コード</span><span class="sxs-lookup"><span data-stu-id="ce3d6-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce3d6-160">コメント</span><span class="sxs-lookup"><span data-stu-id="ce3d6-160">Comments</span></span>

<span data-ttu-id="ce3d6-161">次のプロパティは、append アクションをサポートします。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="ce3d6-162">**メッセージ: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="ce3d6-163">**アイテム: 本文**</span><span class="sxs-lookup"><span data-stu-id="ce3d6-163">**item:Body**</span></span>
    
- <span data-ttu-id="ce3d6-164">すべての受信者と出席者のコレクションのプロパティ</span><span class="sxs-lookup"><span data-stu-id="ce3d6-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="ce3d6-165">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="ce3d6-166">AppendToItemField Request 要素</span><span class="sxs-lookup"><span data-stu-id="ce3d6-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="ce3d6-167">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce3d6-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ce3d6-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ce3d6-169">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ce3d6-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ce3d6-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ce3d6-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ce3d6-171">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce3d6-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ce3d6-172">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="ce3d6-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ce3d6-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ce3d6-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="ce3d6-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ce3d6-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="ce3d6-175">Message</span><span class="sxs-lookup"><span data-stu-id="ce3d6-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ce3d6-176">Body</span><span class="sxs-lookup"><span data-stu-id="ce3d6-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="ce3d6-177">DeleteItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="ce3d6-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ce3d6-178">Description</span><span class="sxs-lookup"><span data-stu-id="ce3d6-178">Description</span></span>

<span data-ttu-id="ce3d6-179">次の**updateitem**要求の例は、アイテムのプロパティを削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce3d6-180">コード</span><span class="sxs-lookup"><span data-stu-id="ce3d6-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce3d6-181">コメント</span><span class="sxs-lookup"><span data-stu-id="ce3d6-181">Comments</span></span>

<span data-ttu-id="ce3d6-182">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="ce3d6-183">DeleteItemField 要求要素</span><span class="sxs-lookup"><span data-stu-id="ce3d6-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="ce3d6-184">要求では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce3d6-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ce3d6-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ce3d6-186">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ce3d6-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ce3d6-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ce3d6-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ce3d6-188">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce3d6-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ce3d6-189">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="ce3d6-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ce3d6-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ce3d6-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="ce3d6-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ce3d6-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="ce3d6-192">成功した応答の例</span><span class="sxs-lookup"><span data-stu-id="ce3d6-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="ce3d6-193">Description</span><span class="sxs-lookup"><span data-stu-id="ce3d6-193">Description</span></span>

<span data-ttu-id="ce3d6-194">次の例は、 **Updateitem**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce3d6-195">コード</span><span class="sxs-lookup"><span data-stu-id="ce3d6-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce3d6-196">コメント</span><span class="sxs-lookup"><span data-stu-id="ce3d6-196">Comments</span></span>

<span data-ttu-id="ce3d6-197">読みやすくするために、アイテム識別子と変更キーが短縮されています。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ce3d6-198">成功した応答要素</span><span class="sxs-lookup"><span data-stu-id="ce3d6-198">Successful response elements</span></span>

<span data-ttu-id="ce3d6-199">応答では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce3d6-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ce3d6-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce3d6-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce3d6-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce3d6-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="ce3d6-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce3d6-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce3d6-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce3d6-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="ce3d6-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce3d6-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce3d6-205">Items</span><span class="sxs-lookup"><span data-stu-id="ce3d6-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="ce3d6-206">Message</span><span class="sxs-lookup"><span data-stu-id="ce3d6-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ce3d6-207">ItemId</span><span class="sxs-lookup"><span data-stu-id="ce3d6-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="ce3d6-208">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce3d6-208">See also</span></span>



[<span data-ttu-id="ce3d6-209">UpdateItem 操作 (タスク)</span><span class="sxs-lookup"><span data-stu-id="ce3d6-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="ce3d6-210">UpdateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="ce3d6-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="ce3d6-211">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ce3d6-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ce3d6-212">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="ce3d6-212">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="ce3d6-213">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="ce3d6-213">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

