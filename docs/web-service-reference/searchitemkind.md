---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: SearchItemKind 要素は、FindMailboxStatisticsByKeyword 操作で検索されるアイテムの種類を示します。
ms.openlocfilehash: e0625ac169c3083702494c094da15d38d220fe67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464001"
---
# <a name="searchitemkind"></a><span data-ttu-id="465b3-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="465b3-103">SearchItemKind</span></span>

<span data-ttu-id="465b3-104">**Searchitemkind**要素は、 **FindMailboxStatisticsByKeyword**操作で検索されるアイテムの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="465b3-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="465b3-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="465b3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="465b3-106">Attributes and elements</span></span>

<span data-ttu-id="465b3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="465b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="465b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="465b3-108">Attributes</span></span>

<span data-ttu-id="465b3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="465b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="465b3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="465b3-110">Child elements</span></span>

<span data-ttu-id="465b3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="465b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="465b3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="465b3-112">Parent elements</span></span>

[<span data-ttu-id="465b3-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="465b3-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="465b3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="465b3-114">Text value</span></span>

<span data-ttu-id="465b3-115">**Searchitemkind**要素のテキスト値は、キーワードを検索するアイテムの種類です。</span><span class="sxs-lookup"><span data-stu-id="465b3-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="465b3-116">次のリストには、 **Searchitemkind**要素で使用できるテキスト値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="465b3-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="465b3-117">**Email** -キーワードを検索する電子メールメッセージを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-118">**会議**-キーワードを検索する会議を指定します。</span><span class="sxs-lookup"><span data-stu-id="465b3-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-119">**タスク**-キーワードを検索するタスクを指定します。</span><span class="sxs-lookup"><span data-stu-id="465b3-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-120">**メモ**-キーワードに対して notes が検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-121">**Docs** -ドキュメントがキーワードで検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-122">**ジャーナル**-キーワードに対してジャーナルが検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-123">**連絡先**-キーワードを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-124">**Im** -キーワードを検索するインスタントメッセージを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-125">**ボイスメール**-キーワードに対してボイスメールが検索されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-126">**Fax** -キーワードが検索されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-127">**投稿**-キーワードに対して投稿が検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="465b3-128">**Rssfeeds** -RSS フィードがキーワードに対して検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="465b3-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="465b3-129">注釈</span><span class="sxs-lookup"><span data-stu-id="465b3-129">Remarks</span></span>

<span data-ttu-id="465b3-130">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="465b3-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="465b3-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="465b3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="465b3-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="465b3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="465b3-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="465b3-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="465b3-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="465b3-134">Schema name</span></span>  <br/> |<span data-ttu-id="465b3-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="465b3-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="465b3-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="465b3-136">Validation file</span></span>  <br/> |<span data-ttu-id="465b3-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="465b3-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="465b3-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="465b3-138">Can be empty</span></span>  <br/> ||
   

