---
title: SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d8c367a-67e9-43b3-8be0-6362d2152431
description: SearchMailboxes ボックス要素は、SearchMailboxes ボックス要求の開始を示します。
ms.openlocfilehash: 7ccc94157ef6bde7b6ba86e70c16ef6e90d712fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456802"
---
# <a name="searchmailboxes"></a><span data-ttu-id="79aa0-103">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="79aa0-103">SearchMailboxes</span></span>

<span data-ttu-id="79aa0-104">**Searchmailboxes**ボックス要素は、 **searchmailboxes ボックス**要求の開始を示します。</span><span class="sxs-lookup"><span data-stu-id="79aa0-104">The **SearchMailboxes** element indicates the beginning of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxes>
   <SearchQueries/>
   <ResultType/>
   <PreviewItemResponseShape/>
   <SortBy/>
   <Language/>
   <Deduplication/>
   <PageSize/>
   <PageItemReference/>
   <PageDirection/>
</SearchMailboxes>
```

 <span data-ttu-id="79aa0-105">**SearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="79aa0-105">**SearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79aa0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="79aa0-106">Attributes and elements</span></span>

<span data-ttu-id="79aa0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="79aa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79aa0-108">属性</span><span class="sxs-lookup"><span data-stu-id="79aa0-108">Attributes</span></span>

<span data-ttu-id="79aa0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="79aa0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79aa0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="79aa0-110">Child elements</span></span>

<span data-ttu-id="79aa0-111">[Searchqueries](searchqueries.md)  | [ResultType](resulttype.md)  | [プレビュー Itemresponseshape](previewitemresponseshape.md)  | [SortBy](sortby.md)  | [言語](language.md)  | [重複除去](deduplication.md)  | [PageSize](pagesize.md)  | [Pageitemreference](pageitemreference.md)  | [ページの方向](pagedirection.md)</span><span class="sxs-lookup"><span data-stu-id="79aa0-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [SortBy](sortby.md) | [Language](language.md) | [Deduplication](deduplication.md) | [PageSize](pagesize.md) | [PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79aa0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="79aa0-112">Parent elements</span></span>

<span data-ttu-id="79aa0-113">なし。</span><span class="sxs-lookup"><span data-stu-id="79aa0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79aa0-114">注釈</span><span class="sxs-lookup"><span data-stu-id="79aa0-114">Remarks</span></span>

<span data-ttu-id="79aa0-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="79aa0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="79aa0-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="79aa0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79aa0-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="79aa0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79aa0-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="79aa0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="79aa0-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="79aa0-119">Schema name</span></span>  <br/> |<span data-ttu-id="79aa0-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="79aa0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="79aa0-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="79aa0-121">Validation file</span></span>  <br/> |<span data-ttu-id="79aa0-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="79aa0-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="79aa0-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="79aa0-123">Can be empty</span></span>  <br/> |<span data-ttu-id="79aa0-124">false</span><span class="sxs-lookup"><span data-stu-id="79aa0-124">false</span></span>  <br/> |
   

