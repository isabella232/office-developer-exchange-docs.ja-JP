---
title: IsPartiallyIndexed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: IsPartiallyIndexed 要素は、項目が部分的にインデックスを作成するかどうかを示します。
ms.openlocfilehash: e780fac23aeec1d80e547a47b322073fecdc2a0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832082"
---
# <a name="ispartiallyindexed"></a><span data-ttu-id="c9efe-103">IsPartiallyIndexed</span><span class="sxs-lookup"><span data-stu-id="c9efe-103">IsPartiallyIndexed</span></span>

<span data-ttu-id="c9efe-104">**IsPartiallyIndexed**要素は、項目が部分的にインデックスを作成するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9efe-104">The **IsPartiallyIndexed** element indicates whether the item is partially indexed.</span></span> 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 <span data-ttu-id="c9efe-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c9efe-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9efe-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c9efe-106">Attributes and elements</span></span>

<span data-ttu-id="c9efe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c9efe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9efe-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9efe-108">Attributes</span></span>

<span data-ttu-id="c9efe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c9efe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9efe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c9efe-110">Child elements</span></span>

<span data-ttu-id="c9efe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c9efe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9efe-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c9efe-112">Parent elements</span></span>

[<span data-ttu-id="c9efe-113">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="c9efe-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="c9efe-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c9efe-114">Text value</span></span>

<span data-ttu-id="c9efe-115">の**場合は true** 、 **IsPartiallyIndexed**要素のテキスト値は、メールボックスのアイテムのインデックスは部分的にことを示します。</span><span class="sxs-lookup"><span data-stu-id="c9efe-115">A text value of **true** for the **IsPartiallyIndexed** element indicates that the mailbox item is partially indexed.</span></span> <span data-ttu-id="c9efe-116">**False**の値は、メールボックスのアイテムが部分的に索引付けられないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c9efe-116">A value of **false** indicates that the mailbox item is not partially indexed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9efe-117">備考</span><span class="sxs-lookup"><span data-stu-id="c9efe-117">Remarks</span></span>

<span data-ttu-id="c9efe-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c9efe-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c9efe-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c9efe-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9efe-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="c9efe-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9efe-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="c9efe-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9efe-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c9efe-122">Schema name</span></span>  <br/> |<span data-ttu-id="c9efe-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c9efe-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9efe-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c9efe-124">Validation file</span></span>  <br/> |<span data-ttu-id="c9efe-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9efe-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9efe-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c9efe-126">Can be empty</span></span>  <br/> |<span data-ttu-id="c9efe-127">false</span><span class="sxs-lookup"><span data-stu-id="c9efe-127">false</span></span>  <br/> |
   

