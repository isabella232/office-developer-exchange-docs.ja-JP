---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: ConversationNodes 要素は、会話ノードのコレクションを指定します。
ms.openlocfilehash: 39ffb97f1004535e2fc70b58f8d56afe129e8ee2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461395"
---
# <a name="conversationnodes"></a><span data-ttu-id="29ade-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="29ade-103">ConversationNodes</span></span>

<span data-ttu-id="29ade-104">**ConversationNodes**要素は、会話ノードのコレクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="29ade-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="29ade-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="29ade-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29ade-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29ade-106">Attributes and elements</span></span>

<span data-ttu-id="29ade-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29ade-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29ade-108">属性</span><span class="sxs-lookup"><span data-stu-id="29ade-108">Attributes</span></span>

<span data-ttu-id="29ade-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29ade-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29ade-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29ade-110">Child elements</span></span>

|<span data-ttu-id="29ade-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="29ade-111">**Element**</span></span>|<span data-ttu-id="29ade-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="29ade-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29ade-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="29ade-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="29ade-114">スレッド内のノードを指定します。</span><span class="sxs-lookup"><span data-stu-id="29ade-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29ade-115">親要素</span><span class="sxs-lookup"><span data-stu-id="29ade-115">Parent elements</span></span>

|<span data-ttu-id="29ade-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="29ade-116">**Element**</span></span>|<span data-ttu-id="29ade-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="29ade-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29ade-118">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="29ade-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="29ade-119">**GetConversationItems**応答で返される1つの会話を表します。</span><span class="sxs-lookup"><span data-stu-id="29ade-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29ade-120">注釈</span><span class="sxs-lookup"><span data-stu-id="29ade-120">Remarks</span></span>

<span data-ttu-id="29ade-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29ade-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="29ade-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="29ade-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29ade-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29ade-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29ade-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="29ade-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29ade-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29ade-125">Schema Name</span></span>  <br/> |<span data-ttu-id="29ade-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="29ade-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="29ade-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29ade-127">Validation File</span></span>  <br/> |<span data-ttu-id="29ade-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29ade-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="29ade-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="29ade-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="29ade-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="29ade-130">See also</span></span>



- [<span data-ttu-id="29ade-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29ade-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

