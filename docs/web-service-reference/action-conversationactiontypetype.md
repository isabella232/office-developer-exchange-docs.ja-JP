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
description: Action 要素には、ConversationId 要素で指定されたスレッド上で実行するアクションが含まれています。
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759265"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="61eae-103">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="61eae-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="61eae-104">**Action**要素には、 [ConversationId](conversationid.md)要素で指定されたスレッド上で実行するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="61eae-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="61eae-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="61eae-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="61eae-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="61eae-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="61eae-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="61eae-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="61eae-108">アクション (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="61eae-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="61eae-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="61eae-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61eae-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="61eae-110">Attributes and elements</span></span>

<span data-ttu-id="61eae-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="61eae-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61eae-112">属性</span><span class="sxs-lookup"><span data-stu-id="61eae-112">Attributes</span></span>

<span data-ttu-id="61eae-113">なし。</span><span class="sxs-lookup"><span data-stu-id="61eae-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61eae-114">子要素</span><span class="sxs-lookup"><span data-stu-id="61eae-114">Child elements</span></span>

<span data-ttu-id="61eae-115">なし。</span><span class="sxs-lookup"><span data-stu-id="61eae-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61eae-116">親要素</span><span class="sxs-lookup"><span data-stu-id="61eae-116">Parent elements</span></span>

|<span data-ttu-id="61eae-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="61eae-117">**Element**</span></span>|<span data-ttu-id="61eae-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="61eae-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61eae-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="61eae-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="61eae-120">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="61eae-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61eae-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="61eae-121">Text value</span></span>

<span data-ttu-id="61eae-122">**Action**要素のテキスト値では、会話するアクションが実行されますを示します。</span><span class="sxs-lookup"><span data-stu-id="61eae-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="61eae-123">可能なテキスト値と対応するアクションを次に示します。</span><span class="sxs-lookup"><span data-stu-id="61eae-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="61eae-124">**AlwaysCategorize** - 現在の項目との会話では、[カテゴリ](categories-ex15websvcsotherref.md)の要素で識別されるカテゴリを使用して自動的に設定されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="61eae-125">**AlwaysDelete** - 現在の項目との会話に新しいアイテムが自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="61eae-126">削除モードは、[削除の種類](deletetype.md)の要素によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="61eae-127">**AlwaysMove** - 現在の項目との会話では、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーに自動的に移動されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="61eae-128">**削除**・ スレッドの現在のアイテムは削除されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="61eae-129">会話でそれ以降の項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="61eae-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="61eae-130">削除モードは、[削除の種類](deletetype.md)の要素によって設定されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="61eae-131">**移動**- スレッドの現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="61eae-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="61eae-132">スレッドのそれ以降のアイテムは移動されません。</span><span class="sxs-lookup"><span data-stu-id="61eae-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="61eae-133">**コピー** - スレッドの現在のアイテムは、 [DestinationFolderId](destinationfolderid.md)要素で指定されたフォルダーにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="61eae-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="61eae-134">スレッドのそれ以降のアイテムはコピーされません。</span><span class="sxs-lookup"><span data-stu-id="61eae-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="61eae-135">**SetReadState**のスレッドの現在のアイテムの読み取り状態の設定があります。</span><span class="sxs-lookup"><span data-stu-id="61eae-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="61eae-136">[IsRead](isread.md)要素によって、読み取りの状態が設定されています。</span><span class="sxs-lookup"><span data-stu-id="61eae-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="61eae-137">**フラグ**スレッドの現在のアイテムは、フラグが設定されている[フラグ](flag.md)の要素で定義されているがあります。</span><span class="sxs-lookup"><span data-stu-id="61eae-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="61eae-138">備考</span><span class="sxs-lookup"><span data-stu-id="61eae-138">Remarks</span></span>

<span data-ttu-id="61eae-139">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="61eae-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61eae-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="61eae-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61eae-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="61eae-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61eae-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="61eae-142">Schema Name</span></span>  <br/> |<span data-ttu-id="61eae-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="61eae-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="61eae-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="61eae-144">Validation File</span></span>  <br/> |<span data-ttu-id="61eae-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="61eae-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61eae-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="61eae-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="61eae-147">False</span><span class="sxs-lookup"><span data-stu-id="61eae-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61eae-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="61eae-148">See also</span></span>

- [<span data-ttu-id="61eae-149">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="61eae-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="61eae-150">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="61eae-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

