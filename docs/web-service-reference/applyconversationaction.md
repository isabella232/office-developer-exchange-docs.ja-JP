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
description: ApplyConversationAction 要素は、会話内のアイテムにアクションを適用する要求を定義します。
ms.openlocfilehash: 1b672c6e6d2f60e50215417be7100e9cd77e2a58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759413"
---
# <a name="applyconversationaction"></a><span data-ttu-id="d5e4a-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d5e4a-103">ApplyConversationAction</span></span>

<span data-ttu-id="d5e4a-104">**ApplyConversationAction**要素は、会話内のアイテムにアクションを適用する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="d5e4a-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d5e4a-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="d5e4a-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="d5e4a-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5e4a-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d5e4a-107">Attributes and elements</span></span>

<span data-ttu-id="d5e4a-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5e4a-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5e4a-109">Attributes</span></span>

<span data-ttu-id="d5e4a-110">なし。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5e4a-111">子要素</span><span class="sxs-lookup"><span data-stu-id="d5e4a-111">Child elements</span></span>

|<span data-ttu-id="d5e4a-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5e4a-112">**Element**</span></span>|<span data-ttu-id="d5e4a-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5e4a-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5e4a-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="d5e4a-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="d5e4a-115">会話およびそれらに適用するアクションのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5e4a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d5e4a-116">Parent elements</span></span>

<span data-ttu-id="d5e4a-117">なし。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d5e4a-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d5e4a-118">Text value</span></span>

<span data-ttu-id="d5e4a-119">なし。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5e4a-120">備考</span><span class="sxs-lookup"><span data-stu-id="d5e4a-120">Remarks</span></span>

<span data-ttu-id="d5e4a-121">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d5e4a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5e4a-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d5e4a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5e4a-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d5e4a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5e4a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5e4a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d5e4a-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d5e4a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5e4a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5e4a-126">Validation File</span></span>  <br/> |<span data-ttu-id="d5e4a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5e4a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5e4a-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5e4a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5e4a-129">False</span><span class="sxs-lookup"><span data-stu-id="d5e4a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5e4a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5e4a-130">See also</span></span>

- [<span data-ttu-id="d5e4a-131">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="d5e4a-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="d5e4a-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d5e4a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

