---
title: ConversationActions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationActions
api_type:
- schema
ms.assetid: 3d6c663d-4bd9-4eec-b95a-cd683f592672
description: ConversationActions 要素には、会話およびそれらに適用するアクションのコレクションが含まれています。
ms.openlocfilehash: 3dff7ff66f758f1cd2eb3cd7b8126294d2799fc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759757"
---
# <a name="conversationactions"></a><span data-ttu-id="647c4-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="647c4-103">ConversationActions</span></span>

<span data-ttu-id="647c4-104">**ConversationActions**要素には、会話およびそれらに適用するアクションのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="647c4-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="647c4-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="647c4-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="647c4-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="647c4-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="647c4-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="647c4-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="647c4-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="647c4-108">Attributes and elements</span></span>

<span data-ttu-id="647c4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="647c4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="647c4-110">属性</span><span class="sxs-lookup"><span data-stu-id="647c4-110">Attributes</span></span>

<span data-ttu-id="647c4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="647c4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="647c4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="647c4-112">Child elements</span></span>

|<span data-ttu-id="647c4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="647c4-113">**Element**</span></span>|<span data-ttu-id="647c4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="647c4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="647c4-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="647c4-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="647c4-116">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="647c4-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="647c4-117">親要素</span><span class="sxs-lookup"><span data-stu-id="647c4-117">Parent elements</span></span>

|<span data-ttu-id="647c4-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="647c4-118">**Element**</span></span>|<span data-ttu-id="647c4-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="647c4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="647c4-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="647c4-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="647c4-121">会話内のアイテムにアクションを適用する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="647c4-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="647c4-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="647c4-122">Text value</span></span>

<span data-ttu-id="647c4-123">なし。</span><span class="sxs-lookup"><span data-stu-id="647c4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="647c4-124">備考</span><span class="sxs-lookup"><span data-stu-id="647c4-124">Remarks</span></span>

<span data-ttu-id="647c4-125">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="647c4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="647c4-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="647c4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="647c4-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="647c4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="647c4-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="647c4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="647c4-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="647c4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="647c4-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="647c4-130">Validation File</span></span>  <br/> |<span data-ttu-id="647c4-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="647c4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="647c4-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="647c4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="647c4-133">False</span><span class="sxs-lookup"><span data-stu-id="647c4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="647c4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="647c4-134">See also</span></span>



[<span data-ttu-id="647c4-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="647c4-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

