---
title: 用語
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a796535-7e83-4aa8-850a-d217059050f8
description: 用語の要素は、FindConversation または FindItem 応答で強調表示されている用語を指定します。
ms.openlocfilehash: cef2ecd7c51b61ccff2c7261a7a612095047956c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839665"
---
# <a name="term"></a><span data-ttu-id="6a4cc-103">用語</span><span class="sxs-lookup"><span data-stu-id="6a4cc-103">Term</span></span>

<span data-ttu-id="6a4cc-104">**用語**の要素は、 **FindConversation**または**FindItem**応答で強調表示されている用語を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-104">The **Term** element specifies a highlighted term in a **FindConversation** or **FindItem** response.</span></span> 
  
```XML
<Term>
   <Scope/>
   <Value/>
</Term>
```

 <span data-ttu-id="6a4cc-105">**HighlightTermType**</span><span class="sxs-lookup"><span data-stu-id="6a4cc-105">**HighlightTermType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a4cc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6a4cc-106">Attributes and elements</span></span>

<span data-ttu-id="6a4cc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a4cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a4cc-108">Attributes</span></span>

<span data-ttu-id="6a4cc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a4cc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a4cc-110">Child elements</span></span>

<span data-ttu-id="6a4cc-111">[スコープ (HighlightTermType)](scope-highlighttermtype.md) | [の値](value.md)</span><span class="sxs-lookup"><span data-stu-id="6a4cc-111">[Scope (HighlightTermType)](scope-highlighttermtype.md) | [Value](value.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a4cc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6a4cc-112">Parent elements</span></span>

[<span data-ttu-id="6a4cc-113">HighlightTerms</span><span class="sxs-lookup"><span data-stu-id="6a4cc-113">HighlightTerms</span></span>](highlightterms.md)
  
## <a name="remarks"></a><span data-ttu-id="6a4cc-114">備考</span><span class="sxs-lookup"><span data-stu-id="6a4cc-114">Remarks</span></span>

<span data-ttu-id="6a4cc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a4cc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a4cc-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="6a4cc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a4cc-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="6a4cc-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a4cc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a4cc-119">Schema name</span></span>  <br/> |<span data-ttu-id="6a4cc-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6a4cc-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a4cc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a4cc-121">Validation file</span></span>  <br/> |<span data-ttu-id="6a4cc-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a4cc-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a4cc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a4cc-123">Can be empty</span></span>  <br/> ||
   

