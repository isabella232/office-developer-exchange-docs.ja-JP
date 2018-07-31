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
description: 更新プログラム要素は、ローカル クライアント ストアで更新する 1 つの項目を識別します。
ms.openlocfilehash: bf560f18184151a3f17d7016d05cdb725db934ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353631"
---
# <a name="update-itemsync"></a><span data-ttu-id="d48d4-103">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="d48d4-103">Update (ItemSync)</span></span>

<span data-ttu-id="d48d4-104">**Update**要素は、ローカル クライアント ストアで更新する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="d48d4-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d48d4-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="d48d4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d48d4-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="d48d4-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d48d4-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="d48d4-108">Changes (Items)</span><span class="sxs-lookup"><span data-stu-id="d48d4-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="d48d4-109">Update (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="d48d4-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
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

<span data-ttu-id="d48d4-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="d48d4-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d48d4-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d48d4-111">Attributes and elements</span></span>

<span data-ttu-id="d48d4-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d48d4-113">属性</span><span class="sxs-lookup"><span data-stu-id="d48d4-113">Attributes</span></span>

<span data-ttu-id="d48d4-114">なし。</span><span class="sxs-lookup"><span data-stu-id="d48d4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d48d4-115">子要素</span><span class="sxs-lookup"><span data-stu-id="d48d4-115">Child elements</span></span>

|<span data-ttu-id="d48d4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d48d4-116">**Element**</span></span>|<span data-ttu-id="d48d4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d48d4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d48d4-118">Item</span><span class="sxs-lookup"><span data-stu-id="d48d4-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="d48d4-119">更新するのには、一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-120">Message</span><span class="sxs-lookup"><span data-stu-id="d48d4-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d48d4-121">更新する Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d48d4-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d48d4-123">更新するのには、Exchange 予定表のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-124">連絡先</span><span class="sxs-lookup"><span data-stu-id="d48d4-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d48d4-125">Exchange 連絡先を更新する項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d48d4-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d48d4-127">更新する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d48d4-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d48d4-129">会議を更新するメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d48d4-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d48d4-131">更新する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d48d4-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d48d4-133">更新するのには会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d48d4-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d48d4-135">更新するのには、会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="d48d4-136">タスク</span><span class="sxs-lookup"><span data-stu-id="d48d4-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="d48d4-137">更新するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d48d4-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d48d4-138">親要素</span><span class="sxs-lookup"><span data-stu-id="d48d4-138">Parent elements</span></span>

|<span data-ttu-id="d48d4-139">**要素**</span><span class="sxs-lookup"><span data-stu-id="d48d4-139">**Element**</span></span>|<span data-ttu-id="d48d4-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="d48d4-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d48d4-141">Changes (Items)</span><span class="sxs-lookup"><span data-stu-id="d48d4-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="d48d4-142">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d48d4-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d48d4-143">注釈</span><span class="sxs-lookup"><span data-stu-id="d48d4-143">Remarks</span></span>

<span data-ttu-id="d48d4-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d48d4-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d48d4-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="d48d4-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d48d4-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="d48d4-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d48d4-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d48d4-147">Schema name</span></span>  <br/> |<span data-ttu-id="d48d4-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d48d4-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="d48d4-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d48d4-149">Validation file</span></span>  <br/> |<span data-ttu-id="d48d4-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d48d4-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d48d4-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d48d4-151">Can be empty</span></span>  <br/> |<span data-ttu-id="d48d4-152">False</span><span class="sxs-lookup"><span data-stu-id="d48d4-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d48d4-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="d48d4-153">See also</span></span>

- [<span data-ttu-id="d48d4-154">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="d48d4-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="d48d4-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d48d4-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

