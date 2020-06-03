---
title: 用語
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1a796535-7e83-4aa8-850a-d217059050f8
description: Term 要素は、FindConversation または FindItem 応答で強調表示された用語を指定します。
ms.openlocfilehash: fb102e21d6e7866110735cacd60cd2c3c68a9675
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459491"
---
# <a name="term"></a><span data-ttu-id="ddd9d-103">用語</span><span class="sxs-lookup"><span data-stu-id="ddd9d-103">Term</span></span>

<span data-ttu-id="ddd9d-104">**Term**要素は、 **Findconversation**または**FindItem**応答で強調表示された用語を指定します。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-104">The **Term** element specifies a highlighted term in a **FindConversation** or **FindItem** response.</span></span> 
  
```XML
<Term>
   <Scope/>
   <Value/>
</Term>
```

 <span data-ttu-id="ddd9d-105">**HighlightTermType**</span><span class="sxs-lookup"><span data-stu-id="ddd9d-105">**HighlightTermType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddd9d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ddd9d-106">Attributes and elements</span></span>

<span data-ttu-id="ddd9d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddd9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ddd9d-108">Attributes</span></span>

<span data-ttu-id="ddd9d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddd9d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ddd9d-110">Child elements</span></span>

<span data-ttu-id="ddd9d-111">[範囲 (HighlightTermType)](scope-highlighttermtype.md)  | [値](value.md)</span><span class="sxs-lookup"><span data-stu-id="ddd9d-111">[Scope (HighlightTermType)](scope-highlighttermtype.md) | [Value](value.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddd9d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ddd9d-112">Parent elements</span></span>

[<span data-ttu-id="ddd9d-113">HighlightTerms</span><span class="sxs-lookup"><span data-stu-id="ddd9d-113">HighlightTerms</span></span>](highlightterms.md)
  
## <a name="remarks"></a><span data-ttu-id="ddd9d-114">注釈</span><span class="sxs-lookup"><span data-stu-id="ddd9d-114">Remarks</span></span>

<span data-ttu-id="ddd9d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ddd9d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddd9d-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ddd9d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddd9d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ddd9d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddd9d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ddd9d-119">Schema name</span></span>  <br/> |<span data-ttu-id="ddd9d-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ddd9d-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ddd9d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ddd9d-121">Validation file</span></span>  <br/> |<span data-ttu-id="ddd9d-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ddd9d-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddd9d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ddd9d-123">Can be empty</span></span>  <br/> ||
   

