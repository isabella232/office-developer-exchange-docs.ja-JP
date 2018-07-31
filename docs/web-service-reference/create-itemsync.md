---
title: Create (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: 作成要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。
ms.openlocfilehash: d49e54c64f7bd53dcb296d998a856c20570d81be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353946"
---
# <a name="create-itemsync"></a><span data-ttu-id="ec6ab-103">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ec6ab-103">Create (ItemSync)</span></span>

<span data-ttu-id="ec6ab-104">**作成**要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
- [<span data-ttu-id="ec6ab-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="ec6ab-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="ec6ab-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec6ab-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="ec6ab-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec6ab-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) 
- [<span data-ttu-id="ec6ab-108">Changes (Items)</span><span class="sxs-lookup"><span data-stu-id="ec6ab-108">Changes (Items)</span></span>](changes-items.md) 
- [<span data-ttu-id="ec6ab-109">Create (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="ec6ab-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

<span data-ttu-id="ec6ab-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="ec6ab-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ec6ab-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ec6ab-111">Attributes and elements</span></span>

<span data-ttu-id="ec6ab-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec6ab-113">属性</span><span class="sxs-lookup"><span data-stu-id="ec6ab-113">Attributes</span></span>

<span data-ttu-id="ec6ab-114">なし。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec6ab-115">子要素</span><span class="sxs-lookup"><span data-stu-id="ec6ab-115">Child elements</span></span>

|<span data-ttu-id="ec6ab-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="ec6ab-116">**Element**</span></span>|<span data-ttu-id="ec6ab-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec6ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec6ab-118">Item</span><span class="sxs-lookup"><span data-stu-id="ec6ab-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="ec6ab-119">作成する一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-120">Message</span><span class="sxs-lookup"><span data-stu-id="ec6ab-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ec6ab-121">作成する Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ec6ab-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ec6ab-123">作成するのには、Exchange 予定表のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-124">連絡先</span><span class="sxs-lookup"><span data-stu-id="ec6ab-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ec6ab-125">Exchange 連絡先を作成する項目を表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="ec6ab-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="ec6ab-127">作成する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ec6ab-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ec6ab-129">会議を作成するメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ec6ab-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ec6ab-131">作成する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ec6ab-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ec6ab-133">作成する会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ec6ab-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ec6ab-135">作成する会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="ec6ab-136">タスク</span><span class="sxs-lookup"><span data-stu-id="ec6ab-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="ec6ab-137">作成するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec6ab-138">親要素</span><span class="sxs-lookup"><span data-stu-id="ec6ab-138">Parent elements</span></span>

|<span data-ttu-id="ec6ab-139">**要素**</span><span class="sxs-lookup"><span data-stu-id="ec6ab-139">**Element**</span></span>|<span data-ttu-id="ec6ab-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="ec6ab-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec6ab-141">Changes (Items)</span><span class="sxs-lookup"><span data-stu-id="ec6ab-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="ec6ab-142">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ec6ab-143">注釈</span><span class="sxs-lookup"><span data-stu-id="ec6ab-143">Remarks</span></span>

<span data-ttu-id="ec6ab-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec6ab-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="ec6ab-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec6ab-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="ec6ab-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec6ab-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ec6ab-147">Schema name</span></span>  <br/> |<span data-ttu-id="ec6ab-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ec6ab-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec6ab-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ec6ab-149">Validation file</span></span>  <br/> |<span data-ttu-id="ec6ab-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ec6ab-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec6ab-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ec6ab-151">Can be empty</span></span>  <br/> |<span data-ttu-id="ec6ab-152">False</span><span class="sxs-lookup"><span data-stu-id="ec6ab-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec6ab-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="ec6ab-153">See also</span></span>

- [<span data-ttu-id="ec6ab-154">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="ec6ab-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="ec6ab-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ec6ab-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

