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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759795"
---
# <a name="create-itemsync"></a><span data-ttu-id="eef9d-103">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-103">Create (ItemSync)</span></span>

<span data-ttu-id="eef9d-104">**作成**要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
[<span data-ttu-id="eef9d-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="eef9d-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="eef9d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eef9d-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="eef9d-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eef9d-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="eef9d-108">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="eef9d-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="eef9d-109">(ItemSync) を作成します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 <span data-ttu-id="eef9d-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="eef9d-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eef9d-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eef9d-111">Attributes and elements</span></span>

<span data-ttu-id="eef9d-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eef9d-113">属性</span><span class="sxs-lookup"><span data-stu-id="eef9d-113">Attributes</span></span>

<span data-ttu-id="eef9d-114">なし。</span><span class="sxs-lookup"><span data-stu-id="eef9d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eef9d-115">子要素</span><span class="sxs-lookup"><span data-stu-id="eef9d-115">Child elements</span></span>

|<span data-ttu-id="eef9d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="eef9d-116">**Element**</span></span>|<span data-ttu-id="eef9d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="eef9d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eef9d-118">Item</span><span class="sxs-lookup"><span data-stu-id="eef9d-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="eef9d-119">作成する一般的な Exchange アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-120">Message</span><span class="sxs-lookup"><span data-stu-id="eef9d-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="eef9d-121">作成する Exchange 電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-122">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="eef9d-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="eef9d-123">作成するのには、Exchange 予定表のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-124">Contact</span><span class="sxs-lookup"><span data-stu-id="eef9d-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="eef9d-125">Exchange 連絡先を作成する項目を表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="eef9d-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="eef9d-127">作成する配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="eef9d-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="eef9d-129">会議を作成するメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="eef9d-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="eef9d-131">作成する会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="eef9d-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="eef9d-133">作成する会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="eef9d-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="eef9d-135">作成する会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="eef9d-136">タスク</span><span class="sxs-lookup"><span data-stu-id="eef9d-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="eef9d-137">作成するタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="eef9d-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eef9d-138">親要素</span><span class="sxs-lookup"><span data-stu-id="eef9d-138">Parent elements</span></span>

|<span data-ttu-id="eef9d-139">**要素**</span><span class="sxs-lookup"><span data-stu-id="eef9d-139">**Element**</span></span>|<span data-ttu-id="eef9d-140">**説明**</span><span class="sxs-lookup"><span data-stu-id="eef9d-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eef9d-141">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="eef9d-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="eef9d-142">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eef9d-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eef9d-143">備考</span><span class="sxs-lookup"><span data-stu-id="eef9d-143">Remarks</span></span>

<span data-ttu-id="eef9d-144">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="eef9d-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eef9d-145">要素情報</span><span class="sxs-lookup"><span data-stu-id="eef9d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eef9d-146">名前空間</span><span class="sxs-lookup"><span data-stu-id="eef9d-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eef9d-147">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eef9d-147">Schema name</span></span>  <br/> |<span data-ttu-id="eef9d-148">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="eef9d-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="eef9d-149">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eef9d-149">Validation file</span></span>  <br/> |<span data-ttu-id="eef9d-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eef9d-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eef9d-151">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="eef9d-151">Can be empty</span></span>  <br/> |<span data-ttu-id="eef9d-152">False</span><span class="sxs-lookup"><span data-stu-id="eef9d-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eef9d-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="eef9d-153">See also</span></span>



[<span data-ttu-id="eef9d-154">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="eef9d-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="eef9d-155">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="eef9d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

