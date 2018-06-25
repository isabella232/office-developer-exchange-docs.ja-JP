---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: ProcessRightAway 要素は、アクションまたはアクションが完了した後に応答を送信するかどうかの処理を開始するとすぐに応答を送信するかどうかを示します。 この要素は、要求された操作を非同期に送信する応答のために存在する必要があります。
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832898"
---
# <a name="processrightaway"></a><span data-ttu-id="32fcf-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="32fcf-104">ProcessRightAway</span></span>

<span data-ttu-id="32fcf-105">**ProcessRightAway**要素は、アクションまたはアクションが完了した後に応答を送信するかどうかの処理を開始するとすぐに応答を送信するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="32fcf-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="32fcf-106">この要素は、要求された操作を非同期に送信する応答のために存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="32fcf-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="32fcf-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="32fcf-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="32fcf-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="32fcf-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="32fcf-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="32fcf-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="32fcf-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="32fcf-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="32fcf-111">**xs:boolean**</span><span class="sxs-lookup"><span data-stu-id="32fcf-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32fcf-112">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32fcf-112">Attributes and elements</span></span>

<span data-ttu-id="32fcf-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32fcf-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32fcf-114">属性</span><span class="sxs-lookup"><span data-stu-id="32fcf-114">Attributes</span></span>

<span data-ttu-id="32fcf-115">なし。</span><span class="sxs-lookup"><span data-stu-id="32fcf-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32fcf-116">子要素</span><span class="sxs-lookup"><span data-stu-id="32fcf-116">Child elements</span></span>

<span data-ttu-id="32fcf-117">なし。</span><span class="sxs-lookup"><span data-stu-id="32fcf-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32fcf-118">親要素</span><span class="sxs-lookup"><span data-stu-id="32fcf-118">Parent elements</span></span>

|<span data-ttu-id="32fcf-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="32fcf-119">**Element**</span></span>|<span data-ttu-id="32fcf-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="32fcf-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32fcf-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="32fcf-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="32fcf-122">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32fcf-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32fcf-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="32fcf-123">Text value</span></span>

<span data-ttu-id="32fcf-124">**True**の場合、テキスト値は、アクションがサーバー上で処理を開始すると、すぐに応答を送信することを示します。</span><span class="sxs-lookup"><span data-stu-id="32fcf-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="32fcf-125">**False**のテキスト値は、アクションが完了した後に応答を送信することを示します。</span><span class="sxs-lookup"><span data-stu-id="32fcf-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="32fcf-126">備考</span><span class="sxs-lookup"><span data-stu-id="32fcf-126">Remarks</span></span>

<span data-ttu-id="32fcf-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="32fcf-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32fcf-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="32fcf-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32fcf-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="32fcf-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32fcf-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32fcf-130">Schema Name</span></span>  <br/> |<span data-ttu-id="32fcf-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="32fcf-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="32fcf-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32fcf-132">Validation File</span></span>  <br/> |<span data-ttu-id="32fcf-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32fcf-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32fcf-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32fcf-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="32fcf-135">False</span><span class="sxs-lookup"><span data-stu-id="32fcf-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32fcf-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="32fcf-136">See also</span></span>



[<span data-ttu-id="32fcf-137">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="32fcf-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="32fcf-138">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32fcf-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

