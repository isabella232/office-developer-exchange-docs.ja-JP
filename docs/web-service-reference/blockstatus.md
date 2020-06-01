---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: BlockStatus 要素は、アイテムのブロック状態を指定します。
ms.openlocfilehash: e88236274bfa70216e872025c2a94231f837df1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462277"
---
# <a name="blockstatus"></a><span data-ttu-id="222e1-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="222e1-103">BlockStatus</span></span>

<span data-ttu-id="222e1-104">**Blockstatus**要素は、アイテムのブロック状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="222e1-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="222e1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="222e1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="222e1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="222e1-106">Attributes and elements</span></span>

<span data-ttu-id="222e1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="222e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="222e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="222e1-108">Attributes</span></span>

<span data-ttu-id="222e1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="222e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="222e1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="222e1-110">Child elements</span></span>

<span data-ttu-id="222e1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="222e1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="222e1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="222e1-112">Parent elements</span></span>

|<span data-ttu-id="222e1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="222e1-113">**Element**</span></span>|<span data-ttu-id="222e1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="222e1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="222e1-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="222e1-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="222e1-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="222e1-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="222e1-117">連絡先</span><span class="sxs-lookup"><span data-stu-id="222e1-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="222e1-118">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="222e1-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="222e1-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="222e1-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="222e1-120">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="222e1-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="222e1-121">アイテム</span><span class="sxs-lookup"><span data-stu-id="222e1-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="222e1-122">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="222e1-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="222e1-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="222e1-123">Text value</span></span>

<span data-ttu-id="222e1-124">**Blockstatus**要素のテキスト値が**true の場合**は、アイテムがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="222e1-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="222e1-125">値が**false**の場合は、アイテムがブロックされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="222e1-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="222e1-126">注釈</span><span class="sxs-lookup"><span data-stu-id="222e1-126">Remarks</span></span>

<span data-ttu-id="222e1-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="222e1-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="222e1-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="222e1-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="222e1-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="222e1-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="222e1-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="222e1-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="222e1-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="222e1-131">Schema Name</span></span>  <br/> |<span data-ttu-id="222e1-132">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="222e1-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="222e1-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="222e1-133">Validation File</span></span>  <br/> |<span data-ttu-id="222e1-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="222e1-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="222e1-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="222e1-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="222e1-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="222e1-136">See also</span></span>



- [<span data-ttu-id="222e1-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="222e1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

