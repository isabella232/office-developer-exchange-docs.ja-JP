---
title: 重複除外
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: 重複要素は、検索結果が重複する項目を削除する必要があるかどうかを示します。
ms.openlocfilehash: 3f06bb1dccd0677b7fd43c4ad82eda54a0c3f812
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759949"
---
# <a name="deduplication"></a><span data-ttu-id="243c7-103">重複除外</span><span class="sxs-lookup"><span data-stu-id="243c7-103">Deduplication</span></span>

<span data-ttu-id="243c7-104">**重複**要素は、検索結果が重複する項目を削除する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="243c7-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="243c7-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="243c7-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="243c7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="243c7-106">Attributes and elements</span></span>

<span data-ttu-id="243c7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="243c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="243c7-108">属性</span><span class="sxs-lookup"><span data-stu-id="243c7-108">Attributes</span></span>

<span data-ttu-id="243c7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="243c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="243c7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="243c7-110">Child elements</span></span>

<span data-ttu-id="243c7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="243c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="243c7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="243c7-112">Parent elements</span></span>

<span data-ttu-id="243c7-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="243c7-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="243c7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="243c7-114">Text value</span></span>

<span data-ttu-id="243c7-115">の**場合は true**重複除外要素のテキスト値は、検索結果に重複するアイテムが含まれていない可能性があることを示します。</span><span class="sxs-lookup"><span data-stu-id="243c7-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="243c7-116">**False**の値は、検索結果に重複するアイテムが含まれている可能性があることを示します。</span><span class="sxs-lookup"><span data-stu-id="243c7-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="243c7-117">備考</span><span class="sxs-lookup"><span data-stu-id="243c7-117">Remarks</span></span>

<span data-ttu-id="243c7-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="243c7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="243c7-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="243c7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="243c7-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="243c7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="243c7-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="243c7-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="243c7-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="243c7-122">Schema name</span></span>  <br/> |<span data-ttu-id="243c7-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="243c7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="243c7-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="243c7-124">Validation file</span></span>  <br/> |<span data-ttu-id="243c7-125">types.xsd</span><span class="sxs-lookup"><span data-stu-id="243c7-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="243c7-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="243c7-126">Can be empty</span></span>  <br/> |<span data-ttu-id="243c7-127">false</span><span class="sxs-lookup"><span data-stu-id="243c7-127">false</span></span>  <br/> |
   

