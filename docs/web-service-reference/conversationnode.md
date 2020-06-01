---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: ConversationNode 要素は、スレッド内のノードを指定します。
ms.openlocfilehash: 074209c1b5669db8dd1ea4ba7f9dea064628afbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462704"
---
# <a name="conversationnode"></a><span data-ttu-id="e8083-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="e8083-103">ConversationNode</span></span>

<span data-ttu-id="e8083-104">**ConversationNode**要素は、スレッド内のノードを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8083-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="e8083-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="e8083-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8083-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8083-106">Attributes and elements</span></span>

<span data-ttu-id="e8083-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8083-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8083-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8083-108">Attributes</span></span>

<span data-ttu-id="e8083-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8083-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8083-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8083-110">Child elements</span></span>

|<span data-ttu-id="e8083-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e8083-111">**Element**</span></span>|<span data-ttu-id="e8083-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8083-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8083-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="e8083-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="e8083-114">アイテムのインターネットメッセージ識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e8083-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="e8083-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="e8083-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="e8083-116">親インターネットメッセージの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e8083-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="e8083-117">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="e8083-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="e8083-118">会話ノード内のすべてのアイテムを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8083-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8083-119">親要素</span><span class="sxs-lookup"><span data-stu-id="e8083-119">Parent elements</span></span>

|<span data-ttu-id="e8083-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8083-120">**Element**</span></span>|<span data-ttu-id="e8083-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8083-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8083-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="e8083-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="e8083-123">会話ノードのコレクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="e8083-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8083-124">注釈</span><span class="sxs-lookup"><span data-stu-id="e8083-124">Remarks</span></span>

<span data-ttu-id="e8083-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8083-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8083-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8083-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8083-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8083-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8083-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8083-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8083-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8083-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e8083-130">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8083-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="e8083-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8083-131">Validation File</span></span>  <br/> |<span data-ttu-id="e8083-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8083-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8083-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8083-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e8083-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8083-134">See also</span></span>



- [<span data-ttu-id="e8083-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e8083-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

