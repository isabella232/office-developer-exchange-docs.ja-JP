---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: SearchScope 要素は、検索のスコープを指定します。
ms.openlocfilehash: 352292952c735e7d3893790a660096c6b6966536
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833315"
---
# <a name="searchscope"></a><span data-ttu-id="ad440-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="ad440-103">SearchScope</span></span>

<span data-ttu-id="ad440-104">**SearchScope**要素は、検索のスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="ad440-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="ad440-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="ad440-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad440-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ad440-106">Attributes and elements</span></span>

<span data-ttu-id="ad440-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ad440-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad440-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad440-108">Attributes</span></span>

<span data-ttu-id="ad440-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ad440-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad440-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ad440-110">Child elements</span></span>

<span data-ttu-id="ad440-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ad440-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad440-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ad440-112">Parent elements</span></span>

[<span data-ttu-id="ad440-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="ad440-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="ad440-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ad440-114">Text value</span></span>

<span data-ttu-id="ad440-115">**SearchScope**要素のテキスト値は、探索検索の検索対象となるメールボックスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ad440-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="ad440-116">**PrimaryOnly**のテキスト値は、プライマリ メールボックスを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="ad440-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="ad440-117">**ArchiveOnly**のテキスト値は、アーカイブ メールボックスを検索することを示します。</span><span class="sxs-lookup"><span data-stu-id="ad440-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="ad440-118">**すべて**のテキスト値を示しますが、両方のプライマリ、アーカイブ メールボックスが検索されます。</span><span class="sxs-lookup"><span data-stu-id="ad440-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ad440-119">備考</span><span class="sxs-lookup"><span data-stu-id="ad440-119">Remarks</span></span>

<span data-ttu-id="ad440-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ad440-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ad440-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ad440-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad440-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="ad440-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad440-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="ad440-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad440-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ad440-124">Schema name</span></span>  <br/> |<span data-ttu-id="ad440-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ad440-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad440-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ad440-126">Validation file</span></span>  <br/> |<span data-ttu-id="ad440-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad440-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad440-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ad440-128">Can be empty</span></span>  <br/> ||
   

