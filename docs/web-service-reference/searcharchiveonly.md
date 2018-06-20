---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: SearchArchiveOnly 要素は、非インデックス付け可能なアイテムのアーカイブ メールボックスのみを検索するかどうかを示します。
ms.openlocfilehash: ac9d3262784d8052486c631ef3e99e650d4757c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833293"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="a3f55-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="a3f55-103">SearchArchiveOnly</span></span>

<span data-ttu-id="a3f55-104">**SearchArchiveOnly**要素は、非インデックス付け可能なアイテムのアーカイブ メールボックスのみを検索するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a3f55-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="a3f55-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="a3f55-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3f55-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a3f55-106">Attributes and elements</span></span>

<span data-ttu-id="a3f55-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3f55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3f55-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3f55-108">Attributes</span></span>

<span data-ttu-id="a3f55-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a3f55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3f55-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a3f55-110">Child elements</span></span>

<span data-ttu-id="a3f55-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a3f55-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3f55-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a3f55-112">Parent elements</span></span>

<span data-ttu-id="a3f55-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="a3f55-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a3f55-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a3f55-114">Text value</span></span>

<span data-ttu-id="a3f55-115">の**場合は true** 、 **SearchArchiveOnly**要素のテキスト値は、その非インデックス付け可能な項目のみが検索されますアーカイブ メールボックスのことを示します。</span><span class="sxs-lookup"><span data-stu-id="a3f55-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="a3f55-116">テキスト値が**false**のでは、プライマリ メールボックスとアーカイブ メールボックスに対して検索が実行されることを示します。</span><span class="sxs-lookup"><span data-stu-id="a3f55-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a3f55-117">備考</span><span class="sxs-lookup"><span data-stu-id="a3f55-117">Remarks</span></span>

<span data-ttu-id="a3f55-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a3f55-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3f55-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a3f55-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3f55-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="a3f55-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3f55-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="a3f55-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3f55-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a3f55-122">Schema name</span></span>  <br/> |<span data-ttu-id="a3f55-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a3f55-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3f55-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a3f55-124">Validation file</span></span>  <br/> |<span data-ttu-id="a3f55-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3f55-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3f55-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3f55-126">Can be empty</span></span>  <br/> ||
   

