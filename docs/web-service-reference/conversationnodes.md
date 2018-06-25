---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: ConversationNodes 要素は、会話のノードのコレクションを指定します。
ms.openlocfilehash: 62ec061f6d03abb9db7e511722e5570e70d65772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759772"
---
# <a name="conversationnodes"></a><span data-ttu-id="78623-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="78623-103">ConversationNodes</span></span>

<span data-ttu-id="78623-104">**ConversationNodes**要素は、会話のノードのコレクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="78623-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="78623-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="78623-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78623-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="78623-106">Attributes and elements</span></span>

<span data-ttu-id="78623-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="78623-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78623-108">属性</span><span class="sxs-lookup"><span data-stu-id="78623-108">Attributes</span></span>

<span data-ttu-id="78623-109">なし。</span><span class="sxs-lookup"><span data-stu-id="78623-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78623-110">子要素</span><span class="sxs-lookup"><span data-stu-id="78623-110">Child elements</span></span>

|<span data-ttu-id="78623-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="78623-111">**Element**</span></span>|<span data-ttu-id="78623-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="78623-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78623-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="78623-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="78623-114">会話] ウィンドウでノードを指定します。</span><span class="sxs-lookup"><span data-stu-id="78623-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78623-115">親要素</span><span class="sxs-lookup"><span data-stu-id="78623-115">Parent elements</span></span>

|<span data-ttu-id="78623-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="78623-116">**Element**</span></span>|<span data-ttu-id="78623-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="78623-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78623-118">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="78623-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="78623-119">**GetConversationItems**応答で返される 1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="78623-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78623-120">備考</span><span class="sxs-lookup"><span data-stu-id="78623-120">Remarks</span></span>

<span data-ttu-id="78623-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="78623-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="78623-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="78623-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78623-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="78623-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78623-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="78623-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78623-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="78623-125">Schema Name</span></span>  <br/> |<span data-ttu-id="78623-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="78623-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="78623-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="78623-127">Validation File</span></span>  <br/> |<span data-ttu-id="78623-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="78623-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="78623-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="78623-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="78623-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="78623-130">See also</span></span>



- [<span data-ttu-id="78623-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="78623-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

