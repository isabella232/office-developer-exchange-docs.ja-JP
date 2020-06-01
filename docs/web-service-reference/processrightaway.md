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
description: ProcessRightAway 要素は、アクションがサーバーで処理を開始するとすぐに応答が送信されるか、またはアクションの完了後に応答が送信されるかを示します。 この要素は、要求されたアクションに応答を非同期送信するために存在する必要があります。
ms.openlocfilehash: 58d2b926c48db5e7395df64e1f8ee9d6a8f0e73c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44434072"
---
# <a name="processrightaway"></a><span data-ttu-id="4f0fb-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="4f0fb-104">ProcessRightAway</span></span>

<span data-ttu-id="4f0fb-105">**ProcessRightAway**要素は、アクションがサーバーで処理を開始するとすぐに応答が送信されるか、またはアクションの完了後に応答が送信されるかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="4f0fb-106">この要素は、要求されたアクションに応答を非同期送信するために存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="4f0fb-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4f0fb-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="4f0fb-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="4f0fb-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="4f0fb-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="4f0fb-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="4f0fb-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="4f0fb-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="4f0fb-111">**xs: boolean**</span><span class="sxs-lookup"><span data-stu-id="4f0fb-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f0fb-112">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4f0fb-112">Attributes and elements</span></span>

<span data-ttu-id="4f0fb-113">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f0fb-114">属性</span><span class="sxs-lookup"><span data-stu-id="4f0fb-114">Attributes</span></span>

<span data-ttu-id="4f0fb-115">なし。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f0fb-116">子要素</span><span class="sxs-lookup"><span data-stu-id="4f0fb-116">Child elements</span></span>

<span data-ttu-id="4f0fb-117">なし。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f0fb-118">親要素</span><span class="sxs-lookup"><span data-stu-id="4f0fb-118">Parent elements</span></span>

|<span data-ttu-id="4f0fb-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="4f0fb-119">**Element**</span></span>|<span data-ttu-id="4f0fb-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="4f0fb-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f0fb-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="4f0fb-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="4f0fb-122">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4f0fb-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4f0fb-123">Text value</span></span>

<span data-ttu-id="4f0fb-124">テキスト値が**true の場合**は、アクションがサーバー上で処理を開始するとすぐに応答が送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="4f0fb-125">テキスト値が**false**の場合は、アクションが完了した後に応答が送信されることを示します。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4f0fb-126">注釈</span><span class="sxs-lookup"><span data-stu-id="4f0fb-126">Remarks</span></span>

<span data-ttu-id="4f0fb-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4f0fb-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f0fb-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4f0fb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f0fb-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="4f0fb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f0fb-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4f0fb-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4f0fb-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4f0fb-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f0fb-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4f0fb-132">Validation File</span></span>  <br/> |<span data-ttu-id="4f0fb-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4f0fb-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f0fb-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4f0fb-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f0fb-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="4f0fb-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f0fb-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="4f0fb-136">See also</span></span>



[<span data-ttu-id="4f0fb-137">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="4f0fb-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="4f0fb-138">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4f0fb-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

