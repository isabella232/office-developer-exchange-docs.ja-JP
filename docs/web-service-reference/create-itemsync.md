---
title: (ItemSync) を作成します。
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
ms.openlocfilehash: 39056bcaab3577b1b729421118a45571910922fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759795"
---
# <a name="create-itemsync"></a><span data-ttu-id="43880-103">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="43880-103">Create (ItemSync)</span></span>

<span data-ttu-id="43880-104">**作成**要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="43880-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
[<span data-ttu-id="43880-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="43880-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="43880-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="43880-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="43880-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="43880-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="43880-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="43880-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="43880-109">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="43880-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 <span data-ttu-id="43880-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="43880-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43880-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="43880-111">Attributes and elements</span></span>

<span data-ttu-id="43880-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="43880-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43880-113">属性</span><span class="sxs-lookup"><span data-stu-id="43880-113">Attributes</span></span>

<span data-ttu-id="43880-114">なし。</span><span class="sxs-lookup"><span data-stu-id="43880-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43880-115">子要素</span><span class="sxs-lookup"><span data-stu-id="43880-115">Child elements</span></span>

|<span data-ttu-id="43880-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="43880-116">**Element**</span></span>|<span data-ttu-id="43880-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="43880-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43880-118">Item</span><span class="sxs-lookup"><span data-stu-id="43880-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="43880-119">作成する一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-120">Message</span><span class="sxs-lookup"><span data-stu-id="43880-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="43880-121">作成する Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-122">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="43880-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="43880-123">作成するのには、Exchange 予定表のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-124">Contact</span><span class="sxs-lookup"><span data-stu-id="43880-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="43880-125">Exchange 連絡先を作成する項目を表します。</span><span class="sxs-lookup"><span data-stu-id="43880-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="43880-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="43880-127">作成する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="43880-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="43880-129">会議を作成するメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="43880-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="43880-131">作成する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="43880-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="43880-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="43880-133">作成する会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="43880-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="43880-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="43880-135">作成する会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="43880-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="43880-136">タスク</span><span class="sxs-lookup"><span data-stu-id="43880-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="43880-137">作成するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="43880-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43880-138">親要素</span><span class="sxs-lookup"><span data-stu-id="43880-138">Parent elements</span></span>

|<span data-ttu-id="43880-139">**要素**</span><span class="sxs-lookup"><span data-stu-id="43880-139">**Element**</span></span>|<span data-ttu-id="43880-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="43880-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43880-141">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="43880-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="43880-142">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="43880-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43880-143">備考</span><span class="sxs-lookup"><span data-stu-id="43880-143">Remarks</span></span>

<span data-ttu-id="43880-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="43880-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43880-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="43880-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43880-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="43880-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43880-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="43880-147">Schema name</span></span>  <br/> |<span data-ttu-id="43880-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="43880-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="43880-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="43880-149">Validation file</span></span>  <br/> |<span data-ttu-id="43880-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43880-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43880-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="43880-151">Can be empty</span></span>  <br/> |<span data-ttu-id="43880-152">False</span><span class="sxs-lookup"><span data-stu-id="43880-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43880-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="43880-153">See also</span></span>



[<span data-ttu-id="43880-154">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="43880-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="43880-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="43880-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

