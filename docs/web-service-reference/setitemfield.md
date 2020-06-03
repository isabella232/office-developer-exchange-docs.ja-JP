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
description: SetItemField 要素は、UpdateItem 操作のアイテムの1つのプロパティに対する更新を表します。
ms.openlocfilehash: b4606eb7d94b9d0c4c5bcd5a2b56d73a4d4270cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467425"
---
# <a name="setitemfield"></a><span data-ttu-id="dc1d7-103">SetItemField</span><span class="sxs-lookup"><span data-stu-id="dc1d7-103">SetItemField</span></span>

<span data-ttu-id="dc1d7-104">**SetItemField**要素は、 [updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingRequest/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingResponse/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingRequest/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Task/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Message/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingCancellation/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingRequest/>  
</SetItemField>
```

```xml
<SetItemField>
    <FieldURI/> 
    <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
    <IndexedFieldURI/> 
    <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <DistributionList/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Contact/> 
</SetItemField>
```


<span data-ttu-id="dc1d7-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="dc1d7-105">**SetItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dc1d7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dc1d7-106">Attributes and elements</span></span>

<span data-ttu-id="dc1d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc1d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc1d7-108">Attributes</span></span>

<span data-ttu-id="dc1d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc1d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dc1d7-110">Child elements</span></span>

|<span data-ttu-id="dc1d7-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="dc1d7-111">**Element**</span></span>|<span data-ttu-id="dc1d7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc1d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1d7-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="dc1d7-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="dc1d7-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dc1d7-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="dc1d7-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dc1d7-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="dc1d7-118">設定する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-119">Item</span><span class="sxs-lookup"><span data-stu-id="dc1d7-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="dc1d7-120">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-121">Message</span><span class="sxs-lookup"><span data-stu-id="dc1d7-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dc1d7-122">更新する Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="dc1d7-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="dc1d7-124">更新する Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-125">Contact</span><span class="sxs-lookup"><span data-stu-id="dc1d7-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="dc1d7-126">更新する Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="dc1d7-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="dc1d7-128">更新する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="dc1d7-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="dc1d7-130">更新する会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="dc1d7-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="dc1d7-132">更新する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="dc1d7-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="dc1d7-134">更新する会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="dc1d7-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="dc1d7-136">更新する会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="dc1d7-137">タスク</span><span class="sxs-lookup"><span data-stu-id="dc1d7-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="dc1d7-138">更新するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc1d7-139">親要素</span><span class="sxs-lookup"><span data-stu-id="dc1d7-139">Parent elements</span></span>

|<span data-ttu-id="dc1d7-140">**要素**</span><span class="sxs-lookup"><span data-stu-id="dc1d7-140">**Element**</span></span>|<span data-ttu-id="dc1d7-141">**説明**</span><span class="sxs-lookup"><span data-stu-id="dc1d7-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc1d7-142">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="dc1d7-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="dc1d7-143">アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc1d7-144">注釈</span><span class="sxs-lookup"><span data-stu-id="dc1d7-144">Remarks</span></span>

<span data-ttu-id="dc1d7-145">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc1d7-146">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dc1d7-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc1d7-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc1d7-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc1d7-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dc1d7-148">Schema Name</span></span>  <br/> |<span data-ttu-id="dc1d7-149">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dc1d7-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc1d7-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dc1d7-150">Validation File</span></span>  <br/> |<span data-ttu-id="dc1d7-151">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dc1d7-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc1d7-152">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dc1d7-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc1d7-153">正しくない</span><span class="sxs-lookup"><span data-stu-id="dc1d7-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc1d7-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc1d7-154">See also</span></span>

- [<span data-ttu-id="dc1d7-155">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="dc1d7-155">UpdateItem operation</span></span>](updateitem-operation.md)

