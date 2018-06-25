---
title: SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d8c367a-67e9-43b3-8be0-6362d2152431
description: SearchMailboxes 要素は、SearchMailboxes 要求の先頭を示します。
ms.openlocfilehash: cf8007be3201e2248f27371c2a80c960735a3ced
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833306"
---
# <a name="searchmailboxes"></a><span data-ttu-id="5f770-103">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="5f770-103">SearchMailboxes</span></span>

<span data-ttu-id="5f770-104">**SearchMailboxes**要素は、 **SearchMailboxes**要求の先頭を示します。</span><span class="sxs-lookup"><span data-stu-id="5f770-104">The **SearchMailboxes** element indicates the beginning of the **SearchMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="5f770-105">**SearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="5f770-105">**SearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f770-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5f770-106">Attributes and elements</span></span>

<span data-ttu-id="5f770-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5f770-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f770-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f770-108">Attributes</span></span>

<span data-ttu-id="5f770-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5f770-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f770-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5f770-110">Child elements</span></span>

<span data-ttu-id="5f770-111">[SearchQueries](searchqueries.md) | [結果](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [並べ替え](sortby.md) | [言語](language.md) | [の重複除外](deduplication.md) | [PageSize](pagesize.md)  |  [PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span><span class="sxs-lookup"><span data-stu-id="5f770-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [SortBy](sortby.md) | [Language](language.md) | [Deduplication](deduplication.md) | [PageSize](pagesize.md) | [PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f770-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5f770-112">Parent elements</span></span>

<span data-ttu-id="5f770-113">なし。</span><span class="sxs-lookup"><span data-stu-id="5f770-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f770-114">備考</span><span class="sxs-lookup"><span data-stu-id="5f770-114">Remarks</span></span>

<span data-ttu-id="5f770-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5f770-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5f770-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5f770-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f770-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="5f770-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f770-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="5f770-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5f770-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5f770-119">Schema name</span></span>  <br/> |<span data-ttu-id="5f770-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5f770-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5f770-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5f770-121">Validation file</span></span>  <br/> |<span data-ttu-id="5f770-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5f770-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5f770-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5f770-123">Can be empty</span></span>  <br/> |<span data-ttu-id="5f770-124">false</span><span class="sxs-lookup"><span data-stu-id="5f770-124">false</span></span>  <br/> |
   

