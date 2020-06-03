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
description: ConversationActions 要素には、スレッドのコレクションと、それらに適用するアクションが含まれています。
ms.openlocfilehash: 2db84f78b4b8c92e0a6ef7d69fba7c778fb5f96d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527104"
---
# <a name="conversationactions"></a><span data-ttu-id="683a7-103">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="683a7-103">ConversationActions</span></span>

<span data-ttu-id="683a7-104">**ConversationActions**要素には、スレッドのコレクションと、それらに適用するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="683a7-104">The **ConversationActions** element contains a collection of conversations and the actions to apply to them.</span></span> 
  
[<span data-ttu-id="683a7-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="683a7-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="683a7-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="683a7-106">ConversationActions</span></span>](conversationactions.md)
  
```XML
<ConversationActions>
   <ConversationAction/>
</ConversationActions>
```

 <span data-ttu-id="683a7-107">**NonEmptyArrayOfApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="683a7-107">**NonEmptyArrayOfApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="683a7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="683a7-108">Attributes and elements</span></span>

<span data-ttu-id="683a7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="683a7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="683a7-110">属性</span><span class="sxs-lookup"><span data-stu-id="683a7-110">Attributes</span></span>

<span data-ttu-id="683a7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="683a7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="683a7-112">子要素</span><span class="sxs-lookup"><span data-stu-id="683a7-112">Child elements</span></span>

|<span data-ttu-id="683a7-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="683a7-113">**Element**</span></span>|<span data-ttu-id="683a7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="683a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="683a7-115">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="683a7-115">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="683a7-116">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="683a7-116">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="683a7-117">親要素</span><span class="sxs-lookup"><span data-stu-id="683a7-117">Parent elements</span></span>

|<span data-ttu-id="683a7-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="683a7-118">**Element**</span></span>|<span data-ttu-id="683a7-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="683a7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="683a7-120">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="683a7-120">ApplyConversationAction</span></span>](applyconversationaction.md) <br/> |<span data-ttu-id="683a7-121">会話内のアイテムにアクションを適用するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="683a7-121">Defines a request to apply actions to items in a conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="683a7-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="683a7-122">Text value</span></span>

<span data-ttu-id="683a7-123">なし。</span><span class="sxs-lookup"><span data-stu-id="683a7-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="683a7-124">注釈</span><span class="sxs-lookup"><span data-stu-id="683a7-124">Remarks</span></span>

<span data-ttu-id="683a7-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="683a7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="683a7-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="683a7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="683a7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="683a7-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="683a7-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="683a7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="683a7-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="683a7-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="683a7-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="683a7-130">Validation File</span></span>  <br/> |<span data-ttu-id="683a7-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="683a7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="683a7-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="683a7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="683a7-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="683a7-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="683a7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="683a7-134">See also</span></span>



[<span data-ttu-id="683a7-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="683a7-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

