---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: SearchItemKind 要素は、FindMailboxStatisticsByKeyword 操作のために検索される項目の種類を示します。
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833298"
---
# <a name="searchitemkind"></a><span data-ttu-id="fa811-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="fa811-103">SearchItemKind</span></span>

<span data-ttu-id="fa811-104">**SearchItemKind**要素は、 **FindMailboxStatisticsByKeyword**操作のために検索される項目の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="fa811-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="fa811-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa811-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fa811-106">Attributes and elements</span></span>

<span data-ttu-id="fa811-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa811-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa811-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa811-108">Attributes</span></span>

<span data-ttu-id="fa811-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fa811-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa811-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fa811-110">Child elements</span></span>

<span data-ttu-id="fa811-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fa811-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa811-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fa811-112">Parent elements</span></span>

[<span data-ttu-id="fa811-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="fa811-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="fa811-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fa811-114">Text value</span></span>

<span data-ttu-id="fa811-115">**SearchItemKind**要素のテキスト値は、キーワードの検索対象となる項目の種類です。</span><span class="sxs-lookup"><span data-stu-id="fa811-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="fa811-116">次の一覧には、 **SearchItemKind**要素で使用できるテキストの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa811-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="fa811-117">**電子メール**には、キーワードは、電子メール メッセージを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-118">**会議**では、キーワードの会議を検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-119">**タスク**では、キーワードは、タスクを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-120">**ノート**には、キーワードの注釈を検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-121">**ドキュメント**では、キーワードのドキュメントを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-122">**仕訳帳**には、キーワードは、仕訳帳を検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-123">**連絡先**には、キーワードの連絡先を検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-124">**Im**のでは、インスタント メッセージのキーワードは検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-125">**ボイスメール**のでは、ボイス ・ メールでキーワードが検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-126">**Fax**には、キーワードは、fax メッセージを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-127">**投稿**を - には、キーワードの投稿を検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="fa811-128">**Rssfeeds**では、キーワードの RSS フィードを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="fa811-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="fa811-129">備考</span><span class="sxs-lookup"><span data-stu-id="fa811-129">Remarks</span></span>

<span data-ttu-id="fa811-130">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fa811-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa811-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fa811-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa811-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="fa811-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa811-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="fa811-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa811-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa811-134">Schema name</span></span>  <br/> |<span data-ttu-id="fa811-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fa811-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa811-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa811-136">Validation file</span></span>  <br/> |<span data-ttu-id="fa811-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa811-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa811-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa811-138">Can be empty</span></span>  <br/> ||
   

