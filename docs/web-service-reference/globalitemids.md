---
title: GlobalItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemIds
api_type:
- schema
ms.assetid: b0f03ce0-a4c3-47de-9360-a880a3606e42
description: GlobalItemIds 要素には、メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。
ms.openlocfilehash: 064ebc4c612aaf569eafa56e57a27cf7153f2130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831737"
---
# <a name="globalitemids"></a><span data-ttu-id="4a786-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="4a786-103">GlobalItemIds</span></span>

<span data-ttu-id="4a786-104">**GlobalItemIds**要素には、メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a786-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="4a786-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="4a786-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="4a786-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="4a786-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="4a786-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4a786-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="4a786-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="4a786-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="4a786-109">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="4a786-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a786-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4a786-110">Attributes and elements</span></span>

<span data-ttu-id="4a786-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a786-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a786-112">属性</span><span class="sxs-lookup"><span data-stu-id="4a786-112">Attributes</span></span>

<span data-ttu-id="4a786-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4a786-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a786-114">子要素</span><span class="sxs-lookup"><span data-stu-id="4a786-114">Child elements</span></span>

|<span data-ttu-id="4a786-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a786-115">**Element**</span></span>|<span data-ttu-id="4a786-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a786-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a786-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="4a786-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4a786-118">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a786-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4a786-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="4a786-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="4a786-120">定期的なアイテムの 1 回の発生を識別します。</span><span class="sxs-lookup"><span data-stu-id="4a786-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="4a786-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="4a786-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="4a786-122">関連の出現アイテムの id のいずれかを識別することによって、定期的な予定のマスター アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="4a786-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a786-123">親要素</span><span class="sxs-lookup"><span data-stu-id="4a786-123">Parent elements</span></span>

|<span data-ttu-id="4a786-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a786-124">**Element**</span></span>|<span data-ttu-id="4a786-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a786-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a786-126">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4a786-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="4a786-127">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="4a786-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a786-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a786-128">Text value</span></span>

<span data-ttu-id="4a786-129">なし。</span><span class="sxs-lookup"><span data-stu-id="4a786-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a786-130">備考</span><span class="sxs-lookup"><span data-stu-id="4a786-130">Remarks</span></span>

<span data-ttu-id="4a786-131">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4a786-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a786-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="4a786-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a786-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="4a786-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a786-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a786-134">Schema name</span></span>  <br/> |<span data-ttu-id="4a786-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4a786-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a786-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a786-136">Validation file</span></span>  <br/> |<span data-ttu-id="4a786-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a786-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a786-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a786-138">Can be empty</span></span>  <br/> |<span data-ttu-id="4a786-139">False</span><span class="sxs-lookup"><span data-stu-id="4a786-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a786-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a786-140">See also</span></span>



<span data-ttu-id="4a786-141">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4a786-141">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="4a786-142">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="4a786-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="4a786-143">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="4a786-143">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

