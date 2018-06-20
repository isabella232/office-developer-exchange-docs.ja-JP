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
description: UpdateItem 操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839865"
---
# <a name="updateitem-operation"></a><span data-ttu-id="598d2-103">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="598d2-103">UpdateItem operation</span></span>

<span data-ttu-id="598d2-104">**UpdateItem**操作を使用して、Exchange ストア内の既存のアイテムのプロパティを変更します。</span><span class="sxs-lookup"><span data-stu-id="598d2-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="598d2-105">備考</span><span class="sxs-lookup"><span data-stu-id="598d2-105">Remarks</span></span>

<span data-ttu-id="598d2-106">項目を次の 3 つの基本的な更新操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="598d2-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="598d2-107">次の表は、実行できるアクションを示します。</span><span class="sxs-lookup"><span data-stu-id="598d2-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="598d2-108">**アクション**</span><span class="sxs-lookup"><span data-stu-id="598d2-108">**Action**</span></span>|<span data-ttu-id="598d2-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="598d2-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="598d2-110">追加</span><span class="sxs-lookup"><span data-stu-id="598d2-110">Append</span></span>  <br/> |<span data-ttu-id="598d2-111">データを既存のプロパティに追加します。</span><span class="sxs-lookup"><span data-stu-id="598d2-111">Adds data to an existing property.</span></span> <span data-ttu-id="598d2-112">このアクションは、現在のデータを保持します。</span><span class="sxs-lookup"><span data-stu-id="598d2-112">This action preserves the current data.</span></span> <span data-ttu-id="598d2-113">追加のすべてのプロパティには適用されません。</span><span class="sxs-lookup"><span data-stu-id="598d2-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="598d2-114">設定</span><span class="sxs-lookup"><span data-stu-id="598d2-114">Set</span></span>  <br/> |<span data-ttu-id="598d2-115">プロパティは、データ、または、プロパティを作成し、プロパティが存在しない場合、その値を設定する場合は、プロパティのデータを置き換えます。</span><span class="sxs-lookup"><span data-stu-id="598d2-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="598d2-116">アクションのセットは、書き込み可能なプロパティに適用できるのみです。</span><span class="sxs-lookup"><span data-stu-id="598d2-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="598d2-117">削除</span><span class="sxs-lookup"><span data-stu-id="598d2-117">Delete</span></span>  <br/> |<span data-ttu-id="598d2-118">アイテムからプロパティを削除します。</span><span class="sxs-lookup"><span data-stu-id="598d2-118">Removes a property from an item.</span></span> <span data-ttu-id="598d2-119">これは、空の値をプロパティの設定によって異なります。</span><span class="sxs-lookup"><span data-stu-id="598d2-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="598d2-120">この操作が完了したら、プロパティは項目には存在しません。</span><span class="sxs-lookup"><span data-stu-id="598d2-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="598d2-121">削除は、書き込み可能なプロパティに該当する場合のみです。</span><span class="sxs-lookup"><span data-stu-id="598d2-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="598d2-122">**UpdateItem**呼び出しは、1 つまたは複数の項目と各項目の 1 つまたは複数のプロパティを変更するのには使用できます。</span><span class="sxs-lookup"><span data-stu-id="598d2-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="598d2-123">[ItemChanges](itemchanges.md)要素には、この呼び出しの一部として実行されるすべての変更が含まれています。</span><span class="sxs-lookup"><span data-stu-id="598d2-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="598d2-124">[ItemChange](itemchange.md)の要素、 [ItemChanges](itemchanges.md)の要素の子では、1 つのアイテムに対して実行できる変更を表します。</span><span class="sxs-lookup"><span data-stu-id="598d2-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="598d2-125">[ItemChange](itemchange.md)要素には、1 つのアイテムに対して実行できる更新操作のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="598d2-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="598d2-126">[(項目) の更新プログラム](updates-item.md)の要素では、これらの変更が含まれています。</span><span class="sxs-lookup"><span data-stu-id="598d2-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="598d2-127">[アイテム Id](itemid.md)要素は、更新する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="598d2-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="598d2-128">アイテムの 1 つ以上のプロパティを更新するには、 [SetItemField](setitemfield.md)、 [AppendToItemField](appendtoitemfield.md)、または[DeleteItemField](deleteitemfield.md)を更新プログラムを必要とするプロパティごとに指定してください。</span><span class="sxs-lookup"><span data-stu-id="598d2-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="598d2-129">更新アクションは、指定されている順序で適用されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="598d2-130">それぞれの変更の新しい値で変更するプロパティのパスと、その項目の表現を指定する必要です。</span><span class="sxs-lookup"><span data-stu-id="598d2-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="598d2-131">削除アクションは、削除するプロパティのパスのみが必要な点で多少異なります。</span><span class="sxs-lookup"><span data-stu-id="598d2-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="598d2-132">一連のアクションを追加しは、指定されているパスは、品目の表示に設定されている同じプロパティを参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="598d2-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="598d2-133">これらが異なる場合、エラーが戻されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="598d2-134">**UpdateItem**操作は、Exchange ストアの項目の[開始](start.md)と[終了](end-ex15websvcsotherref.md)時間を設定できます。</span><span class="sxs-lookup"><span data-stu-id="598d2-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="598d2-135">**UpdateItem**要求では、[[終了](end-ex15websvcsotherref.md)時刻を設定せず、[開始](start.md)時刻を設定できます。</span><span class="sxs-lookup"><span data-stu-id="598d2-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="598d2-136">[開始](start.md)時刻は[終了](end-ex15websvcsotherref.md)時刻より後の場合は、エラーが発生することができます。</span><span class="sxs-lookup"><span data-stu-id="598d2-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="598d2-137">クライアント アプリケーションが、期間を保持するために[開始](start.md)時刻が変更されたときの[終了](end-ex15websvcsotherref.md)時刻を調整する必要があります。</span><span class="sxs-lookup"><span data-stu-id="598d2-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="598d2-138">マスターの予定表の定期的なアイテムを 1 つの予定表アイテムが更新されると、予定表アイテムの元のタイム ゾーンを保持するために**UpdateItem**操作で[MeetingTimeZone](meetingtimezone.md)プロパティを設定しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="598d2-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="598d2-139">SetItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="598d2-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="598d2-140">説明</span><span class="sxs-lookup"><span data-stu-id="598d2-140">Description</span></span>

<span data-ttu-id="598d2-141">**UpdateItem**要求の次の使用例は、アイテムの秘密度のプロパティを設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="598d2-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="598d2-142">コード</span><span class="sxs-lookup"><span data-stu-id="598d2-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="598d2-143">コメント</span><span class="sxs-lookup"><span data-stu-id="598d2-143">Comments</span></span>

<span data-ttu-id="598d2-144">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="598d2-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="598d2-145">SetItemField 要求の要素</span><span class="sxs-lookup"><span data-stu-id="598d2-145">SetItemField Request Elements</span></span>

<span data-ttu-id="598d2-146">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="598d2-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="598d2-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="598d2-148">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="598d2-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="598d2-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="598d2-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="598d2-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="598d2-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="598d2-151">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="598d2-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="598d2-152">SetItemField</span><span class="sxs-lookup"><span data-stu-id="598d2-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="598d2-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="598d2-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="598d2-154">Message</span><span class="sxs-lookup"><span data-stu-id="598d2-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="598d2-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="598d2-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="598d2-156">AppendToItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="598d2-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="598d2-157">説明</span><span class="sxs-lookup"><span data-stu-id="598d2-157">Description</span></span>

<span data-ttu-id="598d2-158">**UpdateItem**要求の次の例では、アイテムの body プロパティにテキストを追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="598d2-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="598d2-159">コード</span><span class="sxs-lookup"><span data-stu-id="598d2-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="598d2-160">コメント</span><span class="sxs-lookup"><span data-stu-id="598d2-160">Comments</span></span>

<span data-ttu-id="598d2-161">次のプロパティは、追加操作をサポートします。</span><span class="sxs-lookup"><span data-stu-id="598d2-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="598d2-162">**メッセージ: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="598d2-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="598d2-163">**アイテムの本文:**</span><span class="sxs-lookup"><span data-stu-id="598d2-163">**item:Body**</span></span>
    
- <span data-ttu-id="598d2-164">すべての出席者と受信者コレクションのプロパティ</span><span class="sxs-lookup"><span data-stu-id="598d2-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="598d2-165">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="598d2-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="598d2-166">AppendToItemField 要求の要素</span><span class="sxs-lookup"><span data-stu-id="598d2-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="598d2-167">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="598d2-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="598d2-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="598d2-169">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="598d2-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="598d2-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="598d2-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="598d2-171">ItemId</span><span class="sxs-lookup"><span data-stu-id="598d2-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="598d2-172">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="598d2-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="598d2-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="598d2-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="598d2-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="598d2-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="598d2-175">Message</span><span class="sxs-lookup"><span data-stu-id="598d2-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="598d2-176">Body/本文</span><span class="sxs-lookup"><span data-stu-id="598d2-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="598d2-177">DeleteItemField 要求の例</span><span class="sxs-lookup"><span data-stu-id="598d2-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="598d2-178">説明</span><span class="sxs-lookup"><span data-stu-id="598d2-178">Description</span></span>

<span data-ttu-id="598d2-179">**UpdateItem**要求の次の例では、アイテムのプロパティを削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="598d2-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="598d2-180">コード</span><span class="sxs-lookup"><span data-stu-id="598d2-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="598d2-181">コメント</span><span class="sxs-lookup"><span data-stu-id="598d2-181">Comments</span></span>

<span data-ttu-id="598d2-182">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="598d2-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="598d2-183">DeleteItemField 要求の要素</span><span class="sxs-lookup"><span data-stu-id="598d2-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="598d2-184">次の要素は、要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="598d2-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="598d2-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="598d2-186">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="598d2-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="598d2-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="598d2-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="598d2-188">ItemId</span><span class="sxs-lookup"><span data-stu-id="598d2-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="598d2-189">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="598d2-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="598d2-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="598d2-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="598d2-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="598d2-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="598d2-192">正常な応答の例</span><span class="sxs-lookup"><span data-stu-id="598d2-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="598d2-193">説明</span><span class="sxs-lookup"><span data-stu-id="598d2-193">Description</span></span>

<span data-ttu-id="598d2-194">**UpdateItem**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="598d2-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="598d2-195">コード</span><span class="sxs-lookup"><span data-stu-id="598d2-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="598d2-196">コメント</span><span class="sxs-lookup"><span data-stu-id="598d2-196">Comments</span></span>

<span data-ttu-id="598d2-197">項目の識別子と変更キーは、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="598d2-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="598d2-198">正常な応答の要素</span><span class="sxs-lookup"><span data-stu-id="598d2-198">Successful response elements</span></span>

<span data-ttu-id="598d2-199">次の要素は、応答で使用されます。</span><span class="sxs-lookup"><span data-stu-id="598d2-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="598d2-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="598d2-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="598d2-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="598d2-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="598d2-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="598d2-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="598d2-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="598d2-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="598d2-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="598d2-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="598d2-205">Items</span><span class="sxs-lookup"><span data-stu-id="598d2-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="598d2-206">Message</span><span class="sxs-lookup"><span data-stu-id="598d2-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="598d2-207">ItemId</span><span class="sxs-lookup"><span data-stu-id="598d2-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="598d2-208">関連項目</span><span class="sxs-lookup"><span data-stu-id="598d2-208">See also</span></span>



[<span data-ttu-id="598d2-209">UpdateItem 処理 (タスク)</span><span class="sxs-lookup"><span data-stu-id="598d2-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="598d2-210">UpdateItem 操作 (連絡先)</span><span class="sxs-lookup"><span data-stu-id="598d2-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="598d2-211">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="598d2-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="598d2-212">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="598d2-212">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="598d2-213">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="598d2-213">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

