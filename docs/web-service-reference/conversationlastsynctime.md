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
description: ConversationLastSyncTime 要素には、会話が最後に同期された日時が含まれています。 この要素は、指定された時刻までに受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。
ms.openlocfilehash: f7cc6e205ab9936685d7b8c1f34129b799a53021
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461430"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="42358-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="42358-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="42358-105">**ConversationLastSyncTime**要素には、会話が最後に同期された日時が含まれています。</span><span class="sxs-lookup"><span data-stu-id="42358-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="42358-106">この要素は、指定された時刻までに受信した会話内のすべてのアイテムを削除しようとするときに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="42358-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="42358-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="42358-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="42358-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="42358-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="42358-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="42358-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="42358-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="42358-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="42358-111">**xs: dateTime**</span><span class="sxs-lookup"><span data-stu-id="42358-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42358-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="42358-112">Attributes and elements</span></span>

<span data-ttu-id="42358-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="42358-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42358-114">属性</span><span class="sxs-lookup"><span data-stu-id="42358-114">Attributes</span></span>

<span data-ttu-id="42358-115">なし。</span><span class="sxs-lookup"><span data-stu-id="42358-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42358-116">子要素</span><span class="sxs-lookup"><span data-stu-id="42358-116">Child elements</span></span>

<span data-ttu-id="42358-117">なし。</span><span class="sxs-lookup"><span data-stu-id="42358-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42358-118">親要素</span><span class="sxs-lookup"><span data-stu-id="42358-118">Parent elements</span></span>

|<span data-ttu-id="42358-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="42358-119">**Element**</span></span>|<span data-ttu-id="42358-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="42358-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42358-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="42358-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="42358-122">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="42358-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="42358-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="42358-123">Text value</span></span>

<span data-ttu-id="42358-124">**ConversationLastSyncTime**のテキスト値は、会話が最後に同期された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="42358-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="42358-125">注釈</span><span class="sxs-lookup"><span data-stu-id="42358-125">Remarks</span></span>

<span data-ttu-id="42358-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="42358-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42358-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="42358-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42358-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="42358-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42358-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="42358-129">Schema Name</span></span>  <br/> |<span data-ttu-id="42358-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="42358-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="42358-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="42358-131">Validation File</span></span>  <br/> |<span data-ttu-id="42358-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="42358-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42358-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="42358-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="42358-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="42358-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42358-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="42358-135">See also</span></span>



[<span data-ttu-id="42358-136">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="42358-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="42358-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="42358-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

