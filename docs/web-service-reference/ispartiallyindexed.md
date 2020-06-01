---
title: Ispartiのインデックス付き
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: Isparti"Indexed/インデックス" 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。
ms.openlocfilehash: 4bf0c3e5dd7b75a90ac087958fbceda334306af1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466487"
---
# <a name="ispartiallyindexed"></a><span data-ttu-id="3a12b-103">Ispartiのインデックス付き</span><span class="sxs-lookup"><span data-stu-id="3a12b-103">IsPartiallyIndexed</span></span>

<span data-ttu-id="3a12b-104">**Isparti"indexed/インデックス**" 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3a12b-104">The **IsPartiallyIndexed** element indicates whether the item is partially indexed.</span></span> 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 <span data-ttu-id="3a12b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3a12b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a12b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3a12b-106">Attributes and elements</span></span>

<span data-ttu-id="3a12b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a12b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a12b-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a12b-108">Attributes</span></span>

<span data-ttu-id="3a12b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a12b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a12b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a12b-110">Child elements</span></span>

<span data-ttu-id="3a12b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3a12b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a12b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3a12b-112">Parent elements</span></span>

[<span data-ttu-id="3a12b-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="3a12b-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="3a12b-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3a12b-114">Text value</span></span>

<span data-ttu-id="3a12b-115">**Ispartithe indexed**要素のテキスト値が**true の場合**は、メールボックスアイテムが部分的にインデックス付けされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="3a12b-115">A text value of **true** for the **IsPartiallyIndexed** element indicates that the mailbox item is partially indexed.</span></span> <span data-ttu-id="3a12b-116">値が**false**の場合は、メールボックスアイテムが部分的にインデックス付けされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="3a12b-116">A value of **false** indicates that the mailbox item is not partially indexed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3a12b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="3a12b-117">Remarks</span></span>

<span data-ttu-id="3a12b-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3a12b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a12b-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a12b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a12b-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3a12b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a12b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a12b-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a12b-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a12b-122">Schema name</span></span>  <br/> |<span data-ttu-id="3a12b-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3a12b-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="3a12b-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a12b-124">Validation file</span></span>  <br/> |<span data-ttu-id="3a12b-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3a12b-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a12b-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3a12b-126">Can be empty</span></span>  <br/> |<span data-ttu-id="3a12b-127">false</span><span class="sxs-lookup"><span data-stu-id="3a12b-127">false</span></span>  <br/> |
   

