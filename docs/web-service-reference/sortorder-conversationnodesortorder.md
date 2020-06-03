---
title: ソート順序 (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: 並べ替え要素は、GetConversationItems 要求の結果に使用される並べ替え順序を指定します。
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530966"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="1478a-103">ソート順序 (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="1478a-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="1478a-104">並べ替え**要素は、** **GetConversationItems**要求の結果に使用される並べ替え順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="1478a-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="1478a-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="1478a-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1478a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1478a-106">Attributes and elements</span></span>

<span data-ttu-id="1478a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1478a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1478a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1478a-108">Attributes</span></span>

<span data-ttu-id="1478a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1478a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1478a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1478a-110">Child elements</span></span>

<span data-ttu-id="1478a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1478a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1478a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1478a-112">Parent elements</span></span>

[<span data-ttu-id="1478a-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="1478a-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="1478a-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1478a-114">Text value</span></span>

<span data-ttu-id="1478a-115">**ソート**順序要素のテキスト値は、会話が並べ替えられる順序です。</span><span class="sxs-lookup"><span data-stu-id="1478a-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="1478a-116">**Treeorderascending**のテキスト値は、会話が会話ツリーに従って昇順で並べ替えられることを示します。</span><span class="sxs-lookup"><span data-stu-id="1478a-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="1478a-117">**Treeorderdescending**のテキスト値は、会話が会話ツリーに従って降順に並べ替えられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="1478a-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="1478a-118">**Dateorderascending**のテキスト値は、会話の日付に従って、会話が昇順で並べ替えられることを示します。</span><span class="sxs-lookup"><span data-stu-id="1478a-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="1478a-119">**Dateorderdescending**のテキスト値は、会話の日付に基づいて、会話が降順で並べ替えられることを示します。</span><span class="sxs-lookup"><span data-stu-id="1478a-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1478a-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1478a-120">Remarks</span></span>

<span data-ttu-id="1478a-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1478a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1478a-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1478a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1478a-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1478a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1478a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1478a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1478a-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1478a-125">Schema name</span></span>  <br/> |<span data-ttu-id="1478a-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1478a-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1478a-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1478a-127">Validation file</span></span>  <br/> |<span data-ttu-id="1478a-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1478a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1478a-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1478a-129">Can be empty</span></span>  <br/> ||
   

