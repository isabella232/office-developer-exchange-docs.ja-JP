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
description: GlobalItemIds 要素には、メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。
ms.openlocfilehash: aa656e7f2fb78dafe5bf6013c1f7ad14e2372ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459427"
---
# <a name="globalitemids"></a><span data-ttu-id="9a409-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="9a409-103">GlobalItemIds</span></span>

<span data-ttu-id="9a409-104">**Globalitemids**要素には、メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a409-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="9a409-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="9a409-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="9a409-106">会話</span><span class="sxs-lookup"><span data-stu-id="9a409-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="9a409-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="9a409-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="9a409-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="9a409-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="9a409-109">**非 Emptyarrayofbaseitemidstype**</span><span class="sxs-lookup"><span data-stu-id="9a409-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a409-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9a409-110">Attributes and elements</span></span>

<span data-ttu-id="9a409-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a409-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a409-112">属性</span><span class="sxs-lookup"><span data-stu-id="9a409-112">Attributes</span></span>

<span data-ttu-id="9a409-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9a409-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a409-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9a409-114">Child elements</span></span>

|<span data-ttu-id="9a409-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="9a409-115">**Element**</span></span>|<span data-ttu-id="9a409-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a409-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a409-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="9a409-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9a409-118">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a409-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9a409-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="9a409-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="9a409-120">定期的なアイテムの1回の出現を識別します。</span><span class="sxs-lookup"><span data-stu-id="9a409-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="9a409-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="9a409-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="9a409-122">関連するオカレンスアイテムの識別子の1つを識別することによって、定期的なアイテムのマスターアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="9a409-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a409-123">親要素</span><span class="sxs-lookup"><span data-stu-id="9a409-123">Parent elements</span></span>

|<span data-ttu-id="9a409-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a409-124">**Element**</span></span>|<span data-ttu-id="9a409-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a409-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a409-126">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="9a409-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="9a409-127">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="9a409-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a409-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9a409-128">Text value</span></span>

<span data-ttu-id="9a409-129">なし。</span><span class="sxs-lookup"><span data-stu-id="9a409-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a409-130">注釈</span><span class="sxs-lookup"><span data-stu-id="9a409-130">Remarks</span></span>

<span data-ttu-id="9a409-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9a409-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a409-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9a409-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a409-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a409-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a409-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a409-134">Schema name</span></span>  <br/> |<span data-ttu-id="9a409-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9a409-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a409-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a409-136">Validation file</span></span>  <br/> |<span data-ttu-id="9a409-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9a409-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a409-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9a409-138">Can be empty</span></span>  <br/> |<span data-ttu-id="9a409-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="9a409-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a409-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a409-140">See also</span></span>



[<span data-ttu-id="9a409-141">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="9a409-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="9a409-142">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="9a409-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="9a409-143">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="9a409-143">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

