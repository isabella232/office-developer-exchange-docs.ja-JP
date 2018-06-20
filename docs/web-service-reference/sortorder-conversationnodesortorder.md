---
title: 並べ替え順序 (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: SortOrder 要素は、GetConversationItems 要求の結果の並べ替え順序を指定します。
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833520"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="1b624-103">並べ替え順序 (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="1b624-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="1b624-104">**SortOrder**要素は、 **GetConversationItems**要求の結果の並べ替え順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b624-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="1b624-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="1b624-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b624-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1b624-106">Attributes and elements</span></span>

<span data-ttu-id="1b624-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1b624-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b624-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b624-108">Attributes</span></span>

<span data-ttu-id="1b624-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1b624-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b624-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1b624-110">Child elements</span></span>

<span data-ttu-id="1b624-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1b624-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b624-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1b624-112">Parent elements</span></span>

[<span data-ttu-id="1b624-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="1b624-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="1b624-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1b624-114">Text value</span></span>

<span data-ttu-id="1b624-115">**SortOrder**要素のテキスト値は、会話を注文する順序です。</span><span class="sxs-lookup"><span data-stu-id="1b624-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="1b624-116">**TreeOrderAscending**のテキスト値では、会話が昇順で会話ツリーに基づいて並べられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1b624-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="1b624-117">**TreeOrderDescending**のテキスト値では、会話が降順で会話ツリーに基づいて並べられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1b624-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="1b624-118">**DateOrderAscending**のテキスト値では、会話が昇順での会話の日付に基づいて並べられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1b624-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="1b624-119">**DateOrderDescending**のテキスト値では、会話が降順での会話の日付に基づいて並べられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1b624-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1b624-120">備考</span><span class="sxs-lookup"><span data-stu-id="1b624-120">Remarks</span></span>

<span data-ttu-id="1b624-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1b624-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1b624-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1b624-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b624-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="1b624-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b624-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="1b624-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b624-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1b624-125">Schema name</span></span>  <br/> |<span data-ttu-id="1b624-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1b624-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b624-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1b624-127">Validation file</span></span>  <br/> |<span data-ttu-id="1b624-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b624-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b624-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1b624-129">Can be empty</span></span>  <br/> ||
   

