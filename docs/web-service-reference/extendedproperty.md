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
description: ExtendedProperty 要素は、フォルダーとアイテムの拡張 MAPI プロパティを識別します。
ms.openlocfilehash: 99ede097d803d6fbf534cde0e77c08cec054bfa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530608"
---
# <a name="extendedproperty"></a><span data-ttu-id="f6019-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f6019-103">ExtendedProperty</span></span>

<span data-ttu-id="f6019-104">**Extendedproperty**要素は、フォルダーとアイテムの拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="f6019-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Value/>
</ExtendedProperty>
```

<span data-ttu-id="f6019-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="f6019-105">**ExtendedPropertyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f6019-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f6019-106">Attributes and elements</span></span>

<span data-ttu-id="f6019-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6019-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6019-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6019-108">Attributes</span></span>

<span data-ttu-id="f6019-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f6019-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6019-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f6019-110">Child elements</span></span>

|<span data-ttu-id="f6019-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f6019-111">**Element**</span></span>|<span data-ttu-id="f6019-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6019-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6019-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f6019-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f6019-114">取得、設定、または作成する拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="f6019-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="f6019-115">値</span><span class="sxs-lookup"><span data-stu-id="f6019-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="f6019-116">複数値を持つ拡張 MAPI プロパティの値のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="f6019-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="f6019-117">値</span><span class="sxs-lookup"><span data-stu-id="f6019-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="f6019-118">単一値の MAPI 拡張プロパティの値を格納します。</span><span class="sxs-lookup"><span data-stu-id="f6019-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6019-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f6019-119">Parent elements</span></span>

|<span data-ttu-id="f6019-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f6019-120">**Element**</span></span>|<span data-ttu-id="f6019-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6019-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6019-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f6019-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f6019-123">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f6019-124">Contact</span><span class="sxs-lookup"><span data-stu-id="f6019-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f6019-125">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="f6019-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f6019-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f6019-127">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f6019-128">Item</span><span class="sxs-lookup"><span data-stu-id="f6019-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="f6019-129">Exchange ストア内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f6019-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f6019-131">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f6019-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f6019-133">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f6019-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f6019-135">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f6019-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f6019-137">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-138">Message</span><span class="sxs-lookup"><span data-stu-id="f6019-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6019-139">Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f6019-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="f6019-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="f6019-141">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="f6019-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-142">タスク</span><span class="sxs-lookup"><span data-stu-id="f6019-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="f6019-143">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f6019-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="f6019-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="f6019-145">主に予定表アイテムを含むフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="f6019-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="f6019-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="f6019-147">メールボックス内の連絡先フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6019-148">Folder</span><span class="sxs-lookup"><span data-stu-id="f6019-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="f6019-149">作成、取得、検索、同期、更新を行うフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="f6019-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f6019-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f6019-151">メールボックスに含まれている検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6019-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="f6019-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="f6019-153">メールボックスに含まれる tasks フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="f6019-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6019-154">注釈</span><span class="sxs-lookup"><span data-stu-id="f6019-154">Remarks</span></span>

<span data-ttu-id="f6019-155">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="f6019-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6019-156">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f6019-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6019-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6019-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6019-158">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6019-158">Schema Name</span></span>  <br/> |<span data-ttu-id="f6019-159">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f6019-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6019-160">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6019-160">Validation File</span></span>  <br/> |<span data-ttu-id="f6019-161">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f6019-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6019-162">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f6019-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6019-163">正しくない</span><span class="sxs-lookup"><span data-stu-id="f6019-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6019-164">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6019-164">See also</span></span>

- [<span data-ttu-id="f6019-165">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f6019-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

