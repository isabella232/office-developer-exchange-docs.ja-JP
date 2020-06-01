---
title: ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: e0ee8f30-529b-4d87-8bc0-b6616e75fb6b
description: ApplyConversationAction 要素は、会話内のアイテムにアクションを適用するための要求を定義します。
ms.openlocfilehash: 659b3392778bb1a318c3942a0c8e314f12110c12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461689"
---
# <a name="applyconversationaction"></a><span data-ttu-id="0cf12-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0cf12-103">ApplyConversationAction</span></span>

<span data-ttu-id="0cf12-104">**ApplyConversationAction**要素は、会話内のアイテムにアクションを適用するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0cf12-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="0cf12-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0cf12-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="0cf12-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="0cf12-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cf12-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0cf12-107">Attributes and elements</span></span>

<span data-ttu-id="0cf12-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0cf12-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cf12-109">属性</span><span class="sxs-lookup"><span data-stu-id="0cf12-109">Attributes</span></span>

<span data-ttu-id="0cf12-110">なし。</span><span class="sxs-lookup"><span data-stu-id="0cf12-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cf12-111">子要素</span><span class="sxs-lookup"><span data-stu-id="0cf12-111">Child elements</span></span>

|<span data-ttu-id="0cf12-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="0cf12-112">**Element**</span></span>|<span data-ttu-id="0cf12-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0cf12-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cf12-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="0cf12-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="0cf12-115">会話のコレクションと、それらに適用するアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0cf12-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cf12-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0cf12-116">Parent elements</span></span>

<span data-ttu-id="0cf12-117">なし。</span><span class="sxs-lookup"><span data-stu-id="0cf12-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0cf12-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0cf12-118">Text value</span></span>

<span data-ttu-id="0cf12-119">なし。</span><span class="sxs-lookup"><span data-stu-id="0cf12-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0cf12-120">注釈</span><span class="sxs-lookup"><span data-stu-id="0cf12-120">Remarks</span></span>

<span data-ttu-id="0cf12-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0cf12-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cf12-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0cf12-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cf12-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="0cf12-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0cf12-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0cf12-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0cf12-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0cf12-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0cf12-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0cf12-126">Validation File</span></span>  <br/> |<span data-ttu-id="0cf12-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0cf12-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0cf12-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0cf12-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0cf12-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="0cf12-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0cf12-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="0cf12-130">See also</span></span>

- [<span data-ttu-id="0cf12-131">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="0cf12-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="0cf12-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0cf12-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

