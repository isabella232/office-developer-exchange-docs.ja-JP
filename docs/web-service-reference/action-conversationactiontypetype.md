---
title: アクション (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Action 要素には、ConversationId 要素によって指定された会話に対して実行するアクションが含まれています。
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527545"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="76f6f-103">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="76f6f-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="76f6f-104">**Action**要素には、 [ConversationId](conversationid.md)要素によって指定された会話に対して実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="76f6f-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="76f6f-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="76f6f-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="76f6f-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="76f6f-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="76f6f-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="76f6f-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="76f6f-108">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="76f6f-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="76f6f-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="76f6f-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76f6f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="76f6f-110">Attributes and elements</span></span>

<span data-ttu-id="76f6f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76f6f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76f6f-112">属性</span><span class="sxs-lookup"><span data-stu-id="76f6f-112">Attributes</span></span>

<span data-ttu-id="76f6f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="76f6f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76f6f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="76f6f-114">Child elements</span></span>

<span data-ttu-id="76f6f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="76f6f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76f6f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="76f6f-116">Parent elements</span></span>

|<span data-ttu-id="76f6f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="76f6f-117">**Element**</span></span>|<span data-ttu-id="76f6f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="76f6f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76f6f-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="76f6f-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="76f6f-120">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76f6f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="76f6f-121">Text value</span></span>

<span data-ttu-id="76f6f-122">**Action**要素のテキスト値は、会話に対して実行されるアクションを示します。</span><span class="sxs-lookup"><span data-stu-id="76f6f-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="76f6f-123">可能なテキスト値とそれに対応するアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="76f6f-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="76f6f-124">**AlwaysCategorize** -会話内の現在のアイテムと新しいアイテムは、 [categories](categories-ex15websvcsotherref.md)要素で識別されるカテゴリで自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="76f6f-125">**Always delete** -現在のアイテムとスレッドの新しいアイテムは自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="76f6f-126">削除モードは[Deletetype](deletetype.md)要素によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="76f6f-127">**Always move** -現在のアイテムとスレッド内の新しいアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーに自動的に移動されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="76f6f-128">**Delete** -スレッド内の現在のアイテムは削除されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="76f6f-129">スレッド内の後続のアイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="76f6f-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="76f6f-130">削除モードは[Deletetype](deletetype.md)要素によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="76f6f-131">**Move** -スレッド内の現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="76f6f-132">スレッド内の後続のアイテムは移動されません。</span><span class="sxs-lookup"><span data-stu-id="76f6f-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="76f6f-133">**Copy** -スレッド内の現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素によって識別されるフォルダーにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="76f6f-134">スレッド内の後続のアイテムはコピーされません。</span><span class="sxs-lookup"><span data-stu-id="76f6f-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="76f6f-135">**Setreadstate** -会話内の現在のアイテムの読み取り状態が設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="76f6f-136">読み取り状態は、 [isread](isread.md)要素によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="76f6f-137">**Flag** -スレッド内の現在のアイテムには、 [flag](flag.md)要素で定義されているフラグが設定されます。</span><span class="sxs-lookup"><span data-stu-id="76f6f-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="76f6f-138">注釈</span><span class="sxs-lookup"><span data-stu-id="76f6f-138">Remarks</span></span>

<span data-ttu-id="76f6f-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="76f6f-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76f6f-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="76f6f-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76f6f-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="76f6f-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76f6f-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76f6f-142">Schema Name</span></span>  <br/> |<span data-ttu-id="76f6f-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="76f6f-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="76f6f-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76f6f-144">Validation File</span></span>  <br/> |<span data-ttu-id="76f6f-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="76f6f-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76f6f-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76f6f-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="76f6f-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="76f6f-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76f6f-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="76f6f-148">See also</span></span>

- [<span data-ttu-id="76f6f-149">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="76f6f-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="76f6f-150">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="76f6f-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

