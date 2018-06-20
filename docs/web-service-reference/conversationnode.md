---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: ConversationNode 要素は、会話内のノードを指定します。
ms.openlocfilehash: c8289e5f30bfd25eb12d54e3be0c561786308dc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759763"
---
# <a name="conversationnode"></a><span data-ttu-id="d083a-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="d083a-103">ConversationNode</span></span>

<span data-ttu-id="d083a-104">**ConversationNode**要素は、会話内のノードを指定します。</span><span class="sxs-lookup"><span data-stu-id="d083a-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="d083a-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="d083a-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d083a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d083a-106">Attributes and elements</span></span>

<span data-ttu-id="d083a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d083a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d083a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d083a-108">Attributes</span></span>

<span data-ttu-id="d083a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d083a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d083a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d083a-110">Child elements</span></span>

|<span data-ttu-id="d083a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d083a-111">**Element**</span></span>|<span data-ttu-id="d083a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d083a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d083a-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="d083a-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="d083a-114">アイテムのインターネット メッセージ id を表します。</span><span class="sxs-lookup"><span data-stu-id="d083a-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="d083a-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="d083a-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="d083a-116">親のインターネット メッセージの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="d083a-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="d083a-117">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="d083a-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="d083a-118">会話ノード内のすべての項目を指定します。</span><span class="sxs-lookup"><span data-stu-id="d083a-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d083a-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d083a-119">Parent elements</span></span>

|<span data-ttu-id="d083a-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d083a-120">**Element**</span></span>|<span data-ttu-id="d083a-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d083a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d083a-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="d083a-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="d083a-123">会話ノードのコレクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="d083a-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d083a-124">備考</span><span class="sxs-lookup"><span data-stu-id="d083a-124">Remarks</span></span>

<span data-ttu-id="d083a-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d083a-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d083a-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d083a-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d083a-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="d083a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d083a-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="d083a-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d083a-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d083a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d083a-130">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d083a-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="d083a-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d083a-131">Validation File</span></span>  <br/> |<span data-ttu-id="d083a-132">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d083a-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d083a-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d083a-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d083a-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="d083a-134">See also</span></span>



- [<span data-ttu-id="d083a-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d083a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

