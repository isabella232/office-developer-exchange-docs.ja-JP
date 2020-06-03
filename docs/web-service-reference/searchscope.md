---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: SearchScope 要素は、検索範囲を指定します。
ms.openlocfilehash: df11c8db418ac90d1166030aeed3672c0b810052
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466865"
---
# <a name="searchscope"></a><span data-ttu-id="05615-103">SearchScope</span><span class="sxs-lookup"><span data-stu-id="05615-103">SearchScope</span></span>

<span data-ttu-id="05615-104">**Searchscope**要素は、検索範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="05615-104">The **SearchScope** element specifies the scope of a search.</span></span> 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 <span data-ttu-id="05615-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="05615-105">**MailboxSearchLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05615-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="05615-106">Attributes and elements</span></span>

<span data-ttu-id="05615-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05615-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05615-108">属性</span><span class="sxs-lookup"><span data-stu-id="05615-108">Attributes</span></span>

<span data-ttu-id="05615-109">なし。</span><span class="sxs-lookup"><span data-stu-id="05615-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05615-110">子要素</span><span class="sxs-lookup"><span data-stu-id="05615-110">Child elements</span></span>

<span data-ttu-id="05615-111">なし。</span><span class="sxs-lookup"><span data-stu-id="05615-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05615-112">親要素</span><span class="sxs-lookup"><span data-stu-id="05615-112">Parent elements</span></span>

[<span data-ttu-id="05615-113">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="05615-113">MailboxSearchScope</span></span>](mailboxsearchscope.md)
  
## <a name="text-value"></a><span data-ttu-id="05615-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05615-114">Text value</span></span>

<span data-ttu-id="05615-115">**Searchscope**要素のテキスト値は、探索検索を検索するメールボックスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="05615-115">The text value of the **SearchScope** element indicates the mailbox type that is searched for a discovery search.</span></span> <span data-ttu-id="05615-116">Text 値が**Primaryonly**の場合は、プライマリメールボックスが検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="05615-116">A text value of **PrimaryOnly** indicates that the primary mailbox is searched.</span></span> <span data-ttu-id="05615-117">アーカイブのテキスト値は、アーカイブメールボックスが検索される**ことを示し**ます。</span><span class="sxs-lookup"><span data-stu-id="05615-117">A text value of **ArchiveOnly** indicates that the archive mailbox is searched.</span></span> <span data-ttu-id="05615-118">Text 値は、プライマリメールボックスとアーカイブメールボックスの両方が検索さ**れることを示します**。</span><span class="sxs-lookup"><span data-stu-id="05615-118">A text value of **All** indicates that both the primary and archive mailboxes are searched.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="05615-119">注釈</span><span class="sxs-lookup"><span data-stu-id="05615-119">Remarks</span></span>

<span data-ttu-id="05615-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="05615-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="05615-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="05615-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05615-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="05615-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05615-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="05615-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05615-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05615-124">Schema name</span></span>  <br/> |<span data-ttu-id="05615-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="05615-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="05615-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05615-126">Validation file</span></span>  <br/> |<span data-ttu-id="05615-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="05615-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05615-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="05615-128">Can be empty</span></span>  <br/> ||
   

