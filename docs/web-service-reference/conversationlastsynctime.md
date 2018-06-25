---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: ConversationLastSyncTime 要素には、会話が最後に同期された日時が含まれています。 この要素は、会話で指定した時刻までに受信したすべてのアイテムを削除しようとするときに存在する必要があります。
ms.openlocfilehash: 3b086d69ac0ef307059df4902e65f796c63733d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759761"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="732fe-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="732fe-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="732fe-105">**ConversationLastSyncTime**要素には、会話が最後に同期された日時が含まれています。</span><span class="sxs-lookup"><span data-stu-id="732fe-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="732fe-106">この要素は、会話で指定した時刻までに受信したすべてのアイテムを削除しようとするときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="732fe-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="732fe-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="732fe-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="732fe-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="732fe-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="732fe-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="732fe-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="732fe-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="732fe-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="732fe-111">**xs:dateTime**</span><span class="sxs-lookup"><span data-stu-id="732fe-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="732fe-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="732fe-112">Attributes and elements</span></span>

<span data-ttu-id="732fe-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="732fe-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="732fe-114">属性</span><span class="sxs-lookup"><span data-stu-id="732fe-114">Attributes</span></span>

<span data-ttu-id="732fe-115">なし。</span><span class="sxs-lookup"><span data-stu-id="732fe-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="732fe-116">子要素</span><span class="sxs-lookup"><span data-stu-id="732fe-116">Child elements</span></span>

<span data-ttu-id="732fe-117">なし。</span><span class="sxs-lookup"><span data-stu-id="732fe-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="732fe-118">親要素</span><span class="sxs-lookup"><span data-stu-id="732fe-118">Parent elements</span></span>

|<span data-ttu-id="732fe-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="732fe-119">**Element**</span></span>|<span data-ttu-id="732fe-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="732fe-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="732fe-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="732fe-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="732fe-122">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="732fe-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="732fe-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="732fe-123">Text value</span></span>

<span data-ttu-id="732fe-124">**ConversationLastSyncTime**のテキスト値は、前回の会話の同期を示します。</span><span class="sxs-lookup"><span data-stu-id="732fe-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="732fe-125">備考</span><span class="sxs-lookup"><span data-stu-id="732fe-125">Remarks</span></span>

<span data-ttu-id="732fe-126">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="732fe-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="732fe-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="732fe-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="732fe-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="732fe-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="732fe-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="732fe-129">Schema Name</span></span>  <br/> |<span data-ttu-id="732fe-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="732fe-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="732fe-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="732fe-131">Validation File</span></span>  <br/> |<span data-ttu-id="732fe-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="732fe-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="732fe-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="732fe-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="732fe-134">False</span><span class="sxs-lookup"><span data-stu-id="732fe-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="732fe-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="732fe-135">See also</span></span>



[<span data-ttu-id="732fe-136">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="732fe-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="732fe-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="732fe-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

