---
title: Update (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: Update 要素は、ローカルクライアントストアで更新する単一のアイテムを識別します。
ms.openlocfilehash: 12248cbbd5d47a19e36d49fcebe6d4753a2e162f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468888"
---
# <a name="update-itemsync"></a><span data-ttu-id="e7db0-103">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e7db0-103">Update (ItemSync)</span></span>

<span data-ttu-id="e7db0-104">**Update**要素は、ローカルクライアントストアで更新する単一のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="e7db0-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="e7db0-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="e7db0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e7db0-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="e7db0-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e7db0-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="e7db0-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="e7db0-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="e7db0-109">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="e7db0-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

<span data-ttu-id="e7db0-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="e7db0-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e7db0-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e7db0-111">Attributes and elements</span></span>

<span data-ttu-id="e7db0-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7db0-113">属性</span><span class="sxs-lookup"><span data-stu-id="e7db0-113">Attributes</span></span>

<span data-ttu-id="e7db0-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e7db0-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7db0-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e7db0-115">Child elements</span></span>

|<span data-ttu-id="e7db0-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="e7db0-116">**Element**</span></span>|<span data-ttu-id="e7db0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7db0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7db0-118">Item</span><span class="sxs-lookup"><span data-stu-id="e7db0-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="e7db0-119">更新する汎用の Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-120">Message</span><span class="sxs-lookup"><span data-stu-id="e7db0-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e7db0-121">更新する Exchange 電子メールメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="e7db0-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e7db0-123">更新する Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-124">Contact</span><span class="sxs-lookup"><span data-stu-id="e7db0-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e7db0-125">更新する Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="e7db0-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="e7db0-127">更新する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e7db0-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="e7db0-129">更新する会議メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e7db0-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e7db0-131">更新する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="e7db0-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="e7db0-133">更新する会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="e7db0-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="e7db0-135">更新する会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="e7db0-136">タスク</span><span class="sxs-lookup"><span data-stu-id="e7db0-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="e7db0-137">更新するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="e7db0-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7db0-138">親要素</span><span class="sxs-lookup"><span data-stu-id="e7db0-138">Parent elements</span></span>

|<span data-ttu-id="e7db0-139">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7db0-139">**Element**</span></span>|<span data-ttu-id="e7db0-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7db0-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7db0-141">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="e7db0-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="e7db0-142">クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列を含みます。</span><span class="sxs-lookup"><span data-stu-id="e7db0-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7db0-143">注釈</span><span class="sxs-lookup"><span data-stu-id="e7db0-143">Remarks</span></span>

<span data-ttu-id="e7db0-144">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e7db0-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7db0-145">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e7db0-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7db0-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7db0-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7db0-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7db0-147">Schema name</span></span>  <br/> |<span data-ttu-id="e7db0-148">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e7db0-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7db0-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7db0-149">Validation file</span></span>  <br/> |<span data-ttu-id="e7db0-150">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e7db0-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7db0-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e7db0-151">Can be empty</span></span>  <br/> |<span data-ttu-id="e7db0-152">正しくない</span><span class="sxs-lookup"><span data-stu-id="e7db0-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7db0-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7db0-153">See also</span></span>

- [<span data-ttu-id="e7db0-154">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="e7db0-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="e7db0-155">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7db0-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

